# The Learn Path

The order the guide teaches in. Each step gives a real win using one tool that is already in this folder, names the skill it just taught, then offers the next step. Value first, every time. Concepts come after the win, never before.

If you are the guide, follow this order. Do not skip ahead, do not front-load. One step, one win, then check in. Write a one-line update to `.remix/state.md` after each step so the next session resumes here.

If you are a person reading this yourself, you do not have to. Just open the folder in Claude Code and say hi, or run `/start`. The guide walks you through this.

---

## Step 1. The win (start here, always)

**Tool: `/today`. Skill taught: turn a messy brain dump into a sorted day.**

Get them a real result in under five minutes, before any explanation. Say one line and wait:

> Tell me about your day. Dump it all, messy is fine. What is on your plate, what is worrying you, what is due.

Take whatever they give you and produce a sorted `today.md` (the `/today` command has the full recipe). Two things have to happen in this first beat:

1. **They watch you ask before you act.** Before you create the file, say what you are about to do and that you will not touch anything they did not ask for. Let them see the AI ask permission. That kills the black-box fear on contact.
2. **They see the file appear.** Point at it. "That is a real file on your machine, you own it, you can open it in any editor." The work is visible.

End with the win named, not a lecture. "That is the whole idea. You talked, you got a sorted day. Want to see how it remembers things so tomorrow is sharper?"

Log to state: `step: 1 done (first today.md)`.

## Step 2. The front door

**Tool: `/capture`. Skill taught: one place to throw anything, it gets filed for you.**

Now show them the intake. A stray thought, a name, a link, a task. They say it, `/capture` routes it to the right place. This is the habit that feeds everything else. Keep it to one real capture, then name it. "That is your front door. Anything that pops into your head goes here and lands in the right spot."

Log to state: `step: 2 done (first capture)`.

## Step 3. In your voice

**Tool: `/draft`. Skill taught: it writes like you, and learns as it goes.**

Have them draft one small real thing (a follow-up, a note, a post). Show them it reads `context/voice.md`, and that as they correct it, it appends what it learned under `## Learned` and never overwrites their own words. The point that lands here is that it gets more like them over time.

Log to state: `step: 3 done (first draft)`.

## Step 4. Walk in ready

**Tool: `/prep` or `/process-transcript`. Skill taught: your meetings prep and file themselves.**

Pick whichever fits what they actually have in front of them. If they have a call coming, `/prep` builds the brief. If they have a transcript from one that happened, `/process-transcript` gives them a summary and action items, filed under the person. Either way, show the `people/` file it reads or writes.

Log to state: `step: 4 done (first prep or transcript)`.

## Step 5. The compounding reveal

**No new tool. Skill taught: why the whole thing is more than the parts.**

This is the moment. Show them that `context/` and `people/` are now feeding each other. Their sorted day knows what came out of the meeting. The draft knows how they write. The brief walks in already knowing the person. Nothing was wired by hand. Open `COMPOSE-CONTRACT.md` if they want the design, but lead with the felt result, not the diagram.

> Every tool reads the same two folders, `context/` and `people/`. That is the whole trick. Add another tool and it joins the same memory automatically.

Log to state: `step: 5 done (compounding reveal)`.

## Step 6. Personalize (late, on purpose)

**Skill taught: save your own rules once you have some worth saving.**

Only now, after they have felt it work, help them set a few light preferences in `context/you.md` and `context/voice.md`. Their name, their role, one or two "always do this, never do that" rules. This is deliberately late. Rules you save before you have used the thing are guesses. Rules you save now are real.

Keep it to what they actually want. Do not build scaffolding. Do not turn this into a config chore.

Log to state: `step: 6 done (personalized)`.

## Step 7. Evolve

**Skill taught: where this goes when you want more.**

They now run a real personal system by hand. Name the next rung honestly and point to it. This is where `LADDER.md` comes in, Assembled for when they want it to run itself, the Membership for staying sharp, Personal Setup if they want Andy to build it with them. Do not oversell. This repo already gave them something real. The ladder is there when they want it.

Log to state: `step: 7 done (path complete)`.

---

## Notes for the guide

- If the person jumps ahead ("just show me the writer"), let them. Run the tool, then offer to loop back to what they skipped. The order is the default, not a cage.
- If a step's tool needs a value you do not have, use a `{placeholder}` and keep moving. Never stall the win.
- MCP, automation, scheduling, and multi-machine sync are not on this path. They are the Kit. Do not teach them here.
