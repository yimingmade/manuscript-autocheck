# Manuscript Autocheck Skills

Codex skills for auditing manuscripts, tables, supplementary materials, and response-to-reviewers documents before journal submission.

## Contents

- `skills/manuscript-presubmission-checklist/SKILL.md` - pre-submission checklist for manuscripts, tables, and supplementary materials.
- `skills/manuscript-presubmission-checklist/agents/openai.yaml` - optional Codex UI metadata.
- `skills/manuscript-presubmission-checklist-revision/SKILL.md` - revision-stage checklist for manuscripts, supplementary materials, and response-to-reviewers documents.
- `skills/manuscript-presubmission-checklist-revision/agents/openai.yaml` - optional Codex UI metadata.

## Install

Install both skills from this repository:

```bash
python3 install-skill-from-github.py --repo yimingmade/manuscript-autocheck --path skills/manuscript-presubmission-checklist skills/manuscript-presubmission-checklist-revision
```

Or install one skill at a time:

```bash
python3 install-skill-from-github.py --repo yimingmade/manuscript-autocheck --path skills/manuscript-presubmission-checklist
python3 install-skill-from-github.py --repo yimingmade/manuscript-autocheck --path skills/manuscript-presubmission-checklist-revision
```

Or copy the skill directories directly:

```bash
cp -R skills/manuscript-presubmission-checklist ~/.codex/skills/
cp -R skills/manuscript-presubmission-checklist-revision ~/.codex/skills/
```

Restart Codex after installation.

## Dependencies

The skill has no local file, script, package, or runtime dependencies.

## Licence

MIT License. See `LICENSE`.
