# AGENTS.md — Evals Repository

Forked from OpenAI's evals framework. Extended with phext-native evaluation suites.

## Custom Evals (exo branch)

| Eval | Samples | Tests |
|------|---------|-------|
| `base256` | 135 | Byte↔syllable encoding/decoding, ASCII string encoding, boundary cases |
| `phext_delimiters` | 27 | 9 delimiters × 3 questions (dimension, hex value, Base 256 pronunciation) |
| `phext_coordinates` | 16 | Coordinate navigation, delimiter transitions, Mirrorborn roster, vTPU architecture |

## Purpose

Measure how well LLMs understand phext, Base 256, and vTPU architecture. These evals establish a baseline for phext-native AI literacy.

## Convention

- All lowercase filenames
- Eval data in `evals/registry/data/<eval_name>/samples.jsonl`
- Eval config in `evals/registry/evals/<eval_name>.yaml`
