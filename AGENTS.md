# AGENTS.md

## Start here

The durable handoff for this repository is **`research/next_agent_handoff.md`**. Read it first, then
`research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`.

The mission is defined by the canonical prompt, which is maintainer-owned and must not be edited:
`research_prompts/systematic_edge_discovery_agent_prompt.txt`.

## Absolute scope boundary

This is a **theory-only hypothesis-generation and research-prioritisation** environment.

Not allowed here: backtests, simulations, parameter sweeps, optimisation, significance testing on
strategy results, performance or risk metrics, market-data acquisition or processing, strategy or
signal implementation, executable research infrastructure, job or workflow launches, changes to
workflow files, tests, credentials or infrastructure, work in other repositories, and any trading.

Allowed: reading and summarising literature, market-structure and venue documentation, exchange and
regulator material, and the repository's own notes; specifying hypotheses, falsifiable predictions,
observables and data requirements; maintaining the theory-only artifacts below.

If a question can only be answered by running something, write the question down precisely and hand
it off. That is the correct output, not a failure.

## Artifacts to maintain

- `research/next_agent_handoff.md` — the durable handoff; rewrite it at the end of every session.
- `research/idea_register.md` — one complete dossier per retained candidate.
- `research/ranked_shortlist.md` — rubric-scored ranking with hard-stop flags.
- `research/source_ledger.md` — verified citations only, with how each was verified.
- `research/validation_handoffs.md` — validation *specifications* (never executed here).
- `research/rejected_and_parked.md` — rejections, parkings, and the known-baseline reference set.
- `research/cycle_notes.md` — cycle log, the three-pass task-framing loop, artifact history.

ID sequences in use: `IDEA-001…004`, `S-001…028`, `V-001…003`, `R-001…003`, `P-001…004`,
`G-01…05`, `Cycle 1`. Continue each series rather than restarting it.

## Working rules

1. Read the handoff and the register before generating anything; preserve prior work.
2. Never invent a citation. Every external claim points to a source-ledger entry.
3. Score with the fixed rubric as research priority, never as a probability of profit.
4. Leave the session with an updated handoff and a fresh, self-contained initial task message for
   the next agent.
