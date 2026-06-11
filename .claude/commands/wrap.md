---
description: Evening close-the-loop. What got done, what slipped, what's tomorrow.
---

# /wrap

Close the day. Read today's plan, find out how it went, and set up tomorrow. Short and honest, not a performance review.

## On invocation

Read `today.md` in the current folder. If there isn't one, say so and offer to run `/today` instead.

Then ask one open question and wait:

```
How did today go? Tell me what got done and what slipped.
```

Take their answer. Do not interrogate. One follow-up at most if something important is unclear.

## What to do

1. **Mark the plan against reality.** In `today.md`, check off what got done. Leave what slipped unchecked.
2. **Capture what happened that wasn't on the list** under `## Notes` (a call that came in, a decision made). Append, dated, never overwrite.
3. **Roll the unfinished forward.** Anything still unchecked becomes tomorrow's starting set. Write a short `## For tomorrow` block at the bottom of `today.md`.
4. **Update projects if a project moved.** If they mention progress on something in `context/projects.md`, append a dated line under that project's heading (under `Next:` or a `## Log`), never rewriting what's there. Skip if `context/` is absent.
5. **Note the people**, lightly. If they mention an interaction with someone who has a `people/<name>.md` file, append a one-line dated note under that file's `## Notes`. Don't create new people files here, that's what `/capture` and `/process-transcript` are for.

## Close

Archive the final `today.md` to `daily/{YYYY-MM-DD}.md` (overwrite the morning copy with the end-of-day version). Then one line to the user:

```
Day closed. {N} done, {M} carried to tomorrow. {one honest note if there is one.}
```

## Never

- Never guilt-trip about what slipped. State it plainly and carry it forward.
- Never rewrite human-authored notes. Append below the line, dated.
- Never invent outcomes the user did not report.
