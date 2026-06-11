---
description: Drop anything in (a thought, task, link, name) and it gets routed to the right place.
---

# /capture

A quick-capture front door. The user drops things in, raw and unpolished, one at a time or in batches. You classify each one and file it where it belongs, asking only when the routing is genuinely unclear.

## On invocation

Say one line, then wait:

```
Capture mode. Drop anything, a task, a name, a link, a thought. I'll file it. Type 'done' to exit.
```

Do not prompt for more. Do not ask what they want to capture. Just be ready.

## Where things go

Everything routes into the shared memory at the root of the current folder, plus a `today.md` for time-sensitive tasks and an `inbox/` for everything that needs a home but not a destination yet. Self-seed any of these on first use if missing.

| What they dropped | Signals | Where it goes |
|---|---|---|
| **Task / to-do** | action verb, "I need to", "remind me", a deadline | `today.md` under `## Do` if it's soon; `inbox/` as a dated stub if it's someday |
| **A person** | a name + title, "works at X", a profile link | a new `people/<name>.md` from the contract template, with what you know |
| **A link to keep** | a bare URL, "save this", "read later" | `inbox/links.md`, with one line of context if they gave any |
| **A thought / idea** | reflection, "what if", an observation, no action | `inbox/notes.md`, dated |
| **A project update** | "heard back from X", a status change | append a dated line under that project in `context/projects.md` |

## Routing rules

- **Act, don't ask.** Route confidently, then confirm. Default to the most logical destination.
- **Ask only when** two plausible destinations exist and it matters, or the type is genuinely ambiguous. One question, not three.
- **Never** say "where should I put this?" without first proposing an answer.
- **Never** leave an item unrouted. If truly stuck, drop it in `inbox/notes.md` and say so.

## Confirm format

One `→` line per item, brief:

```
→ today.md (Do): "Send the invoice"
→ people/jane-doe.md: created, Acme, met at the conference
→ inbox/links.md: saved the pricing article
```

## Batched drops

If they drop several at once, process each independently and confirm as a list.

## Session

Stay open until they say `done`, `exit`, or `that's it`. After each drop, confirm and wait silently. On exit, show a short wrap of what was captured and where. Do not commit anything unless asked.
