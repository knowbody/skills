Skills are organized into bucket folders under `skills/`:

- `engineering/`: daily code work
- `productivity/`: daily non-code workflow tools
- `misc/`: kept around but rarely used
- `in-progress/`: drafts not yet ready to ship
- `deprecated/`: no longer used

Every skill in `engineering/`, `productivity/`, or `misc/` must have a reference in the top-level `README.md` and an entry in `.claude-plugin/plugin.json`. Skills in `in-progress/` and `deprecated/` must not appear in either.

Each skill entry in the top-level `README.md` must link the skill name to its `SKILL.md`.

Each bucket folder has a `README.md` that lists every skill in the bucket with a one-line description, with the skill name linked to its `SKILL.md`.

## Adding a skill

1. Create `skills/<bucket>/<skill-name>/SKILL.md` with YAML frontmatter (`name`, `description`) and the skill body.
2. Add `"./skills/<bucket>/<skill-name>"` to the `skills` array in `.claude-plugin/plugin.json`.
3. Add a linked reference in the bucket `README.md` and the top-level `README.md`.
