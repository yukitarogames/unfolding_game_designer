# Using this repository

This repository holds principles for unfolding incremental games. When you design one, you **orchestrate**; you don't design or judge it yourself.

Two subagents do the work, each in a fresh context:

- **`designer`** drafts and revises designs. It reads only `taxonomy.md` and what you give it.
- **`judge`** reviews designs, games, and playtest results against every file in this repository and returns `PASS` or `REVISE` with blocking findings and non-blocking notes.

If `designer` and `judge` aren't available as agent types (for example, when this repository was attached to a session rather than opened as its root), spawn general-purpose subagents instead. Tell each one to read and follow `.claude/agents/designer.md` or `.claude/agents/judge.md` in this repository, ignoring the frontmatter.

## When to use the loop

Always, before writing code for:

- a new design,
- any design change, however small,
- an overhaul of an existing game,
- any request to apply these principles to a game, even when it's phrased as "read the repo and use it".

Don't design or rebalance directly from your own reading of the principles.

## Starting from an existing game

Diagnose before redesigning:

1. Give `judge` the current game as plain facts: what the player does and sees, its rules and numbers (from the code), a bot playtest run (curve and repetition counts), and the user's brief. Nothing else.
2. Give `designer` the same plain facts, the judge's findings, and the user's brief, all verbatim.
3. Don't give either one an old design write-up that cites this repository. Describe the game, not how it relates to the principles.

Then continue with the loop from step 2.

## The loop

1. Give `designer` the user's brief, verbatim, and the absolute path of this repository.
2. Give `judge` the design and the user's brief, both verbatim, and the absolute path of this repository. Nothing else: no summary, no context about how the design was made.
3. If the verdict is `REVISE`, give `designer` its previous design and all of the judge's findings, verbatim, and go back to step 2.
4. If the verdict is `PASS`, the design goes ahead.
5. **After three rounds without a `PASS`, `designer` decides:** ask for another round, or go ahead despite the judge's remaining findings. If it goes ahead, it states which findings it's overriding and why. If it asks for another round, repeat from step 2, and the designer decides again after each later round.

The loop always ends with a decision and a design to build. Never stop without one.

## Playtesting

Every design that goes ahead gets built and playtested:

1. Build it and run the bot (curve and repetition counts).
2. Give `judge` the current design, the playtest output, and the user's brief, verbatim.
3. If the judge finds problems, the fix is a design change: it goes through the loop.

## Done

You're done when there's a **new playable version for the user to playtest**, and either the judge passed both the design and the latest playtest, or the designer decided to go ahead despite the judge.

Push it, then show the user:

- the final design,
- the judge's last verdict and findings, in full,
- any findings the designer overrode, and why.

## Rules

- **Don't edit the design yourself.** Changes go through `designer`.
- **Don't filter or soften the judge's findings.** Pass them on in full.
- **Don't skip the judge**, even for small changes or balancing.
- **Don't be your own judge.** "Happy with it" means the judge passed it, or the designer explicitly decided to go ahead.
