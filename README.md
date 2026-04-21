# Claude Session Handoff Template

A structured HTML template for maintaining continuity across Claude AI sessions.

Claude has no memory between conversations. This template solves that by giving each new Claude instance a complete project briefing — so you can pick up exactly where you left off, without re-explaining your project from scratch.

---

## The problem this solves

Every time you start a new Claude conversation, Claude knows nothing about your project. If you're doing ongoing work — writing a book, designing software, researching a complex topic, planning something with many moving parts — you spend the first part of every session re-explaining context. This is friction, and it compounds over time.

The handoff file is a structured briefing document you update at the end of each session and upload at the start of the next. Claude reads it and resumes as if the previous conversation never ended.

---

## What's in the template

| Section | What goes here |
|---|---|
| §1 Session status | What happened this session — decisions made, things deferred, scope changes |
| §2 Top priority | The single most important thing for next session, with a concrete workflow |
| §3 Current state | Where things actually stand right now — what exists, what's been decided, what's ruled out |
| §4 File inventory | Every file that matters, where it lives, and its current status |
| §5 Watch items | Hard constraints, dependencies, known risks |
| §6 Operating core | Your project's methodology, vocabulary, decision rules, and quality standards |
| §7 Resume instructions | Direct instructions to the next Claude instance |
| §8 Session notes | New rules or precedents established this session |

The **Operating Core (§6)** is the most important section. It tells Claude *how to think* about your project — your methodology, your standards, your constraints — so it applies your approach consistently without being re-briefed each time.

---

## How to use it

### First session
1. Download `template.html`
2. Open it in any text editor or your browser's developer tools
3. Fill in every `▶ placeholder` with your project's content
4. Delete the usage guide block at the top
5. Save as `your-project-handoff-YYYY-MM-DD.html`

### Starting a session
Upload the file to Claude and say:
> *"Please read this handoff and resume from where we left off."*

That's it. Claude will read the file and pick up where you left off.

### Ending a session
Ask Claude to help you update the handoff:
> *"Please update the handoff file with what we accomplished today, any new decisions, and the top priority for next session."*

Download the updated file and save it for next time. Keep previous versions if you want a history.

---

## Works from anywhere

Upload from:
- **Google Drive** — open on any device, share with collaborators
- **iCloud** — works from iPhone/iPad without a computer
- **Dropbox, OneDrive** — any cloud storage
- **Local storage** — direct file upload from your device

No special tools, no plugins, no accounts required beyond Claude itself.

---

## Who this is useful for

- **Writers and researchers** working on long-form projects across many sessions
- **Developers** using Claude for ongoing architecture or code review work
- **Anyone running complex, multi-session projects** — legal analysis, business planning, academic work, creative projects
- **Teams** where multiple people interact with Claude on the same project (share the handoff file)
- **Mobile users** who don't have ready access to paste context but can upload a file

---

## Tips for getting the most out of it

**Be specific in §3 (Current State).** "We decided to use approach X because Y, and ruled out Z because W" is far more useful than "we discussed approaches." Claude can only work with what's written.

**The Operating Core (§6) compounds over time.** The more precisely you define your methodology, decision rules, and vocabulary, the less you need to correct Claude mid-session. Invest time in §6 early and update it when you establish new rules.

**Keep a version history.** Rename each session's file with the date: `project-handoff-2026-04-21.html`. You get a natural project log and can roll back if needed.

**Let Claude write the update.** At the end of a productive session, ask Claude to draft the updated handoff. It has full context of what happened and can populate §1, §2, and §8 accurately. You review and save.

**Use it for any ongoing work, not just complex projects.** Even a simple recurring task benefits from a handoff if you do it across multiple sessions — the setup cost is low and the continuity payoff compounds quickly.

---

## Customising the template

The template is plain HTML with embedded CSS — no dependencies, no build step. Customise freely:

- **Add sections** for your project type (e.g. a patch queue for software projects, a chapter tracker for books)
- **Change the colour scheme** — the callout box colours are defined in the `<style>` block at the top
- **Pre-populate §6** with your standing methodology so you don't re-fill it each session (this is particularly valuable for ongoing projects with stable processes)
- **Add a project-specific naming convention** to §6 so Claude always produces files with consistent names

---

## File format note

The template is `.html` rather than `.md` or `.docx` because:

- It renders correctly in any browser with no tooling
- It can be uploaded directly to Claude from any device
- The coloured callout boxes provide visual hierarchy that aids skimming — useful when you're quickly checking what Claude should prioritise
- It requires no markdown parser, no Google account, no special software

---

## Contributing

Issues and PRs welcome. If you've adapted the template for a specific project type (software development, academic research, legal work, creative writing) and want to contribute a variant, open a PR with your version in the `examples/` directory.

---

## License

MIT — use freely, adapt freely, attribution appreciated but not required.
