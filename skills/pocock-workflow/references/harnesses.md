# Harness setup

## Install

Copy the whole `pocock-workflow` folder into a folder your agent reads skills from:

- Claude Code: `~/.claude/skills/pocock-workflow` (all projects) or `.claude/skills/pocock-workflow` (one project).
- Codex: `~/.agents/skills/pocock-workflow` or `.agents/skills/pocock-workflow`.

This skill coordinates other skills; it does not install them. Also install:

- Matt Pocock's skills: https://github.com/mattpocock/skills (follow its README, or https://www.aihero.dev/skills).
- GitHub Spec Kit in each project that uses it: https://github.com/github/spec-kit (`specify init --here --integration claude`, or `--integration codex --integration-options="--skills"`).

Install each skill one way only. Two copies of the same skill show up twice.

## Native invocation

- Codex: open the target project and invoke $pocock-workflow.
- Claude Code: open the target project and invoke /pocock-workflow.
- Enjoy: select the target project and underlying Claude Code/Codex agent, then select this skill in its native picker. Plain slash text is not evidence of activation.

Restart existing sessions after installation. Check that a fresh session lists the skill before relying on it. File integrity, native discovery and task behavior are separate results. General Claude web chat is not configured by local setup.

Sources: https://code.claude.com/docs/en/skills ; https://learn.chatgpt.com/docs/build-skills ; https://enjoy.dev/help/conversations/run-a-skill/ . Checked 21 November 2026.
