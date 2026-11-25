# pocock-workflow

An agent skill that combines [Matt Pocock's engineering skills](https://github.com/mattpocock/skills) with [GitHub Spec Kit](https://github.com/github/spec-kit) in one workflow:

- Spec Kit keeps the project records: constitution, spec, plan and tasks.
- Matt's skills do the engineering inside them: `grill-with-docs` to clarify, `tdd` to build, `code-review` against the spec, and `retro` afterwards.
- Implementation runs in bounded loops, with a default cap of 10 attempts per task.

This is my own skill. It is not part of Matt Pocock's package, and the interview it draws on does not prescribe Spec Kit. That combination is my choice.

## Install

1. Install Matt Pocock's skills: https://github.com/mattpocock/skills (or see https://www.aihero.dev/skills).
2. Install Spec Kit (`uv tool install specify-cli`), then, in your project, run `specify init --here --integration claude`. For Codex, run `specify init --here --integration codex --integration-options="--skills"`.
3. Copy `skills/pocock-workflow` into `~/.claude/skills/` (Claude Code) or `~/.agents/skills/` (Codex).
4. In a fresh session, type `/pocock-workflow` (Claude Code) or `$pocock-workflow` (Codex) and check that it is listed.

The skill runs with your agent's full permissions. Read it before you use it.

## Credits

- NetworkChuck and Matt Pocock, ["How to Actually Code with AI"](https://www.youtube.com/watch?v=mU8WKII1gpk)
- Matt Pocock's skills: https://github.com/mattpocock/skills and https://www.aihero.dev/skills
- GitHub Spec Kit: https://github.com/github/spec-kit
