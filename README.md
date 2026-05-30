# Skills

My agent skills for real engineering work. Small, composable, and model-agnostic. Hack them, adapt them, make them your own.

## Quickstart

Install with the [skills.sh](https://skills.sh) CLI:

```
npx skills@latest add knowbody/skills
```

Pick the skills you want and the coding agents to install them on.

Prefer native Claude Code plugins? Point a marketplace at this repo and install it as the `matt-skills` plugin.

## Reference

### Engineering

Skills for daily code work.

- **[roast-me](./skills/engineering/roast-me/SKILL.md)**: Adversarially review finished code, hunting for bugs and weaknesses instead of reassuring you. Reports each finding with an exact location, why it's wrong, and a concrete fix, tagged Critical / Worth fixing / Nit.

## Adding more skills

See [`CLAUDE.md`](./CLAUDE.md) for the repo conventions. In short: drop a new `skills/<bucket>/<name>/SKILL.md`, register it in `.claude-plugin/plugin.json`, and add a linked reference here and in the bucket README.
