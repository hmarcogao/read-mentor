# Read Mentor

A Codex skill for deep reading through active recall, Socratic questioning, argument mapping, spaced review, and evidence-based recommendations.

## Install

Copy this repository into your Codex skills directory as `read-mentor`, then invoke `$read-mentor` in Codex.

The skill stores personal reading records outside the skill directory at `$CODEX_HOME/read-mentor-data` (or `~/.codex/read-mentor-data`). Personal archives are intentionally excluded from this repository.

## Included

- `SKILL.md`: core behavior and safety boundaries
- `agents/openai.yaml`: display metadata
- `references/`: session playbooks, data model, and knowledge-map guidance
- `examples/read-mentor-data/`: sanitized, empty templates only

## Privacy

Never commit a real `read-mentor-data` directory. The root `.gitignore` excludes it; the files under `examples/` contain no personal reading history.
