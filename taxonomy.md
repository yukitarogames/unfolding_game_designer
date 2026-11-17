# Taxonomy

Definitions only. Design guidance that uses these terms lives in:

- [promises.md](promises.md): how promises work and how to keep them
- [curves.md](curves.md): reading and fixing curves, early game, retention

Terms are ordered so that each one only builds on terms above it.

---

## Incremental Game

**A game in which the player builds out their economy and their power.**

The thrill is that **you cover a lot of distance**: you get much stronger. There are many, many things to unlock and many, many challenges, and a combination of things you can upgrade, build, or improve helps you get there faster.

> If you start a session in the morning, what seems like weeks away might be minutes away by evening, because your ability to produce improves very rapidly.

## Unfolding Incremental Game

**A genre in which the scope revealed at the start is much smaller than the full scope.**

- As you play, more ways and more things are revealed, so the scope feels like it grows over time.
- Generally, things refer to each other.

> If you start farming and then unlock fishing, fishing would help you when you farm.

---

## Mechanic

**A set of rules that refer to each other and enable actions and progress in the game.**

- **Bounded by** its items, its currencies, and its main progression arc.
- **Currencies:** a mechanic may buy things with another mechanic's currency, but the currencies a mechanic produces are always usable in that mechanic.
- **Standalone:** a mechanic can be a standalone game.
- **Theme:** a mechanic usually has a theme. Fishing and farming are different themes, so they are different mechanics.
- **Verb:** each mechanic has its own verb (see [Verb](#verb)).

## Engine

**A way to progress within a mechanic, defined by what drives it.**

A mechanic starts with just a few of its engines and expands into more.

> In a *kill → get gold → upgrade the killer* mechanic, gold is the engine. Adding labs that research upgrades on a timer adds a new engine: **time**.

## Currency

_To define._

## Verb

_To define._ (Known examples: killing, fishing, building.)

---

## Unfolding

**Unlocking something new.** There are two very different types:

1. [Expansion](#expansion): more of an existing mechanic is revealed.
2. [New Mechanic](#new-mechanic): a whole new mechanic is revealed.

## Expansion

**Revealing another aspect of an existing mechanic, usually a new [engine](#engine).**

We're still in the same mechanic and still pushing the same goal, but there's a new way to progress.

> In the kill-for-gold mechanic, unlocking time-gated research labs is an expansion. We're still trying to get more damage to kill more things, but we have a new way of increasing damage.

## New Mechanic

**Unfolding into an entirely new mechanic.** It:

- **Almost always introduces a new currency.**
- **Almost always introduces a new verb**: killing vs. fishing vs. building.
- **Usually lives in a new tab.** You don't see two mechanics on screen at the same time.
- **Starts from scratch.** If you unfold into farming, you have a tiny farm with one plot. At first it feels like starting a new game.
- **Feeds back.** After some progress, it benefits your other mechanics (or one specific mechanic). You return with fresh energy and progress where you were stuck.

---

## Promise

**Something the player knows is coming: "once you have this, you will get something."**

- A surprise is **not** a promise. Something exciting that happens unexpectedly doesn't count; the player has to know it's coming.
- The player knows the **condition** and the **kind** of reward, not the exact reward.
- Small promises can be simple goals, like a big upgrade the player knows is very strong.
- **The big promises in an unfolding incremental game are [expansions](#expansion) and [new mechanics](#new-mechanic).**
- Promises are the **meta engine** of the game: after playing for a while, the player's main goal is reaching the next promise or promises.

> Tell a kid, "If you count to 100, I'll give you a treat." That's a promise. Whether they count to 100 next time depends on the quality of the treat.

See [promises.md](promises.md).

### Promise Noun

**The word, or the place in the UI, that tells the player what kind of thing a promise holds.**

> "Count to 100 and you get a *treat*. Count to 1,000 and you get a *fun day*." Different noun, different promise.

If you're consistent about what kind of thing sits behind each noun, the player learns it and reacts appropriately. In the UI, the noun is where the promise sits and how it's organized, e.g. a locked tab means a new mechanic.

### Promise Size

The player should learn what a **small, medium, and large** promise is, from its [noun](#promise-noun).

_To define: what sits at each size?_

---

## Curve

**The graph of a timestamped log of every purchase and unlock in a play session.**

A curve can be spaced out (nothing bought, or nothing unlocked, for a long time), dense, or oscillating between fast and slow.

See [curves.md](curves.md).

## Legibility

**The player can understand how things scale.**

_To expand._ An incremental game has to be legible. Chasing a perfect curve with special-case rules makes it illegible (see [curves.md](curves.md#fixing-a-curve)).

## Stale

_To define._ (Used as: "a curve gets too stale: it slows down predictably and nothing happens for a long time.")
