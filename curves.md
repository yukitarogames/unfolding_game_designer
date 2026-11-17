# Curves

Reading and balancing curves. Terms are defined in [taxonomy.md](taxonomy.md).

---

## Reading a curve

When balancing a game, look at the curve and ask: **Do I like this curve? Is this a good curve?**

## Don't optimize for the curve

What makes a good curve is very tricky. You almost never fine-tune numbers to get a specific curve shape, because a precise shape is not important. **The general outline is what matters, and the curve tells you where you have a problem.**

## Runaway curves

A curve can fail by going too fast as well as too slow. When progress cascades and the player passes several promises at once, those promises lose their value. A common cause is a connection between mechanics that pays out too much (see [unfolding.md](unfolding.md#too-much-is-also-a-failure)).

## Fixing a curve

When the curve shows a problem, fix it in one of two ways:

### 1. Change a constant

Adjust an existing scaling value rather than adding a rule.

### 2. Unfold

Introduce a new mechanic or an expansion of an existing mechanic.

When a curve gets [stale](taxonomy.md#stale), **the curve needs to break with an unfolding**. What pushes the player through the slowing progress is a [promise](promises.md) they're pushing towards.

### Don't: add special-case rules

Don't introduce lots of new rules to fix the curve. Incremental games have to be **legible**. If you chase a perfect curve, you'll make an illegible game where the player doesn't understand how things scale.

This is about patching the curve, not about a mechanic's own rules. Rules that interact are what make a mechanic worth playing (see [fun.md](fun.md)).

---

## The early game

The beginning needs more density of progress: more buying things and getting more powerful. You don't have to go crazy. You keep the player busy and happy by giving them power.

- **Too slow loses the player.** If they act and then nothing happens for a long time, you lose them.
- **Too fast also fails.** If the player just clicks and progresses really fast, you've failed too.

**The real job of the early game is to teach the shape of the game's promises**, the language of the game. The player should learn the game's promise sizes, know when each is unlocked, and experience each one.

---

## Retention

Once the player understands the promises and sees the next promise and when they'll reach it, they have a goal to work towards. You get retention when:

- the goal is **reasonably within reach** (not obscenely far away), and
- the first time that kind of promise was fulfilled, it was a **significant boost in power, interest, and fun**.
