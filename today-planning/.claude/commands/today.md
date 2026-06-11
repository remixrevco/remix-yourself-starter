---
description: Voice dump in, a prioritized day out. Talk the way you think and get a sorted today.md back.
---

# /today

Turn a raw brain dump into a prioritized day. The user talks the way they actually think, half-formed and jumping around. You return a clean, ordered `today.md`.

## On invocation

If the user did not already dump, say one line and wait:

```
Tell me about your day. Dump it all, messy is fine. What's on your plate, what's worrying you, what's due.
```

Then take whatever they give you, in any order, and sort it.

## Before you sort, read the memory (if present)

Look for a shared memory at the root of the current folder. Read what exists, skip what doesn't. Never fail because it's missing.

- `context/you.md` — their role and working style, so priorities are framed for them.
- `context/projects.md` — active projects, so loose tasks attach to the right work.
- A `people/` folder — recognize names they mention.

If `context/` does not exist, create it on first run from the templates in `COMPOSE-CONTRACT.md` (a minimal `you.md` and `projects.md`), tell the user you seeded it, and continue. The first day never waits on setup.

## How to sort

Produce a `today.md` in the current folder. Order by what actually matters today, not by the order they said it.

1. **Pull the avoided thing to the top.** The task they buried or said with a sigh ("I should probably...") usually matters most. Name it first.
2. **Group by area** only if there is enough to warrant it (Work, Admin, Personal). A short day stays one list.
3. **Make each item a real next action**, not a vague topic. "Send Jim the one-pager" not "Jim stuff."
4. **Surface what's time-boxed** (a meeting, a hard deadline, "before 2") at the top of its group with the time.
5. **Carry nothing you invented.** Only what they said. Use a `{add detail}` placeholder if something is unclear rather than guessing.

## today.md shape

```markdown
# Today, {YYYY-MM-DD}

## Focus
The one thing that makes today a win.

## Do
- [ ] {highest-priority next action}
- [ ] {next}

## Time-boxed
- {time} — {what}

## If there's time
- [ ] {nice-to-have}

## Notes
{anything that was context, not a task}
```

If a `today.md` already exists for today, append new items under the right headings rather than overwriting. Roll yesterday's unchecked items forward into `Do` and note them as carried.

## After writing

Archive a copy to `daily/{YYYY-MM-DD}.md` so there's a history. Then show the user the `## Focus` and `## Do` list in chat, nothing else. End with one line, not a summary:

```
Sorted. Focus is {the one thing}. Run /wrap tonight to close the loop.
```

## Never

- Never invent tasks, dates, or people.
- Never rewrite a section the user hand-edited above a list.
- Never lecture about productivity. Sort the day and get out of the way.
