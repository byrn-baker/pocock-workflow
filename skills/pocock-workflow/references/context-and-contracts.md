# Context and task contracts

## Manage the working set

Keep durable requirements, glossary terms, ADRs, commands, and task status in their authoritative project records. Load the files needed for the current decision. Repository navigability matters more than raw size. Do not use the interview's approximately 150,000-token comfort point as a universal threshold or hard reset trigger.

Start with normal effort for bounded exploration. Escalate when a demonstrated reasoning problem, difficult diagnosis, or consequential verification merits it. Effort labels differ across providers. Diagnose missing evidence, unavailable tools, and unclear requirements before switching models.

Checkpoint at a phase boundary, before a provider/host handoff, or when accumulated exploration obscures the task. Preserve consequential decisions before compaction. After resuming, inspect actual state; a summary is not proof that files or external systems remain unchanged.

## Task contract for a delegate

Supply the following, using the existing project task format:

- Goal, non-goals, specification/plan/task references, and relevant ADRs.
- Host/OS, repository, working directory, branch or base revision, and existing edits to preserve.
- Applicable repository instructions and the selected skill instructions. Supply reachable copies or excerpts with source/version when the worker cannot access the original; a name alone is insufficient.
- Owned files or module boundaries, dependencies, shared-resource owner, and allowed actions.
- Acceptance scenarios, commands or observation methods, expected results, and evidence location.
- Attempt cap, attempts already consumed, stop conditions, and required final report.

Before launching, verify the worker's environment, skill access, runner, and agent launch path on the actual OS. Worktrees separate changes; they are not credential, process, or network sandboxes. Parallelize independent work; sequence coupled edits. One coordinator owns final integration and acceptance.

Completion criterion: the worker can locate the task and instructions, state its bounded ownership, and run the agreed checks. If these prerequisites fail, report the specific gap before unattended mutation.

## Handoff template

Goal and authoritative task:
Accepted decisions and non-goals:
Current host/repository/revision and changed files:
Running processes, active workers, pending external actions:
Checks run, tested revision, observed results, evidence paths:
Known failures and remaining work:
Attempts consumed and remaining cap:
Authorization already granted and decisions still needed:
Next unblocked action:

Include just enough source evidence to verify the summary. Before retrying a timed-out write, determine whether it already succeeded. Stop duplicate writers and reconcile ownership before continuing.

## Independent completion review

Compare the full result with both the specification and standards. Check normal and meaningful failure behavior through the actual interface. Assess irreversible effects and blast radius separately from Git reversibility. Confirm integrated checks after combining worker results. An agent's confidence, an idle pane, or a worker's green test report alone does not establish task completion.

Return changed artifacts, observed evidence, unresolved risks, and the next action. A retrospective should propose a small durable improvement grounded in a demonstrated failure, preferably a deterministic check or better interface where practical.
