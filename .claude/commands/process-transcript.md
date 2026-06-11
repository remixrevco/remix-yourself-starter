---
description: Turn a meeting transcript into a summary, decisions, and action items by owner. Files notes onto the people involved.
---

# /process-transcript

Take a raw transcript and return a clean summary, the decisions, and action items split by who owns them. Then file what matters onto the people who were in the room.

## Get the transcript

The user will paste a transcript or point you at a file in the current folder (any source, any format, Granola, Fireflies, Gong, a voice memo, plain notes). If they ran the command with nothing, ask:

```
Paste the transcript, or tell me the file name. Any format works.
```

## Read the people first

Before summarizing, glance at the `people/` folder in the current folder so you recognize who's who and use their real names. If `people/` does not exist, self-seed it. Don't block on it, an unknown attendee is fine.

## Produce the summary

Write a summary file to `transcripts/{YYYY-MM-DD}-{short-slug}.md` in this shape:

```markdown
# {Meeting name or topic}, {YYYY-MM-DD}

## Summary
{3 to 6 sentences. What it was about and what came of it. Plain, no fluff.}

## Decisions
- {decision made, if any}

## Action items
- [ ] **{owner}** — {the action} {due date if stated}
- [ ] **{owner}** — {the action}

## Open questions
- {anything left unresolved}
```

Rules for action items:

- **Split by owner.** Include other people's action items, not just the user's. Use the attendee's name as the owner.
- **Real next actions**, not topics. "Send the revised SOW" not "SOW discussion".
- **Only what was actually said.** Don't invent owners, dates, or commitments. Use `{owner unclear}` rather than guessing.

## File onto the people

For each attendee who has (or should have) a `people/<name>.md` file, append a dated note under `## Notes`:

```markdown
- {YYYY-MM-DD}, {meeting}: {one line of what's relevant about them or what they own}
```

- Match names case-insensitively. If someone new and clearly worth tracking appears, create `people/<name>.md` from the contract template.
- Append only, under `## Notes`, newest last. Never rewrite anything a human wrote above the line.

## Close

Show the user the `## Summary` and `## Action items` in chat. End with one line naming where the file landed and which people got updated. Don't commit unless asked.

## Never

- Never invent action items, owners, or due dates.
- Never overwrite human-authored content in a person's file.
- Never reformat or "improve" the user's own notes if they pasted some, summarize the transcript, leave their notes alone.
