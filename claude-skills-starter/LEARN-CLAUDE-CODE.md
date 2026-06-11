# Learn Claude Code in Five Minutes

You keep hearing "just use Claude Code." Here is enough to actually start. No prior coding required.

## What it is

Claude Code is an AI you run in a terminal that can read and write files in a folder. You point it at a folder, talk to it, and it does the work, drafting, sorting, summarizing, filing. It is not just chat. It can change the files in front of it.

That is the whole idea. A folder full of your stuff, and an assistant that can actually touch it.

## The three things you need to know

### 1. A folder is the workspace

Whatever folder you open Claude Code in, that is what it can see and change. This Starter is built around that. The components read a shared `context/` and `people/` folder, so the more you put there, the more the AI knows about you.

### 2. A command is a saved instruction

A command is a `/something` you can run. When you type `/capture`, Claude reads a file that tells it exactly how to behave. That file lives at `.claude/commands/capture.md`. Open it. It is just plain English, telling the AI what to do.

That is the trick that makes this not-magic. A command is a markdown file with instructions. You can read every one. You can change them.

### 3. You can make your own

Want a new command? Make a file at `.claude/commands/myidea.md`, write what you want it to do in plain English, and now `/myidea` exists. That is the entire mechanism.

## Make your first command (two minutes)

1. Look in `examples/`. There are a couple of small ones, read them, they are short on purpose.
2. Copy one to `.claude/commands/` and rename it.
3. Change the instructions to whatever you want.
4. Run it with `/yourname`.

You just built a tool. That is the loop, and it is the whole skill.

## The mental model that makes it click

You are not learning to code. You are learning to **write down what you want clearly enough that an assistant can do it every time.** A command is just a good instruction you saved so you never have to repeat it.

The people who get the most out of this are not the best programmers. They are the ones who got specific about their own workflow and wrote it down.

## Where to go next

- Run `/capture` and feel how routing works.
- Read the other components' commands in this Starter, they are all just markdown you can study.
- When you want the system to set itself up for you and run on its own instead of you running each command by hand, that is the Kit.
