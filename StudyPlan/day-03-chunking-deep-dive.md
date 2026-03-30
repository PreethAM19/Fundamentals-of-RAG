# Day 3 - Chunking Deep Dive

## Goal

Understand the design tradeoffs behind chunk size, overlap, and chunking method selection.

## Module

- `ChunkingDemo`

## Read First

- `ChunkingDemo/README.md`

## Install

```bash
cd ChunkingDemo
pip install -r requirements.txt
```

## Run At Least Five Methods

```bash
python document_chunker.py sample_document.txt fixed --chunk-size 500 --overlap 50
python document_chunker.py sample_document.txt sliding --window-size 800 --step-size 400
python document_chunker.py sample_document.txt sentence --max-sentences 3
python document_chunker.py sample_document.txt paragraph --max-paragraphs 2
python document_chunker.py sample_document.txt section --heading-pattern "^#{1,6}\\s+"
```

Optional:

```bash
python document_chunker.py sample_document.txt token --max-tokens 256
```

## Focus Questions

- Which method keeps meaning together best?
- Which method creates the cleanest retrieval units?
- When does overlap help?
- When does overlap just create noise and duplication?

## Deliverables

- Fill in `outputs/chunking-comparison.md`
- Write your preferred strategy for:
  - books and articles
  - technical docs
  - structured notes

## Completion Check

You are done with Day 3 when you can justify a chunking strategy instead of picking one by habit.
