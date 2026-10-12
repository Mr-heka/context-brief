# Set up Context Brief

You are installing this kit on the user's machine. Paths that don't start with `~` are relative to this repo.

## 1. Install the skill

Copy `skills/context-brief/` to `~/.claude/skills/context-brief/`, replacing an older copy of this same skill if one is there. Create `~/.claude/skills/` if it's missing.

If Codex is installed (`~/.codex` exists), copy the same folder to `~/.codex/skills/context-brief/` as well.

Change nothing else. Installing this kit saves nothing about the user's business; the skill only saves a business brief later, when they ask for it and say yes.

## 2. Check

1. `~/.claude/skills/context-brief/SKILL.md` exists and matches this repo's copy (and the Codex copy, if you made one).
2. Check whether `~/.context-brief/business.md` already exists, without changing it.

## 3. Report

Tell the user, briefly:

- the skill is installed (and where);
- whether they already have a saved business brief;
- next step: start a new session and say "Let me brief you". If they want to talk instead of type, the Wispr Flow setup is in `skills/context-brief/references/wispr-flow.md`.

## Removing

Delete `~/.claude/skills/context-brief/` (and `~/.codex/skills/context-brief/` if present). A saved business brief stays in `~/.context-brief/` until the user deletes it.
