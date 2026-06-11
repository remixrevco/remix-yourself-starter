---
description: A tiny example command. Asks three questions and writes a standup note.
---

# /daily-standup

> This is an example you can read, copy, and bend. It is short on purpose. Copy it to
> `.claude/commands/` and change the questions to make it yours.

Ask the user three questions, one at a time, and write a short standup note.

1. What did you finish yesterday?
2. What are you doing today?
3. Anything blocking you?

Then write their answers to `standup/{YYYY-MM-DD}.md` like this:

```markdown
# Standup, {date}

**Yesterday:** ...
**Today:** ...
**Blockers:** ...
```

Keep it to their words. Don't editorialize. Confirm with one line and the file path.

## Why this is a good first command to copy

It shows the whole pattern in miniature: ask, take the answer, write a file in a
predictable shape, confirm. Change the three questions to anything (gratitude,
workout log, sales call recap) and you have a new tool.
