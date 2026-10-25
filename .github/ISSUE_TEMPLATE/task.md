---
name: Task / Change
about: Everything an agent or a human needs to do the work without asking anyone
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

<!--
This template IS the brief. It is read by an autonomous agent that cannot ask you anything, and by a
human who needs to know months later what happened and why. Fill every section.

If you do not know something, write UNKNOWN and say why. Never invent a file path, a command or a
check - a wrong detail is worse than a missing one.

Source of truth: the codebase. If this issue and the code disagree, the code is right. Correct the
issue, do not change the code to match the ticket.
-->

## Request (verbatim)

<!-- Paste the words that actually asked for this: the user message, the chat line, the alert text.
Do not paraphrase - the original words carry intent a summary loses. If it came from an incident,
paste the alert. If from a conversation, quote it and give the session or message id. -->

## Why this matters

<!-- The problem, who it affects, and what happens if it is not done. One short paragraph. This is what
lets an agent make a sensible judgement when the instructions run out. -->

## Done when (the check, not the goal)

<!-- A command, a URL, a file path or a test a stranger can run to see it is finished, plus what output
means success. "Works better" is not a check. Example:
    `pytest tests/test_alerts.py -k dedupe` exits 0, and the duplicate card no longer sends.
An agent that cannot verify its own work cannot honestly claim it is done. -->

## Where to work

- **Repo:** <!-- owner/name, or "none - ops task" -->
- **Branch:** <!-- agent/<issue-id> unless told otherwise -->
- **Directory / machine:** <!-- absolute path on the machine that will run it -->
- **Files that matter:** <!-- the 1-5 paths already known to be involved, or UNKNOWN -->
- **Read first:** <!-- related commits, docs, prior tickets, one specific file -->
- **Pattern to copy:** <!-- an existing example in the codebase that already does this well -->

## Constraints

<!-- What must not change and what is out of bounds, stated specifically: "do not touch the broker
adapter", "no new dependencies", "keep current behaviour when X". An agent with no boundaries will
helpfully refactor something you needed left alone. -->

## Out of scope

<!-- Related work deliberately not part of this, so the diff stays reviewable. -->

## Risk / sensitivity

- **Blast radius:** <!-- Low / Medium / High - what breaks if this is wrong -->
- **Touches:** <!-- secrets, auth, money, live trading, data schema, other systems - or "none" -->
- **Rollback:** <!-- how to undo it, or say that it is irreversible -->

## Approach, if you have one

<!-- Optional. If you already know how it should be done, say it and say why. If not, write
"open - agent's judgement". A suggested approach is guidance, not a cage: if it turns out not to work,
say so rather than forcing it. -->

## When you are stuck

<!-- Default behaviour: if the check cannot be met, if this ticket contradicts the codebase, or if the
work needs a decision only the owner can make, stop, comment what you found, and set this issue to
Blocked. Do not guess, do not widen the scope. Change this line only if you want different behaviour. -->

## Provenance

- **Asked by:** <!-- human name, or the agent that created this -->
- **When:** <!-- date and time, PT -->
- **From:** <!-- session id, chat, alert, or the ticket this was split from -->
- **Prior work:** <!-- commits or issues that already touched this, from the repo history -->
