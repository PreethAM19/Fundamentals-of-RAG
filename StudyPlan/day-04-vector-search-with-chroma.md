# Day 4 - Vector Search With Chroma

## Goal

Learn the retrieval pipeline before adding LLM generation.

## Module

- `ChromaDemo`

## Read First

- `ChromaDemo/README.md`

## Install

```bash
cd ChromaDemo
pip install -r requirements.txt
```

## Run

```bash
python ingest_and_query.py
```

Then edit the search calls at the bottom of the script and try your own natural-language queries.

## Focus Questions

- How are chunks persisted in the vector store?
- What is the role of the embedding function?
- What does the returned metadata tell you?
- When do the top matches feel strong, weak, or surprising?

## Deliverables

- Add Day 4 notes to `outputs/daily-log-template.md`
- Capture at least 3 retrieval examples in your log:
  - one good
  - one weak
  - one surprising

## Completion Check

You are done with Day 4 when you can describe the pipeline as:

`document -> chunk -> embedding -> vector DB -> similarity search`
