# Second Brain — operating manual

Heno's second brain: a plain-markdown, Obsidian-compatible vault organised with PARA and maintained with Claude. Unrelated to the legacy website at the repo root.

## Structure

| Folder | Holds | Rule of thumb |
|---|---|---|
| `0-Inbox/` | Raw, unprocessed captures | Everything lands here first; empty it weekly |
| `1-Projects/` | Efforts with a goal and an end | "Done when…" can be stated |
| `2-Areas/` | Ongoing responsibilities with a standard to keep | Never "done" (Health, Finances, Career…) |
| `3-Resources/` | Topics and reference material of interest | Useful later, not tied to a responsibility |
| `4-Archive/` | Anything inactive from the above | Finished projects, dropped interests |
| `Daily/` | One note per day, `YYYY-MM-DD.md` | Focus, log and captures of the day |
| `Reviews/` | Weekly reviews, `YYYY-Www.md` (ISO week) | Output of `/weekly-review` |
| `Templates/` | Note templates | Copy them; never fill one in place |
| `Attachments/` | Images, PDFs, files | Created on first use |

`Home.md` is the index of every active project and area. Update it whenever one is created, archived or renamed.

## Note conventions

- Filename = note title in Title Case, e.g. `Sleep Protocol.md`. Daily and review notes use their date formats.
- Start each note from its template in `Templates/` and replace `{{title}}` / `{{date}}`. Notes in `0-Inbox/` and `3-Resources/` use `Note.md`.
- Line after the H1 is `> **Summary:**` — 1–3 sentences in Heno's words, written when the note is processed. Inbox notes may leave it blank.
- Link with `[[Note Title]]`; in frontmatter, quote links: `area: "[[Health]]"`. Every processed note links to its parent project/area or to ≥1 related note. When linking A → B, add B → A if it helps.
- Keep Heno's words. Don't pad, rewrite their voice or invent facts; mark your own additions *(Claude)*.
- Tasks are `- [ ]` checkboxes inside the project or daily note they belong to. No separate task list.

## Workflows

- **Capture** — `/capture`
- **Process** — `/process-inbox`
- **Review** — `/weekly-review`
- **Ask** — when Heno asks something the brain might know, search the vault first (`grep -ril`), answer from the notes and cite them as `[[links]]`. Say plainly when the brain has nothing on it.

## Rules

- Never delete a note without asking; move it to `4-Archive/` instead.
- Create subfolders inside a PARA folder only once ≥ 5 notes share a theme.
- Dates are ISO (`YYYY-MM-DD`).
- After changes, commit with a message starting `brain:` and push.
