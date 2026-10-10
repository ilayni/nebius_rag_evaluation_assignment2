# RAG Assignment 2 — Retrieval, Generation and Evaluation

Assignment 2 of the Nebius ML course: a RAG pipeline with naive-generation
baselines, iterative improvement cycles, and RAGAS-based evaluation.

## Contents

| Path | What it is |
|---|---|
| `assignment2_rag_ilay_nisim_boris_kogan.ipynb` | Full pipeline: retrieval, generation, improvement cycles, evaluation |

| `assignment2_naive_generation_*.xlsx` | Baseline (no retrieval) generation results |
| `assignment2_run_and_compare_*.xlsx` | Side-by-side run comparison |
| `assignment2_improvement_cycles_*.xlsx` | Iterative improvement cycle results |
| `assignment2_evaluation_*.xlsx` | RAGAS evaluation scores |

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


## Note on paths

Some files (notebook outputs, plan docs) contain the placeholder path `/Users/YOUR_USER`. It replaces the original author's local home directory. If you run or adapt this project, replace `YOUR_USER` with your own username (or the relevant local path) wherever it appears, e.g. `grep -rn "YOUR_USER" .`.
