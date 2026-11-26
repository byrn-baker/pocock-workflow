---
name: new-project
description: Start a new project repo from this Home Repo, with Spec Kit set up, a short agent instructions file, and a pointer added to the Home Repo's AGENTS.md. Use when the user wants to create, start or scaffold a new project.
---

# New project

Run this from the Home Repo. It creates one project beside it and registers it here.

## 1. Ask, in one message
- Project name (lowercase, hyphens). It becomes the folder and repo name.
- One sentence on what it is for.
- Which agents will work in it: Claude Code, Codex, or both. Default: Claude Code.
- Whether to create a GitHub repo now, and if so, public or private. Default: no repo yet.

Wait for the answers.

## 2. Check before changing anything
- The folder `../<name>` must not exist. If it does, stop and say so.
- `specify --help` must run. If it does not, stop and point to https://github.com/github/spec-kit for installation.
- The Home Repo working tree must be clean, so the pointer change can be committed on its own.

## 3. Create the project
In `../<name>`:
1. `git init -b main`.
2. Run `specify init --here --force --non-interactive --integration claude`. For Codex, run `specify init --here --force --non-interactive --integration codex --integration-options="--skills"`. For both agents, run both commands.
3. Write `README.md`: the name and the one-sentence purpose.
4. Write `AGENTS.md`, no more than 15 lines:
   - What the project is (the sentence).
   - How to start it and run the tests: "not decided yet". Replace this once the first spec is done.
   - Read first: `.specify/memory/constitution.md` and the current spec under `specs/`.
   - Shared standards and skills live in the Home Repo at `../<home folder name>`.
5. Write `CLAUDE.md` containing only `@AGENTS.md`.
6. Commit: "Start <name> with Spec Kit".

## 4. Register it in the Home Repo
Add one line under `## Projects` in this repo's `AGENTS.md`:
`- <name>: <purpose>. Path: ../<name>. Remote: <url, or "none yet">.`
Commit it in the Home Repo.

## 5. GitHub, only if the user said yes in step 1
Run `gh repo create <name> --<public|private> --source ../<name> --push`. Then put the remote URL in the pointer line and commit again.

## 6. Hand over
Tell the user:
- The path, both commits, and the remote (if any).
- To open a fresh session in the new project and run `/setup-matt-pocock-skills` there. The user has to run it; the agent cannot start it.
- The check: in that fresh session, typing `/` lists `grill-with-docs`, `speckit-specify` and `pocock-workflow`. List any that are missing.

Do not start building the project itself. The next step is the user's: `/grill-with-docs` with what they want to make.
