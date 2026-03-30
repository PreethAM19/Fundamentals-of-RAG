# Day 1 - Setup and Simple Ingestion

## Goal

Understand what a RAG-ready document looks like and how raw source data is turned into searchable text plus metadata.

## Modules

- `TextParser`
- `CSVParser`

## Read First

- Root `README.md` overview and repository structure
- `TextParser/README.md`
- `CSVParser/README.md`

## Run

### TextParser

```bash
cd TextParser
python main.py
```

If `python` is not available yet, install Python first and try again.

### CSVParser

```bash
cd ../CSVParser
python main.py
```

## Focus Questions

- What is the shape of a chunk in `TextParser`?
- What metadata is attached to each text chunk?
- How does `CSVParser` turn one row into a text field that can be embedded later?
- What is the tradeoff when you flatten structured data into plain text?

## Deliverables

- Fill in `outputs/daily-log-template.md`
- Answer these in your log:
  - What is a chunk?
  - Why does metadata matter?
  - How is a CSV row converted into searchable text?

## Completion Check

You are done with Day 1 when you can explain:
- the difference between `text` and `metadata`
- why chunking exists at all
- why structured data still has to be converted into readable text for semantic search
