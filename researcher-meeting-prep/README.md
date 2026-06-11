# Researcher + Meeting Prep

Pre-call briefs and on-demand research, so you walk in ready. Ask it to prep you for a meeting and it pulls what it knows about the person plus what it can find, into one brief you can read in two minutes.

## What it does

Two jobs. Research, ask it about a company, a person, a topic, and get a tight, sourced answer instead of a wall of tabs. And meeting prep, point it at a call and get a brief, who you're meeting, what matters, what to ask, what's open from last time.

## Get your first brief in a few minutes

1. Drop the `researcher-meeting-prep` folder into any folder.
2. Open it in Claude Code.
3. Run `/prep` and name the person or meeting. "Prep me for my call with Jane at Acme."
4. Read the brief. Walk in ready.

## What's in it

- `/research` — on-demand, sourced answers
- `/prep` — a pre-call brief
- It writes briefs and updates the people it researched

## How it remembers you

It reads `people/` and `context/` to ground the brief in what you already know, then appends what it finds to `people/<name>.md`. Knows who you are from `context/you.md` so the brief is framed for your role. Self-seeds the stubs on first run, works on a cold name too.

## It sticks together

This component is best when it's not alone. Paired with Transcription Intake, every brief is built on the actual history of your calls with that person. Paired with Writer, the follow-up after the meeting comes out in your voice. Paired with Today-Planning, the prep shows up for the meeting your day already prioritized.

## When you want more

Free preps when you ask. The Kit preps every meeting on your calendar automatically and connects to your real tools, so the brief pulls from your actual email and docs, not just what you've captured. The Membership keeps adding new research and prep patterns every week.

## A note on sources

Web research needs Claude Code to have web access (a search or fetch tool enabled). If it doesn't, `/research` and `/prep` still work from what's in your `context/` and `people/` memory, and will tell you when a claim is from memory versus the live web.
