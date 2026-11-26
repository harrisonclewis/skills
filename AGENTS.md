# AGENTS.md

This file is the single source of guidance for coding agents working in this repository. `CLAUDE.md` imports it, so put repository facts here.

## What this repository is

A collection of agent skills for building production web apps, distributed two ways: via `npx skills add harrisonclewis/skills` and as the Claude Code plugin `skills` served by the marketplace in this same repository. It is documentation, with no build, lint or test tooling.

`.claude-plugin/plugin.json` and `.claude-plugin/marketplace.json` define the plugin and its marketplace. Plugin users invoke skills as `/skills:api`, skills-CLI users as `/api`. Skills are discovered from `skills/` automatically, so adding a skill needs no manifest change.

Bump `version` in `plugin.json` in the same commit as any change under `skills/`. `claude plugin update` compares that number and nothing else, so an unbumped change never reaches plugin users. Run `claude plugin validate .` after touching either manifest.

`opencode.json` registers `skills/` so opencode loads the collection while this repository is open.

## Structure

Each skill lives in `skills/<skill-name>/`, with `SKILL.md` as the entry point and supporting `.md` files beside it or under `references/`.

- Frontmatter carries `name` (matching the directory) and `description`.
- Each skill has an `agents/openai.yaml` with `display_name` and `short_description` for Codex.
- A skill's name appears in its directory, its frontmatter `name` and its `display_name`. Renaming means changing all three, then `grep`ing for the old name.
- Each skill's line in `README.md` summarises its `description`. Change both together.
- Skills point to each other by name in backticks (`security`), never by cross-skill relative link, because each skill directory ships on its own.
