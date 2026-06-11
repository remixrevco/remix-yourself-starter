# Transcription Intake

Drop a meeting transcript in, get a clean summary plus action items, filed where they belong. The thing that turns an hour of talking into a paragraph and a to-do list, with the right people's names attached.

## What it does

Paste or drop a transcript from any tool, Granola, Fireflies, Gong, a voice memo, plain notes. It gives you a clean summary, the decisions, and the action items split out by who owns them. Then it files the relevant bits onto the people who were in the room.

## Get your first summary in a few minutes

1. Drop the `transcription-intake` folder into any folder.
2. Open it in Claude Code.
3. Drop a transcript file in, or paste one.
4. Run `/process-transcript`. Read the summary. Check the action items.

Works on the first transcript with nothing set up.

## What's in it

- `/process-transcript` — transcript to summary + decisions + action items
- It writes a clean summary file and updates the people involved

## How it remembers you

It reads `people/` to recognize who's who, and appends dated notes to `people/<name>.md` under `## Notes`. New person, new file. It never rewrites what you wrote, it only adds below the line. Self-seeds `people/` on first run.

So the second time someone shows up in a transcript, the system already knows them, and their file grows a history instead of starting over.

## It sticks together

This is the component that feeds the others. The people and notes it captures are what make the Researcher's briefs sharp and Today-Planning's priorities aware of what just happened. Drop it in a folder with those and the whole thing compounds.

## When you want more

Free processes a transcript when you run it. The Kit processes them automatically, while you sleep it reads the day's calls, drafts the follow-ups in your voice, and has them waiting at 6am. Same engine, no hands.
