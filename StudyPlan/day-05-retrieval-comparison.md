# Day 5 - BM25 vs Semantic vs Hybrid Retrieval

## Goal

Build intuition about when keyword search, semantic search, or hybrid search works best.

## Module

- `SearchTool`

## Read First

- Open the notebooks in `SearchTool/`
- Start with `BM25-vs-Semantic.ipynb`

## Install

```bash
cd SearchTool
pip install -r requirements.txt
```

## Run

Launch Jupyter and open the notebook:

```bash
jupyter lab
```

If you prefer, open the notebook directly in VS Code.

## What To Compare

- Queries that rely on exact wording or acronyms
- Queries that rely on meaning rather than literal keywords
- Queries where hybrid retrieval should outperform either single method

## Exercise

Create at least five example queries and predict the winner before you inspect results.

## Deliverables

- Fill in `outputs/retrieval-comparison.md`
- Add your five query examples and notes

## Completion Check

You are done with Day 5 when you can explain:
- when BM25 wins
- when semantic retrieval wins
- why hybrid retrieval is often the safest default
