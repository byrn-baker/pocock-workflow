---
name: pocock-workflow
description: Coordinate Spec Kit coding work with Matt Pocock's engineering skills, bounded implementation loops, and context handoffs across Claude Code, Codex and Enjoy. Use for starting or resuming project work and cross-harness delegation, not general conversation or document editing.
---

# Pocock workflow

Start at the decision the user actually faces. Inspect the working directory, its instructions, and any existing spec, tickets, glossary or prior acceptance evidence. An approved ticket can go straight to implementation. For the upstream procedure behind any route, locate the matching official SKILL.md using [the skill index](references/skills.md) and read it before using it. The index includes experimental and specialist tools.

This is a user-owned coordinating skill, not the official Matt Pocock package or a Spec Kit installer. Current user instructions and repository rules govern its use. Keep the existing model unless the task or user calls for a change. Load only the references for the active branch:
- **New or resumed coding work:** read [Spec Kit integration](references/spec-kit.md) before implementation.
- **Provider change, remote worker, long context, or delegated task:** read [context and task contracts](references/context-and-contracts.md).
- **Task completion, review feedback, or repeated failures:** read [continuous improvement](references/continuous-improvement.md); explicit Retro invocation is separate from installation.
- **Installing, invoking, or troubleshooting the skill in a harness:** read [harness setup](references/harnesses.md).

When a required engineering skill or Spec Kit integration is missing, identify the gap and establish its supported integration within the authorized scope. Continue independent inspection or diagnosis; do not silently replace the required process or claim it is configured. Prefer the installed official mattpocock/skills package over duplicate copies. If a skill is explicit-only, invoke it through a supported user-directed mechanism or explain the needed invocation rather than claiming it ran.

## Work across repositories

Start the session in the Home Repo when the project has one. Follow its AGENTS.md pointer for the capability you need. Verify the target checkout, branch and local instructions before acting there. Keep shared skills, tooling and cross-repo knowledge in the home. Put commands, constraints and vocabulary that apply to one project close to that project.

When asked to establish a home, inventory the repos in scope, their remotes, shared material and conflicting copies. Agree on membership, personal or team ownership, visibility and checkout locations. Show the proposed moves and the treatment of each conflicting copy before migrating. Keep secrets in place. Give each pointer a purpose and a checkout location. Test the result from a fresh session in the home by following a pointer into a member repo and locating its authoritative instructions.

For a cross-repo feature, trace one observable behavior across the boundary. Record which repo owns the contract, which consumes it, and what check exercises both. For example, a changed payment response needs a storefront check that consumes the new response. Report each checkout and the integrated result.

## Choose the next step

- **Small, understood change.** Use the existing task and the cheapest check that can catch a wrong result. A tiny, reversible diff can skip a design interview.
- **Unclear intent.** Use grill-with-docs in a project or grill-me for a standalone conversation. Investigate facts yourself. Bring the user decisions in dependency order with your recommendation. Record settled domain terms in the existing glossary and consequential trade-offs in an ADR. If one decision needs runnable evidence, hand it to prototype and bring the result back. If the decision tree outgrows a session, use wayfinder to map open questions and their dependencies.
- **Agreed feature.** Use to-spec to capture intent and observable acceptance criteria. Use to-tickets for independently checkable vertical slices. List blockers explicitly. In a Spec Kit project use the existing spec, plan and task IDs as the authoritative records. Put each slice and its acceptance check there. Publishing tracker items is a separate action subject to the user's scope.
- **Failure or regression.** Use diagnosing-bugs to reproduce the symptom, narrow the cause with a discriminating experiment and repeat the original reproduction after the fix. For a performance claim, compare the same workload before and after.
- **Implementation.** Choose an unblocked slice. For TDD, drive one behavior through a public interface, see it fail, make it pass, then refactor on green. For tangled internals, use codebase-design to look for a small interface that hides substantial complexity. If the change needs a broader refactor, surface that decision before editing.
- **Review and delivery.** Use code-review against a fixed base. Compare the diff separately with repository standards and the originating spec. Exercise the normal entry point. Use pr to present what changed, what demonstrates it and the remaining merge risk. For visual behavior, include observed screenshots or recordings when appropriate. Use retro when repeated friction points to a specific improvement.
- **Continuation.** Hand off at a phase boundary. Give the next session the authoritative task, decisions, files, reproduction or acceptance command, observed results and next unblocked action.

## Apply the user's execution rules

Use the project's Spec Kit process and the installed Matt skills together. Keep documentation proportional. For authorized implementation or repair, set the cumulative attempt cap before starting (default 10 here). Record each attempt, command, result and diff findings. Stop on verified success, a real blocker or the cap. Keep human judgment in the loop where acceptance is subjective. Before an unattended run, verify the runner, isolation and agent launch on the target OS. Retain existing delegation and external-action boundaries.

Carry the attempt count across sessions and agents. Keep acceptance checks and authorization intact when repairing failures. Once checks pass and the full diff is reviewed, stop the loop; a cap is a maximum, not a target. When work is delegated to another agent or model, the coordinating agent keeps independent verification, complete diff review and final integration; the delegate's own tests do not authorize integration or publication.

Finish with the result, authoritative task references, tested revision and observed evidence, unresolved gaps, and next action. Distinguish implemented, tested, merged, deployed, and verified-live states. Use risk and reversibility to choose review depth; preserve already-granted authorization without repeatedly asking for it. A useful retrospective turns one demonstrated recurring failure into a check, clearer interface, or focused instruction.

For attribution, the specific posts behind these choices, and the limits of the timeline review, see [source notes](references/sources.md).
