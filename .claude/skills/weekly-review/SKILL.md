---
name: weekly-review
description: Run Heno's weekly second-brain review — empty the inbox, close open loops, update projects and set next week's focus. Use when Heno asks for a weekly review or reset.
---
Read `second-brain/CLAUDE.md` first; its conventions apply.

1. Run the `process-inbox` procedure until `0-Inbox/` is empty or only holds notes waiting on Heno.
2. Read the last 7 daily notes. Move unchecked tasks into their project, or into a list of open loops if they have none. Note recurring themes.
3. For each project in `1-Projects/`: confirm status and next action. Done or dropped → set `status: done`, move to `4-Archive/`, remove it from `Home.md`.
4. For each area in `2-Areas/`: flag any with no activity in the last 30 days.
5. Write `second-brain/Reviews/<YYYY-Www>.md` from `Templates/Weekly Review.md`; propose at most 3 focus items for next week and ask Heno to confirm them. Link it under `## Latest review` in `Home.md`.

Commit `brain: weekly review <YYYY-Www>`, push, and reply with the open loops and proposed focus.
