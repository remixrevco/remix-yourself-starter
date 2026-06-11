---
description: A tiny example command. Summarizes any file you point it at into three bullets.
---

# /summarize-file

> An example you can read, copy, and bend. Copy it to `.claude/commands/` to use it,
> then change the output shape to whatever you need.

The user names a file (or pastes text). Read it and return a tight summary.

1. If they gave a file path, read it. If they pasted text, use that.
2. Return exactly three things:
   - **The point** in one sentence.
   - **Three bullets** of what matters.
   - **One open question** the file leaves unanswered, if any.
3. No preamble. No "here is a summary of". Just the summary.

## Why this is a good second command to copy

It shows that a command can take an input (a file or pasted text), not just ask
questions. Swap the output for "five bullets" or "a tweet" or "action items only"
and you have retargeted it in one edit. That is how every component in this Starter
was built, a clear instruction, a predictable output.
