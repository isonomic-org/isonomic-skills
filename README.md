# Isonomic Skills

The skills bundled with Isonomic, in the open Agent Skills format, with the
record, checks and evaluation for each one.

A skill is a folder that teaches an agent one kind of task. In Isonomic a skill
is data and never authority: it cannot change policy, approvals, grants,
budgets, tools or presets. Its scripts run as ordinary commands, with the same
approvals and confinement as any other command.

## Layout

| Path | Holds |
| --- | --- |
| `skills/<name>/` | The skill in the open format, with the upstream licence file when it was imported |
| `skills/<name>/record.toml` | Source ID and upstream commit, licence, the kits it needs, who reviewed it and when, the models it was tested on, the tool-name changes made |
| `evals/<name>/` | At least two tasks per skill, each with a starting state and a check on the end state |
| `catalog.json` | Generated: name, version, hash, summary and kits for every skill, signed at release |
| `THIRD_PARTY_NOTICES.md` | The attributions the licences require |

No skill enters the bundled set without passing the intake pipeline: licence,
format, scan, adaptation, review, evaluation and pin.

## Licence

Isonomic's own content is licensed under the Apache License 2.0. See
[LICENSE](LICENSE). Each imported skill keeps its own licence, in the licence
file inside that skill's folder.

Copyright 2026 Anud Inc.
