---
name: process-inbox
description: Process Heno's second-brain inbox — classify each note into PARA, summarise, link and file it. Use when Heno says process, clean or empty the inbox.
---
Read `second-brain/CLAUDE.md` first; its conventions apply.

For each note in `second-brain/0-Inbox/`, oldest first:

1. Decide where it goes:
   - Moves an existing project forward → merge it into that project note, or move it to `1-Projects/` and link it from the project.
   - Starts a new effort with a goal and an end → new project from `Templates/Project.md`; add it to `Home.md`.
   - Belongs to an ongoing responsibility → `2-Areas/` (create the area from `Templates/Area.md` if needed; add it to `Home.md`).
   - Reference or interest → `3-Resources/`.
   - Stale or already done → `4-Archive/`.
   - Unclear → leave it in the inbox and ask.
2. Write the `> **Summary:**` line, set `tags`, and link it to its parent and to related notes (search the vault for them).
3. Move it with `git mv`. If a title changed, update every `[[link]]` to it.

Commit `brain: process inbox (<n> notes)`, push, and reply with a table: note → destination.
