# Example family package

This scaffold shows the layout every family follows.

- `docs/brief.md` and `docs/prompt.md` are the human-facing briefs; both are required, must be
  non-empty and must be written in English.
- `eval/run.py`, `data/`, `groundtruth/` and `notes/` are optional in the sense that their
  contents are free-form; keep whatever material the family needs.

## Canonical rendering

`data/records.jsonl` contains two exported conversations and
`data/expected_messages.jsonl` contains their canonical rendering, one JSON object per line.
The pair is the normative reference for the canonical message form used in releases: field
names, ordering and the treatment of call turns and return records must match it exactly.
