# Day 2 - Real Document Parsing

## Goal

Learn how ingestion changes when the source is a PDF or DOCX instead of plain text or CSV.

## Modules

- `PDFParser`
- `WordParser`

## Read First

- `PDFParser/README.md`
- `WordParser/README.md`

## Install

```bash
cd PDFParser
pip install -r requirements.txt
```

```bash
cd ../WordParser
pip install -r requirements.txt
```

## Run

### PDFParser

```bash
cd ../PDFParser
python main.py
```

### WordParser

```bash
cd ../WordParser
python main.py
```

## Focus Questions

- What parser limitations show up with PDF extraction?
- What metadata does `WordParser` preserve that `PDFParser` does not?
- Why are PDFs often harder to ingest cleanly?
- Why is preserving document structure useful for downstream chunking?

## Deliverables

- Fill in `outputs/parser-comparison.md`
- Add notes in `outputs/daily-log-template.md` for Day 2

## Completion Check

You are done with Day 2 when you can compare:
- plain text vs PDF vs DOCX ingestion
- parser quality vs parser simplicity
- metadata richness vs extraction reliability
