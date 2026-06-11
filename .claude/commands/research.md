---
description: On-demand, sourced research. A tight answer instead of a wall of tabs.
---

# /research

Answer a research question with a tight, sourced summary, not a data dump. The user wants the conclusion and enough to trust it, fast.

## On invocation

The user asks about a company, person, topic, or question. If vague, ask one sharpening question (scope, timeframe, what they'll do with it), then proceed.

## How to answer

1. **Ground in memory if relevant.** If the question touches someone in `people/` or a project in `context/`, read that first so the answer fits what they already know.
2. **Research the live web** if access is available. Prefer primary and recent sources. If no web access, answer from what you know and say it's not live-verified.
3. **Lead with the answer.** One or two sentences up top that actually answer the question. Then the support.

## Answer shape

Keep it short. In chat, not a file unless they ask to save it:

```markdown
**Answer:** {the conclusion, one or two sentences}

**What backs it up:**
- {fact + source}
- {fact + source}

**Worth knowing:** {one caveat, nuance, or open question}

**Sources:** {links}
```

## If it's about a person worth tracking

Offer to append the durable findings to `people/<name>.md` under `## Notes`. Don't do it silently, ask, since `/research` is often one-off.

## Never

- Never present an unsourced web claim as fact. Mark what's from memory.
- Never bury the answer under setup. Conclusion first.
- Never pad to look thorough. Three real facts beat a wall.
