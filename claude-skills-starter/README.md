# Claude Skills Starter

Road-tested skills that teach you Claude Code and automate the boring parts. The "learn this fast" on-ramp, plus a capture command that routes whatever you throw at it to the right place.

## What it does

Two things. It gets you fluent in Claude Code fast, with a short guide and a few skills you can read and copy. And it gives you `/capture`, a single command you can throw anything at, a thought, a task, a link, a name, and it files it where it belongs.

This is the component for the person who keeps hearing "just use Claude Code" and doesn't know where to start.

## Get going in a few minutes

1. Drop the `claude-skills-starter` folder into any folder.
2. Open it in Claude Code.
3. Read `LEARN-CLAUDE-CODE.md` (five minutes).
4. Run `/capture` and dump something. Watch where it lands.

## What's in it

- `/capture` — a quick-capture router that files thoughts, tasks, links, and contacts
- `LEARN-CLAUDE-CODE.md` — the fast on-ramp, what a skill is, what a command is, how to make your own
- `examples/` — small, readable example skills you can copy and bend

## How it remembers you

It keeps a light `context/` stub so captured items have somewhere to go, and writes new `people/` files when you capture a name. Self-seeds on first run. The router gets more useful as your other components give it more places to file things.

## It sticks together

`/capture` is the front door for the whole Starter. Capture a name and the Researcher can prep it. Capture a task and Today-Planning can prioritize it. The more components in the folder, the smarter the routing.

## When you want more

Free teaches you the mental model and gives you the basics. The Kit ships the full skill library and, more importantly, builds your config for you instead of making you learn it first. This component is the bridge, it's how you learn enough to know you want the Kit.
