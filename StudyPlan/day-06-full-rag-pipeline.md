# Day 6 - Full RAG Pipeline

## Goal

Move from pure retrieval to grounded answering with a local LLM.

## Module

- `BookSearch/app_v1.py`
- `BookSearch/app_v2.py`

## Prerequisites

- Python installed
- Ollama installed
- Models pulled:

```bash
ollama pull llama3.3:latest
ollama pull nomic-embed-text
```

## Install

```bash
cd BookSearch
pip install -r requirements.txt
```

## Run

### Version 1

```bash
python app_v1.py init
python app_v1.py demo
```

### Version 2

```bash
python app_v2.py init
python app_v2.py ingest --dir ./books
python app_v2.py ask "Who is Sherlock Holmes?"
python app_v2.py stats
```

## Focus Questions

- What changes between a search system and a RAG system?
- How is the prompt built from retrieved chunks?
- Why do citations matter?
- What is the purpose of top-k retrieval before generation?

## Deliverables

- Add Day 6 notes to `outputs/daily-log-template.md`
- Write down the purpose of:
  - embeddings
  - top-k retrieval
  - context assembly
  - grounded prompting
  - citations

## Completion Check

You are done with Day 6 when you can explain the end-to-end RAG loop without relying on the README.
