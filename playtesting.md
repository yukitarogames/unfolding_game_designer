# Playtesting

Principles for simulated playtests and what to look for. Terms are defined in [taxonomy.md](taxonomy.md).

A simulated playtest uses a bot that, ideally, simulates a player. It should produce two things:

1. **The [curve](curves.md).**
2. **Repetition counts:** how many times the bot did the same thing.

---

## Repetition

**Repetition is fine.** What matters is whether the reward justifies it. The output should flag repetition that isn't justified by enough reward.

### Automation is one possible fix

Automation is **not necessarily the fix**, but it's one of the possible fixes for repetition that isn't worth its reward.

---

## Automation

Nobody's building clicker games anymore. There's no doing something by hand in the sense of clicking to generate; the player's actions are things like **allocating a resource or buying something**.

So games don't need much automation, because the player isn't supposed to tinker with things very often. You'll still need it sometimes.
