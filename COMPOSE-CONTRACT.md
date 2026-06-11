# The Compose Contract

The shared memory shape every component reads and writes. This is the single thing that lets standalone components stick together into a system. You never have to think about it to use the tools, but here is the whole design if you are curious or want to build your own component that fits.

## The promise this enables

Drop one component in a folder, it works alone. Drop a second one in the same folder, the two share one memory (your identity, your voice, your people, your projects) without any wiring. That shared memory is this contract. Nothing else is shared, no shared code, no shared config, no install step.

## The shape

Every component agrees on exactly one thing, a `context/` folder and a `people/` folder at the root of whatever folder it runs in. That is the whole contract.

```
your-folder/
├── context/
│   ├── you.md           identity, role, what you do
│   ├── voice.md         how you write (the Writer learns and appends here)
│   └── projects.md      what you are working on now
├── people/
│   └── <name>.md        one file per person you interact with
└── <component folders>  each component lives in its own folder, reads the two above
```

That is the floor, not the ceiling. Components may read and write their own working files (a `today.md`, a `daily/` archive, a `transcripts/` folder). Those are component-local outputs, not shared memory. The only cross-component surface is `context/` and `people/`.

## File schemas

Plain markdown. No required fields, editor-agnostic (works in Obsidian, VS Code, plain text). A human can read and edit any of these in ten seconds. Labels are sections, not strict schema, components read by heading and degrade gracefully if a heading is missing.

### context/you.md

```markdown
# You

- Name:
- Role:
- Company:
- What you do: (one or two sentences)
- Working style: (anything the AI should know, optional)
```

### context/voice.md

```markdown
# Voice

## Rules
- (e.g. short sentences, no corporate filler)

## Samples
- (paste a few sentences that sound like you)

## Learned
<!-- the Writer appends observations here, newest last, never overwrites above -->
```

### context/projects.md

```markdown
# Projects

## <project name>
- Status:
- Next:
```

### people/<name>.md

```markdown
# <Full Name>

- Relationship: (colleague / client / prospect / friend)
- Company:
- Context: (what matters about them)

## Notes
<!-- components append dated notes here: summaries, prep, follow-ups -->
```

Naming: `people/` uses kebab-case of the person's name, `people/jane-doe.md`. One person, one file. Components match case-insensitively and create the file if no match exists.

## Read and write rules

These rules are what keep components from fighting.

1. **Read freely.** Any component may read anything in `context/` and `people/` to personalize its output.
2. **Write narrowly.** A component writes only to the surfaces it owns:
   - The Writer appends to `context/voice.md` under `## Learned` only.
   - Transcription Intake and Researcher append to `people/<name>.md` under `## Notes` only, and create new `people/` files.
   - Today-Planning writes its own `today.md` and `daily/`, and may append to `context/projects.md` under an existing project heading.
3. **Append, never clobber.** Writes to shared files are additive and dated. Never rewrite a section a human authored. Human-authored content above a `## Learned` or `## Notes` marker is sacred.
4. **Self-seed if missing.** If `context/` or `people/` does not exist, the component creates the minimal stub on first run, so it works alone. It never fails because memory is absent.
5. **Stub, do not assume.** Unknown values use a visible placeholder (`{add role}`), never an invented one.

## The standalone guarantee

Each component produces real value on a clean machine with an empty or absent `context/`. First run, it self-seeds the stub, asks for the one or two things it needs, and delivers output. The shared memory makes it better over time and better when combined. It is never a prerequisite for the first result.

## Versioning

A one-line marker at the folder root, `.remix-compose`, containing `contract: v1`. Components check it on run. If absent, assume v1 and write it. This lets later contract versions migrate cleanly without breaking older folders.

## Build your own

Any tool that reads `context/` + `people/` and follows the five rules above is a compatible component. Drop it in the folder and it joins the system. That is the whole extension model.
