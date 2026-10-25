---
name: Feature
about: New capability, multi-step work, or anything with a design decision in it
title: ""
labels: []
---

<!--
MINIMUM BAR - every issue, however small, must answer these. A two-line ticket is fine if it does.

  1. What is wrong or wanted        (the request, in the owner's words where you have them)
  2. Where                          (repo, path, machine, or "none - ops task")
  3. How we know it is finished     (a command, URL or observation, not a feeling)
  4. Who asked                      (human name, or the agent that raised it)

Scale the rest to the size of the change. A typo fix does not need a rollout plan; a feature that
touches live trading does. When in doubt, write more - silence is what costs an agent a wasted run.

The codebase is the source of truth. If this issue and the code disagree, the code is right.
-->

## Request (verbatim)

<!-- The words that asked for this, quoted. Session id or link if it came from a chat. -->

## Why this matters

<!-- The problem, who has it, what it costs today, and what changes if this exists. This is the section
that lets someone re-derive the design two years from now. -->

## What "good" looks like

<!-- Concrete: the user-visible behaviour after this ships. One or two sentences, plus the failure modes
that would make it a bad release. -->

## Design intent

<!-- How you expect it to work, and why that shape rather than the obvious alternative. If you already
ruled options out, say which and why - that is the most expensive knowledge to rediscover. -->

## Alternatives considered

<!-- Optional but valuable: the other approach, and the reason it lost. Write "none" if genuinely none. -->

## Done when

<!-- The check a stranger runs. Include the regression risk: what must still work afterwards. -->

## Where to work

- **Repo / branch:**
- **Directory or machine:**
- **Files that matter:**
- **Pattern to copy:**

## Constraints and out of scope

<!-- What must not change; what is deliberately not part of this. -->

## Risk, blast radius, rollback

- **Blast radius:** Low / Medium / High
- **Touches:** secrets, auth, money, live trading, data schema - or none
- **Rollback:**

## Plan

<!-- Link the written plan, or say "none needed - small/mechanical". Multi-step work should have one. -->

## Open questions

<!-- Anything still undecided, and who decides. Write "none" once they are settled. -->

## Provenance

- **Asked by:**
- **When (PT):**
- **From:**
- **Prior work:**
