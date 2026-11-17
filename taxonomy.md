# Taxonomy

Definitions only. Design guidance that uses these terms lives in:

- [promises.md](promises.md): how promises work and how to keep them
- [curves.md](curves.md): reading and fixing curves, early game, retention
- [unfolding.md](unfolding.md): how mechanics connect
- [legibility.md](legibility.md): why legibility matters and what it covers
- [prestige.md](prestige.md): when and how to use prestige
- [playtesting.md](playtesting.md): simulated playtests, repetition, automation
- [choices.md](choices.md): meaningful vs. artificial choices
- [attention.md](attention.md): active vs. occasional players

Terms are ordered so that each one only builds on terms above it.

> **About examples:** Examples in this repository are illustrative only. They show what a principle means; they are **not** themes, mechanics, numbers, or structures to copy. See [README](README.md#principles-not-a-spec).

---

## Incremental Game

**A game in which the player builds out their economy and their power.**

The thrill is that **you cover a lot of distance**: you get much stronger. There are many, many things to unlock and many, many challenges, and a combination of things you can upgrade, build, or improve helps you get there faster. What seems far away early in a session can be close by the end of it, because the player's ability to produce improves very rapidly.

## Unfolding Incremental Game

**A genre in which the scope revealed at the start is much smaller than the full scope.**

- As you play, more ways and more things are revealed, so the scope feels like it grows over time.
- Generally, things refer to each other: what is revealed later helps with what came before.

> **Example (illustrative only):** you start farming, then unlock fishing, and fishing helps your farming.

---

## Mechanic

**A set of rules that refer to each other and enable actions and progress in the game.**

- **Bounded by** its items, its currencies, and its main progression arc.
- **Currencies:** a mechanic may buy things with another mechanic's currency, but the currencies a mechanic produces are always usable in that mechanic.
- **Standalone:** a mechanic can be a standalone game.
- **Theme:** a mechanic usually has its own theme; different themes mean different mechanics.
- **Verb:** a mechanic usually has its own verb, the core action the player performs.

## Engine

**A way to progress within a mechanic, defined by what drives it.**

A mechanic starts with just a few of its engines and expands into more. Different engines push toward the same goal through different drivers.

> **Example (illustrative only):** in a *kill → get gold → upgrade the killer* mechanic, gold is the engine. Adding research that improves the killer on a timer adds a second engine driven by time.

---

## Unfolding

**Unlocking something new.** There are two very different types:

1. [Expansion](#expansion): more of an existing mechanic is revealed.
2. [New Mechanic](#new-mechanic): a whole new mechanic is revealed.

## Expansion

**Revealing another aspect of an existing mechanic, usually a new [engine](#engine).**

We're still in the same mechanic and still pushing the same goal, but there's a new way to progress.

## New Mechanic

**Unfolding into an entirely new mechanic.** It:

- **Almost always introduces a new currency.**
- **Almost always introduces a new verb.**
- **Is usually separated from other mechanics** (e.g. its own tab); you don't usually see two mechanics on screen at the same time.
- **Starts from scratch.** At first it feels like starting a new game.
- **Feeds back.** After some progress, it benefits your other mechanics (or one specific mechanic). You return with fresh energy and progress where you were stuck.

---

## Promise

**Something the player knows is coming: "once you have this, you will get something."**

- A surprise is **not** a promise. The player has to know it's coming.
- The player knows the **condition** and the **kind** of reward, not the exact reward.
- **The big promises in an unfolding incremental game are [expansions](#expansion) and [new mechanics](#new-mechanic).**
- Promises are the **meta engine** of the game: after playing for a while, the player's main goal is reaching the next promise or promises.

> **Analogy:** tell a kid, "If you count to 100, I'll give you a treat." That's a promise. Whether they count to 100 next time depends on the quality of the treat.

See [promises.md](promises.md).

## Promise Noun

**How the game tells the player what kind of thing a promise holds**, through what it's called, or where and how it sits in the UI.

A different noun means a different kind of promise. If the game is consistent about what kind of thing sits behind each noun, the player learns it and reacts appropriately.

The specific nouns are up to each game.

## Promise Size

An unfolding incremental game needs **a few sizes** of promise, and the player should learn to tell them apart by their [noun](#promise-noun).

What the sizes are, and what sits at each, depends on the game.

---

## Curve

**The graph of a timestamped log of every purchase and unlock in a play session.**

A curve can be spaced out (nothing bought, or nothing unlocked, for a long time), dense, or oscillating between fast and slow.

See [curves.md](curves.md).

## Legibility

**The player can understand the game well enough to predict how long progress takes.**

Covers both the game itself (UI, what there is to learn) and its mechanics and progression (how things scale). See [legibility.md](legibility.md).

## Stale

**A curve that slows down predictably, with nothing happening for a long time.**

---

## Prestige

**Resetting progress in exchange for something lasting.** Can apply to the whole game or to a specific mechanic.

See [prestige.md](prestige.md).

## Automation

**A way for the game to perform a repeated player action** (e.g. allocating by a ratio, auto-building).

See [playtesting.md](playtesting.md#automation).
