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
4. Give `designer` earlier drafts or old designs only when the user asks. Label them as material it may use or ignore, not as a starting point. (This is about material from before this loop. Versions made during the loop are handled under **Versions**.)

The current game is the first **best so far**. Then continue with the loop from step 2.

## Versions

Keep every version of the design as a numbered file next to the game, together with the judge's verdict and findings on it. Never overwrite a version.

- **Best so far** is the version currently designated the strongest. It starts as the first draft, or as the current game when starting from one.
- Every new version is a **candidate**. Being newer, or answering the judge's findings, doesn't make it best so far. Only `designer` moves best so far, by comparing the two versions (see `.claude/agents/designer.md`).
- A candidate may revise best so far, revise the latest candidate, or start fresh from the brief. Exploratory candidates may come out worse than best so far. That's fine; they just don't replace it.
- The designer's revision notes and comparisons are for the user's report. Don't give them to `judge`.

## The loop

1. Give `designer` the user's brief, verbatim, and the absolute path of this repository.
2. Give `judge` the latest candidate's design and the user's brief, both verbatim, and the absolute path of this repository. Nothing else: no summary, no revision notes, no context about how the design was made.
   From round 2 on, also give `judge` the designer's list of findings it chose to override, with its reasons, and nothing else about how the design was made.
3. If the verdict is `REVISE`, give `designer`, verbatim and labelled: the latest candidate with all of the judge's findings on it, and best so far with its findings if it's a different version. The designer picks best so far, then writes a new candidate. Go back to step 2.
4. If the verdict is `PASS`:
   - If the passed candidate is best so far (e.g. a first draft), it goes ahead.
   - Otherwise, give `designer` both versions with their findings, verbatim and labelled. It either adopts the passed candidate, which goes ahead, or keeps best so far and writes a new candidate. In that case, go back to step 2.
5. **After three rounds without a `PASS`, `designer` decides:** ask for another round, or go ahead with best so far despite the judge's remaining findings. If it goes ahead, it states which findings it's overriding and why. If it asks for another round, repeat from step 2, and the designer decides again after each later round.
6. **Hard cap: seven rounds.** After round seven, the designer must go ahead with best so far, the strongest version that satisfies the brief, listing the findings it's overriding and why.

A round is one review by `judge`. The loop always ends with a decision and a design to build. Never stop without one. The version that goes ahead is never assumed to be the latest one.

## Playtesting

Every design that goes ahead gets built and playtested:

1. Build it and run the bot (curve and repetition counts). The built version is now best so far.
2. Give `judge` the current design, the playtest output, and the user's brief, verbatim.
3. If the judge finds problems, the fix is a design change: it goes through the loop, as a candidate against the built version.
4. If the new build replaces something the user can already play (the current game, or an earlier build), keep that build playable next to the new one, so the user can compare them.

## Done

You're done when there's a **new playable version for the user to playtest**, and either the judge passed both the design and the latest playtest, or the designer decided to go ahead despite the judge.

Push it, then show the user:

- the final design,
- the judge's last verdict and findings, in full,
- any findings the designer overrode, and why,
- the version history: which version went ahead, and each time best so far changed or was kept, the designer's comparison,
- where to play the previous build, if one was kept.

## Rules

- **Don't edit the design yourself.** Changes go through `designer`.
- **Don't filter or soften the judge's findings.** Pass them on in full.
- **Don't skip the judge**, even for small changes or balancing.
- **The brief sets the scope.** The judge lists problems outside the brief separately, as **out of scope**. Report those to the user; don't pass them to the designer.
- **Don't be your own judge.** "Happy with it" means the judge passed it, or the designer explicitly decided to go ahead.
