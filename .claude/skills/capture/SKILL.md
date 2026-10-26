---
name: capture
description: Capture an idea, link, quote, task or thought into Heno's second brain. Use when Heno says capture, save, remember or note this, or shares something to keep.
---
Read `second-brain/CLAUDE.md` first; its conventions apply.

Input: $ARGUMENTS (or what Heno just shared).

1. Split the input into distinct items — one idea per note.
2. For each item:
   - A task or update for an existing project or area → add it there (`- [ ]` under Next actions, or under Notes).
   - Otherwise → new note in `second-brain/0-Inbox/` from `Templates/Note.md`. Short, specific Title Case title; keep Heno's wording; fill `source` if there is one. For a URL, fetch it and add a 3–5 bullet gist under Notes, marked *(Claude)*.
3. Under `## Captures` in `second-brain/Daily/<today>.md` (create it from `Templates/Daily.md` if missing), append `- [[Note Title]] — one-line gist` per item.
4. Commit `brain: capture <n> item(s)` and push.
5. Reply with one line per item: where it went.
