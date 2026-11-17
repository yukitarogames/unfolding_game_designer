# Using this repository

This repository holds principles for unfolding incremental games. When you design one, you **orchestrate**; you don't design or judge it yourself.

Two subagents do the work, each in a fresh context:

- **`designer`** drafts and revises designs. It reads only `taxonomy.md` and the user's brief.
- **`judge`** reviews designs against every file in this repository and returns `PASS` or `REVISE` with findings.

If `designer` and `judge` aren't available as agent types (for example, when this repository was attached to a session rather than opened as its root), spawn general-purpose subagents instead. Tell each one to read and follow `.claude/agents/designer.md` or `.claude/agents/judge.md` in this repository, ignoring the frontmatter.

## The loop

Use it for every new design and every design change, before writing code for it.

1. Give `designer` the user's brief, verbatim, and the absolute path of this repository.
2. Give `judge` the design, verbatim, and the absolute path of this repository. Nothing else: no summary, no context about how the design was made.
3. If the verdict is `REVISE`, give `designer` its previous design and all of the judge's findings, verbatim, and go back to step 2.
4. Stop when the verdict is `PASS`, or after three rounds.
5. Show the user the final design and the last verdict and findings, including any the designer disagreed with.

## Rules

- **Don't edit the design yourself.** Changes go through `designer`.
- **Don't filter or soften the judge's findings.** Pass them on in full.
- **Don't skip the judge**, even for small changes.
- Playtest results (curves, repetition counts) also go to `judge`, together with the current design.
