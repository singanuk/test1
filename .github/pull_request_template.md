<!--
PR title: an imperative sentence ("Add X", not "Added X" / "Adding X") — matches the
commit convention and keeps history searchable. Vague titles ("Fix bug", "Update docs")
make a change unfindable months from now (Google eng-practices CL-description guidance).
-->

## Intent

<!-- The problem being solved and why this is the right approach — not just what changed.
One or two sentences. Link the issue (Closes #NNN) rather than restating its content. -->

## What changed

<!-- Bullet list: files/behavior touched. A reviewer should get the shape of the diff
without opening it. When bullets do not make the key point clear, add one compact
diagram, call tree, file tree, or diff sketch showing the relevant flow, ownership,
or change shape. Keep it focused and omit it when it adds no clarity. -->

## Risk assessment

- **Blast radius:** Low / Medium / High — affected consumers or surfaces if this is wrong
- **Merge door:** Two-way / One-way / Mixed / Uncertain — why
- **Failure modes:** <!-- concrete ways this could break — not "nothing should break" -->
- **Rollback:** <!-- concrete revert, migration rollback, or containment/recovery path; note any irreversible state -->

## Pipeline (issue -> plan -> implementation -> review -> merge)

- **Issue:** Closes #NNN
- **Plan:** <!-- link, or "none — small/mechanical change" per AGENTS.md rule 1 -->
- **Worktree/branch:** <!-- branch name; worktree path if one was used -->
- **Authoring agent/toolchain:** <!-- local toolchain / human / mixed -->
- [ ] Fresh Sol adversarial review run by a **fresh `major_reviewer_sol` instance** pinned to `gpt-5.6-sol`/`xhigh` — no unresolved P0/P1
- [ ] Security-focused review run (only if this PR touches secrets, auth, or LLM I/O) — no unresolved P0/P1

## Testing

<!-- Commands run + actual pasted output. "Should pass" is not evidence — every claim
here must be something you just verified, not something you expect to be true.
Pair a representative before/baseline state with the verified after state when
meaningful. Screenshots, command output, and test results are valid evidence.
If no meaningful before state exists, say why; never invent a failing test or imply
an unrun check passed. -->

- **Before / baseline:** <!-- screenshot, output, failing test, or "not applicable — explain why" -->
- **After / verified result:** <!-- screenshot, output, passing test result -->
