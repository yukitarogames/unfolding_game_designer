# Unfolding Game Designer

Knowledge and taste for developing unfolding incremental games, written to guide the development of new ones.

## Principles, not a spec

This repository defines **what good looks like** without constraining what kind of game can emerge from it.

- It holds **taxonomy and principles only**. It does not prescribe themes, mechanics, numbers, promise sizes, UI conventions, or structures.
- **No examples.** Concrete game examples (themes, mechanics, numbers) pull every new game toward the same shape, so this repository doesn't contain them. The only illustrations are analogies from outside games.
- Where a principle leaves something open, the choice belongs to each game.
- **Fun comes first.** The rest of the principles keep a fun game going; they can't make a boring one fun. See [fun.md](fun.md).

## Deliberately left to judgment

These have no principle here on purpose. Decide them per game:

- **Unfold timing:** how far apart unfolds are. It just needs to make sense.
- **Expansion vs. new mechanic:** which one a given moment needs.
- **Endings:** not a thing in this repository. If a game needs one, it's a late-development decision.
- **Failure modes:** there are many; this repository doesn't try to list them all.

## How it's used

> **Agents:** before designing or reviewing a game with this repository, read and follow [CLAUDE.md](CLAUDE.md).

Designs are made by a `designer` subagent that sees only [taxonomy.md](taxonomy.md) and [fun.md](fun.md), and reviewed by a `judge` subagent that sees everything. The main agent runs the loop between them. See [CLAUDE.md](CLAUDE.md) and [.claude/agents/](.claude/agents/).

## Files

| File | What it holds |
|------|---------------|
| [taxonomy.md](taxonomy.md) | Definitions of the shared vocabulary. Start here. |
| [fun.md](fun.md) | What makes a mechanic worth playing. Comes first. Read by both designer and judge. |
| [mechanics.md](mechanics.md) | Dictionary of mechanic forms: what's possible and what makes each work. Read by the judge, not the designer. |
| [promises.md](promises.md) | How promises drive the player, and the rules for keeping them. |
| [curves.md](curves.md) | Reading and fixing progression curves, the early game, retention. |
| [unfolding.md](unfolding.md) | How unfolds work and how mechanics connect. |
| [legibility.md](legibility.md) | Why legibility matters and what it covers. |
| [prestige.md](prestige.md) | When and how to use resets and prestige. |
| [playtesting.md](playtesting.md) | Simulated playtests: curves, repetition, automation. |
| [choices.md](choices.md) | What makes player choices meaningful, and what makes them bad. |
| [attention.md](attention.md) | Accommodating players who check in often and rarely. |
