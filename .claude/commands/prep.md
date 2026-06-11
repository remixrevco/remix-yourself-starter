---
description: Build a pre-call brief. Who you're meeting, what matters, what to ask, what's open from last time.
---

# /prep

Build a tight pre-call brief the user can read in two minutes and walk in ready. Ground it in what they already know, then fill the gaps with research.

## On invocation

The user names a person, company, or meeting ("prep me for my call with Jane at Acme"). If they didn't, ask:

```
Who or what are you prepping for? A name, a company, or the meeting.
```

## Build the brief in three passes

1. **Memory first.** Read `context/you.md` (so the brief is framed for their role and goals), and any matching `people/<name>.md` (relationship, company, the `## Notes` history of past calls). This is the most valuable input, use it.
2. **Live research second.** If web access is available, look up what's current and relevant, the company, recent news, the person's role. Keep it to what changes how the call should go. Cite sources. If web access is not available, say so and build from memory.
3. **Synthesize, don't dump.** A brief is a decision aid, not a research report.

## Brief shape

Write to `briefs/{YYYY-MM-DD}-{name-slug}.md` and show it in chat:

```markdown
# Prep, {Person / Meeting}, {YYYY-MM-DD}

## Who
{Name, role, company. One line on the relationship if you have history.}

## Why this call matters
{What's at stake for the user, framed by their goals from context/you.md.}

## What's open from last time
{Pulled from people/<name>.md ## Notes. "Nothing on file" if new.}

## What to know
- {2 to 4 facts that actually change how the call should go}

## What to ask
- {2 to 3 sharp questions}

## Sources
- {links, if web research was used}
```

## File what you learned

If you researched a person who has (or warrants) a `people/<name>.md`, append a dated line under `## Notes` with anything durable you found. Append only, never overwrite. Create the file from the contract template if they're worth tracking and don't have one.

## Never

- Never pad the brief. Four facts that matter beat twelve that don't.
- Never present web claims as certain without a source.
- Never overwrite the user's notes on a person. Append under `## Notes`.
