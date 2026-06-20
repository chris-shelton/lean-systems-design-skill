# Simplify Then Ship

[![skills.sh](https://skills.sh/b/chris-shelton/simplify-then-ship-skill)](https://skills.sh/chris-shelton/simplify-then-ship-skill)

An agent skill for cutting through messy work and shipping the smallest useful result.

It applies a first-principles execution loop:

1. Challenge requirements.
2. Delete parts.
3. Simplify what remains.
4. Accelerate feedback.
5. Automate last.

Use it for implementation, code, architecture, product/design decisions, process improvement, research workflows, and technical objectives that feel overcomplicated, slow, brittle, approval-heavy, or prematurely automated.

## Install

With the Vercel `skills` CLI:

```bash
npx skills add chris-shelton/simplify-then-ship-skill
```

Install globally for Codex:

```bash
npx skills add chris-shelton/simplify-then-ship-skill -g -a codex
```

Use without installing:

```bash
npx skills use chris-shelton/simplify-then-ship-skill --skill simplify-then-ship
```

## Example Prompts

```text
Use simplify-then-ship to work through this implementation before we add another abstraction.
```

```text
Review this process and tell me what to delete before we automate it.
```

```text
Help me narrow this research plan to the fastest test of the riskiest assumption.
```

## Skill Format

This repo follows the open Agent Skills format:

```text
simplify-then-ship-skill/
|-- SKILL.md
|-- README.md
`-- LICENSE
```

`SKILL.md` contains the required YAML frontmatter:

- `name`
- `description`

The skill is intentionally small. It has no scripts, references, assets, or runtime dependencies.

## Publishing Notes

As of June 20, 2026, the active public directory is [skills.sh](https://skills.sh), not the singular `skill.sh` domain. `skills.sh` is powered by Vercel's open-source `skills` CLI.

To publish/list this skill:

1. Keep this repository public on GitHub.
2. Keep `SKILL.md` at the repository root or under a supported skill directory.
3. Ensure the frontmatter is valid. This repo exposes one skill named `simplify-then-ship`.
4. Install it once with `npx skills add chris-shelton/simplify-then-ship-skill`.

`skills.sh` lists repositories automatically through anonymous CLI install telemetry. A root `skills.sh.json` file is optional and only changes how multi-skill repository pages are grouped, so this single-skill repo does not need one.

## License

MIT. See [LICENSE](LICENSE).

## Author

Chris Shelton.
