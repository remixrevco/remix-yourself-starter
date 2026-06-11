---
description: Draft in your voice. Reads how you write, then learns from your edits.
---

# /draft

Write something in the user's voice, then learn from what they change. The goal is that draft two starts closer to them than draft one did.

## Before you write, read the voice

Read `context/voice.md` at the root of the current folder. It has three sections:

- `## Rules` — hard lines. Obey every one. If a rule says no em-dashes, use none.
- `## Samples` — real writing of theirs. Match the rhythm, sentence length, and vocabulary, not the topic.
- `## Learned` — your own past observations. Apply them.

If `context/voice.md` does not exist, self-seed it from the template in `COMPOSE-CONTRACT.md`, then ask the user to paste two or three samples or just describe how they want to sound. You can draft from a single sample or even from rules alone, but say that more samples sharpen it.

## On invocation

If the user did not say what to write, ask:

```
What do you want to write, and who's it for? Rough is fine, or just tell me the gist.
```

Take their gist, the audience, and any rough version they give you.

## How to draft

1. **Match the voice, not the average.** Read the samples for cadence. Short, punchy writers get short punchy drafts. Do not regress to generic business prose.
2. **Lead with the point.** Verdict or ask first, reasoning after, unless their samples clearly do otherwise.
3. **Obey the rules literally.** A `## Rules` line is non-negotiable.
4. **Keep it the right length.** A Slack reply is three lines, not three paragraphs. Match the medium.
5. **Give one draft, not three.** Confidence over a menu. Offer a variant only if they ask.

Show the draft, nothing around it. No preamble, no "here's a draft that...".

## Learn from the edit

After they react, capture what changed:

- If they edit it, compare their version to yours. What did they cut, soften, sharpen, reorder?
- If they say "more X" or "less Y," that is a rule.
- Append one or two concise observations to `context/voice.md` under `## Learned`, dated, newest last. Examples: `2026-06-10: cuts hedging words ("just", "I think"). Prefers a direct ask.`

Never rewrite anything above `## Learned`. The user's rules and samples are theirs. You only add below the line.

## Never

- Never use a banned construction from `## Rules`, not even once.
- Never overwrite the user's samples or rules.
- Never wrap the draft in explanation. Deliver the words.
