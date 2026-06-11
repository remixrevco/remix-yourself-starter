# Today-Planning

Voice dump in, a prioritized day out. Plus an evening wrap that closes the loop. The 60-second wow of the Remix Yourself Starter, talk at it the way you actually think and get a sorted day back.

## What it does

Dump the mess in your head. Half-formed, run-on, jumping around. It comes back as a prioritized day, the real priorities sorted, the thing you are avoiding pulled to the top. At night, run the wrap and it closes the loop, what got done, what slipped, what's tomorrow.

Mess in, plan out. No perfect prompt required.

## Get your first day in 60 seconds

1. Drop the `today-planning` folder into any folder on your machine (or use it where it sits).
2. Open it in Claude Code.
3. Run `/today` and just talk. "Okay big meeting tomorrow I still owe Jim the one-pager also the invoice and I should walk the dog before 2."
4. Watch it write a prioritized `today.md`.

That's it. The first one needs nothing set up.

## What's in it

- `/today` — voice dump to a prioritized day
- `/wrap` — evening close-the-loop
- A `today.md` it writes and a `daily/` archive it keeps

## How it remembers you

On first run it self-seeds the shared memory if it isn't there:

- `context/you.md` — who you are, your role
- `context/projects.md` — what you are working on, so priorities land in context

It reads those to sort your day. It never needs them to give you the first one. The more you fill in, the sharper it gets.

## It sticks together

Drop another Starter component in the same folder and they share this memory. Add Transcription Intake and your day knows what came out of yesterday's calls. Add the Researcher and your day can pull a brief for the meeting it just prioritized. See `STICK-TOGETHER.md` at the repo root.

## When you want more

The free version is manual, you run it. The Kit makes it fire on its own every morning and wraps every night without you asking. That's the upgrade, not a different tool.
