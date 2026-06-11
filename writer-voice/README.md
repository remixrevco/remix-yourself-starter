# Writer / Voice

Drafts emails and posts in your voice, and remembers how you write so it gets closer every time. Paste a rough thought, get back something that sounds like you, not like a robot wearing your name.

## What it does

You write a rough version or just describe what you want to say. It drafts it in your voice. Then it remembers what you liked and what you changed, so the next draft starts closer. Over a few uses it stops sounding generic and starts sounding like you.

## Get your first draft in a few minutes

1. Drop the `writer-voice` folder into any folder.
2. Open it in Claude Code.
3. Paste two or three things you have actually written into `context/voice.md` under `## Samples`.
4. Ask it to draft an email with `/draft`. Compare. Edit. It learns from the edit.

## What's in it

- `/draft` — a drafting command that reads your voice before it writes
- `context/voice.md` — your rules, your samples, and a `## Learned` section it appends to

## How it remembers you

It reads `context/voice.md` every time it drafts:

- `## Rules` — your hard lines (e.g. no em-dashes, short sentences, no corporate filler)
- `## Samples` — a few things that sound like you
- `## Learned` — observations it appends over time, newest last. It never overwrites what you wrote.

Self-seeds the file on first run if it's missing. Works from samples alone, gets better with every edit.

## It sticks together

In a shared folder, your voice is available to every other component. The follow-up that Transcription Intake drafts, the outreach the Researcher preps, all of it can come out in your voice because they read the same `context/voice.md`.

## When you want more

Free learns your voice manually as you use it. The Kit wires the voice into every draft your system makes automatically, across all your workflows, and the Membership keeps the patterns improving with each week's drop.
