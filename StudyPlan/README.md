# One-Week RAG Study Plan

This folder turns the repository into a one-week guided course.

It is designed for:
- 2 to 3 hours per day
- balanced learning across ingestion, chunking, retrieval, and end-to-end RAG
- a final mini capstone on Day 7

## What Is In This Folder

- `day-01-setup-and-simple-ingestion.md` through `day-07-hybrid-rag-capstone.md`: daily guides
- `outputs/`: fill-in templates for logs, comparison sheets, and the final capstone summary
- `capstone-corpus/`: a small ready-to-use corpus for Day 7 if you do not want to source your own files yet

## Environment Note

I validated the local workspace before writing this guide:
- `py.exe` exists on this machine, but there is no active Python runtime installed yet
- `ollama` was not found on `PATH`

That means you should expect to do the setup below before running the Python demos in this repo.

## Setup Checklist

1. Install Python 3.11 or newer.
2. Confirm one of these works:
   - `python --version`
   - `py -3 --version`
3. Install Ollama for Days 6 and 7.
4. Pull the local models needed by `BookSearch`:
   - `ollama pull llama3.3:latest`
   - `ollama pull nomic-embed-text`

## Suggested Daily Time Split

- 20 minutes: read the day guide and repo docs
- 60 to 80 minutes: run the examples and inspect outputs
- 20 to 30 minutes: fill in the matching output template
- 20 to 30 minutes: write down what worked, what failed, and what you would change

## Weekly Flow

- Day 1: [Setup and simple ingestion](./day-01-setup-and-simple-ingestion.md)
- Day 2: [Real document parsing](./day-02-real-document-parsing.md)
- Day 3: [Chunking deep dive](./day-03-chunking-deep-dive.md)
- Day 4: [Vector search with Chroma](./day-04-vector-search-with-chroma.md)
- Day 5: [BM25 vs semantic vs hybrid retrieval](./day-05-retrieval-comparison.md)
- Day 6: [Full RAG pipeline](./day-06-full-rag-pipeline.md)
- Day 7: [Hybrid RAG and capstone](./day-07-hybrid-rag-capstone.md)

## Output Templates

- [Daily log template](./outputs/daily-log-template.md)
- [Weekly checklist](./outputs/weekly-checklist.md)
- [Parser comparison](./outputs/parser-comparison.md)
- [Chunking comparison](./outputs/chunking-comparison.md)
- [Retrieval comparison](./outputs/retrieval-comparison.md)
- [Capstone summary](./outputs/capstone-summary.md)

## Recommended Repo Order

If you ever get behind, protect this order:
1. `TextParser` and `CSVParser`
2. `ChunkingDemo`
3. `ChromaDemo`
4. `BookSearch/app_v1.py` and `app_v2.py`
5. `BookSearch/hybrid_rag.py`

That sequence preserves the main learning arc even if you have to skip some optional depth.
