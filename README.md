# Remix Yourself Starter

Five working AI components for Claude Code. Each one is useful on its own. Drop two or more in the same folder and they share one memory, so the whole thing compounds.

This is a personal operating system, disassembled into its best parts, run by hand. Start with one. Add as you go.

**Never used this before?** Open the folder in [Claude Code](https://claude.com/claude-code) and run `/start`. A guide in Andy's voice gets you a real sorted day in about five minutes, then teaches the rest one step at a time. Want to look around first, run `/tour`. Using a different AI? Point it at [`AI-START-HERE.md`](./AI-START-HERE.md).

---

## The five components

| Component | What it does | Run |
|---|---|---|
| **today-planning** | Voice dump in, a prioritized day out. Evening wrap closes the loop. | `/today`, `/wrap` |
| **writer-voice** | Drafts in your voice and remembers how you write. | `/draft` |
| **claude-skills-starter** | Learn Claude Code fast, plus a `/capture` command that files anything. | `/capture` |
| **transcription-intake** | Drop a meeting transcript, get a summary + action items, filed by person. | `/process-transcript` |
| **researcher-meeting-prep** | Pre-call briefs and on-demand research, so you walk in ready. | `/prep`, `/research` |

---

## Two ways to use this

**Want the whole thing?** Open this folder in Claude Code. All five components are already here, already sharing one memory (`context/` + `people/`). Run any command above.

**Want just one?** Copy a single component folder (say `today-planning/`) anywhere on your machine and open that. It works alone and self-seeds its own memory on first run.

Either way, you need [Claude Code](https://claude.com/claude-code). That is the only dependency.

---

## The whole trick

Every component reads and writes two folders at the root of wherever it runs:

```
your-folder/
├── context/        who you are, how you write, what you're working on
├── people/         one file per person you deal with
└── <components>    drop as many as you want, they all read the two above
```

That is the entire contract. No install, no config, no glue code. Put two components in one folder and they share `context/` and `people/` automatically. Your planned day knows what came out of yesterday's calls. Your brief walks in already knowing the person. Your follow-up sounds like you. Nothing is wired by hand.

Full explanation in [`STICK-TOGETHER.md`](./STICK-TOGETHER.md).

---

## Start in 60 seconds

1. Open this folder in Claude Code.
2. Run `/today` and just talk. "Big meeting tomorrow, I still owe Jim the one-pager, also the invoice, and I should walk the dog before 2."
3. Watch it write a prioritized `today.md`.

The first run needs nothing set up. The more you fill in `context/`, the sharper everything gets.

---

## The rules that keep components from fighting

You do not need to know these to use it, but here is why it just works:

- **Read freely, write narrowly.** Every component can read your memory. Each only writes to its own corner of it.
- **Append, never clobber.** Components add to your files, dated. They never rewrite what you wrote.
- **Self-seed.** If `context/` or `people/` is missing, the first component you run creates it. You never hit a wall.

---

## When you want more

This is the system disassembled and run by hand. The **Kit** is the same parts assembled, with the part most people never figure out alone, it sets itself up by interviewing you, wires into your email and calendar and docs, runs on your phone, and ships with workflows tuned to your role.

The **Membership** is the standing home that keeps your system improving every week, new components, explainer videos, office hours, and a health check.

→ [See the ladder](https://remixsystems.co) · [Join the list](https://tally.so/r/D4yd0R)

Full walk of the rungs, and how to reach Andy before checkout is wired up, in [`LADDER.md`](./LADDER.md).

---

Built by [Remix Systems](https://remixsystems.co). Free to use, fork, and bend. MIT licensed, see [LICENSE](./LICENSE).
