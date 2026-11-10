# Family packages

Each candidate family lives in its own directory under `families/<slug>/` and follows the
shared skeleton used across the corpus:

```
<slug>/
  docs/
    brief.md        # short human-facing description of the family
    prompt.md       # the system prompt used to seed the family's conversations
  eval/
    run.py          # evaluation harness entry point
  data/
    records.jsonl   # exported conversations
```

The scaffold under `families/_example/` shows the layout and is not itself a candidate
family.

Only the human-facing documentation has strict content requirements: `docs/brief.md` and
`docs/prompt.md` must exist, be non-empty and be written in English. Everything under
`eval/`, `data/`, `groundtruth/` and `notes/` is optional -- those files are placeholders and
their contents are entirely up to each family's maintainers.

Families that are still being prepared may be missing parts of the skeleton. They stay on the
tracker until the package is complete.
