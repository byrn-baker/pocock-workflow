# Spec Kit integration

Use Spec Kit for project process and the relevant installed Matt Pocock skills for engineering execution. This division is the user's chosen workflow; the interview does not prescribe Spec Kit.

## Preflight and authority

Inspect the actual repository instructions, working tree, existing .specify configuration, generated agent commands or skills, and current spec, plan, tasks, and acceptance evidence. Record which artifact governs the task. Existing artifact paths and IDs win over any examples here.

Check the installed tool's version/help and repository integration before choosing commands. A directory named .specify or a specification file alone does not prove that tooling is installed. If setup is missing, consult the official installation and integration documentation at https://github.com/github/spec-kit and establish the supported route appropriate to the target OS. Preserve existing project material. Do not reinitialize over it or invent slash commands.

Completion criterion: the repository, applicable instructions, active artifact, available integration, and next process stage are identified; missing requirements are explicit.

## Feature route

1. Clarify intent with repository evidence first. Use grilling and domain-modeling guidance where relevant. Record domain terms and consequential decisions in the existing glossary and ADR structure.
2. Capture user behavior, non-goals, failure behavior, and measurable acceptance in the authoritative specification. Use the installed Spec Kit specification/clarification process; an approved existing specification can be reused.
3. Plan module boundaries, dependencies, and verification. Apply codebase-design guidance. If a natural implementation needs a broader refactor, explain it and stop before performing that refactor.
4. Divide into independently checkable tasks linked to the specification. Preserve dependency order. If upstream to-spec or to-tickets guidance expects a tracker, adapt the output to the established Spec Kit records; publish tracker items only within authorization.
5. Implement the next unblocked task with its acceptance checks and cumulative attempt budget. Apply relevant implementation/TDD guidance without writing tests that merely duplicate the implementation.
6. Review against a fixed base, standards, and the originating specification. After integrating delegated changes, validate the combined result. Record remaining uncertainty and release consequences.

Completion criterion: acceptance evidence covers the requested behavior on the actual result, the full diff has been reviewed, and the authoritative task status matches reality.

## Bug route

Use scoped diagnosis and verification in the project's existing task record. Read diagnosing-bugs; reproduce the symptom, distinguish competing explanations, isolate the cause, repair it, and rerun the original reproduction plus relevant regression checks. Keep documentation proportional. A bug repair does not automatically require a new feature specification.

For performance claims, compare the same workload and conditions. For unavailable live environments, state what fixture or local evidence proves and what remains unverified.

## Loop record

Before attempt 1, set the cap (default 10 total per task). For a resumed task, recover attempts already used. If the count cannot be established, record that uncertainty and resolve the remaining budget before unattended execution; do not reset it silently.

For each attempt record: task ID, attempt number and cap, starting revision/state, hypothesis or intended change, meaningful checks and observed outcomes, full-diff findings, next correction or stop reason. Use the existing task log or evidence location; do not create a parallel task system.

Stop on passing checks and completed review, missing required input/authorization, or cap exhaustion. Keep assertions and checks intact. Record a newly discovered requirement instead of expanding scope to make the current attempt pass.

## Delivery

For PR writing, read the installed PR skill. Explain the concrete behavior change, evidence, and merge consequences. Committing, pushing, merging, deploying, and external communication retain their existing authorization requirements. A merge-triggered deployment is a release action. Routine repeatable checks and releases should use verified scripts or CI rather than improvised agent steps.
