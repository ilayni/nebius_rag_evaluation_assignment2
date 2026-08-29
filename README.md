# RAG Assignment 2 — Retrieval, Generation and Evaluation

Assignment 2 of the Nebius ML course: a RAG pipeline with naive-generation
baselines, iterative improvement cycles, and RAGAS-based evaluation.

## Contents

| Path | What it is |
|---|---|
| `assignment2_rag_ilay_nisim_boris_kogan.ipynb` | Full pipeline: retrieval, generation, improvement cycles, evaluation |

> The accompanying `.xlsx` result workbooks (naive generation, run-and-compare,
> improvement cycles, evaluation) are intentionally **not** committed — they are
> generated artifacts and are covered by `.gitignore`.

## Setup

```bash
cp .env.example .env   # then fill in NEBIUS_API_KEY
```

The notebook reads credentials from the environment:

```python
NEBIUS_API_KEY  = os.environ["NEBIUS_API_KEY"]
NEBIUS_BASE_URL = "https://api.studio.nebius.ai/v1/"
```

`.env` is git-ignored; never commit real credentials.
