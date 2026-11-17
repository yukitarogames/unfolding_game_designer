# Playtesting

Principles for simulated playtests and what to look for. Terms are defined in [taxonomy.md](taxonomy.md).

A simulated playtest uses a bot that, ideally, simulates a player. It should produce:

1. **The [curve](curves.md), for the whole game and for each mechanic.** A new mechanic is a game with its own curve.
2. **Promises on the curve,** marked by size, so the gaps between promises of each size are visible.
3. **Repetition counts:** how many times the bot did the same thing.
4. **The decision gap:** how much better a bot that plays well does than a bot that always buys the cheapest thing, for each mechanic.

---

## The decision gap

This is the playtest's measure of [whether the verb has decisions in it](fun.md#the-verb-has-decisions-in-it).

- **A small gap means the choices aren't real.** Thinking doesn't pay, so the mechanic is boring however good its curve looks.
- **Look at it per mechanic.** One mechanic with real decisions doesn't make up for another without them.

---

## Repetition

**Repetition is fine.** What matters is whether the reward justifies it. The output should flag repetition that isn't justified by enough reward.

### Automation is one possible fix

Automation is **not necessarily the fix**, but it's one of the possible fixes for repetition that isn't worth its reward.

---

## Automation

Nobody's building clicker games anymore. There's no doing something by hand in the sense of clicking to generate; the player's actions are things like **allocating a resource or buying something**.

So games don't need much automation, because the player isn't supposed to tinker with things very often. You'll still need it sometimes.
