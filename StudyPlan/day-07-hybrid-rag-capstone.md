# Day 7 - Hybrid RAG and Mini Capstone

## Goal

Finish the week by running hybrid retrieval and evaluating a small corpus of your own.

## Module

- `BookSearch/hybrid_rag.py`

## Corpus Options

- Use your own 3 to 5 short `.txt` files
- Or use the ready-made files in `StudyPlan/capstone-corpus/`

## Prerequisites

- Everything from Day 6

## Run

```bash
cd BookSearch
python hybrid_rag.py ingest --dir ../StudyPlan/capstone-corpus
python hybrid_rag.py ask --query "Why is overlap useful in chunking?"
```

Try at least 8 to 10 questions over your corpus.

## What To Evaluate

- Which questions worked well?
- Which questions failed?
- Was the failure caused by parsing, chunking, retrieval, or prompting?
- Would pure semantic search or pure BM25 have done worse?

## Suggested Questions For The Included Corpus

- Why is metadata important in RAG pipelines?
- When is BM25 likely to beat semantic retrieval?
- Why do people use overlap in chunking?
- What is a common failure mode during evaluation?
- Why should answers include citations?

## Deliverables

- Fill in `outputs/capstone-summary.md`
- Mark completion in `outputs/weekly-checklist.md`

## Completion Check

You are done with Day 7 when you can:
- run hybrid ingestion
- ask grounded questions over a local corpus
- explain at least one failure mode
- name one improvement you would make next
