# Parser Comparison Sheet

Fill this in after Days 1 and 2.

| Parser | Input Type | Output Shape | Metadata Preserved | Common Limitation | Best Use Case | My Notes |
| --- | --- | --- | --- | --- | --- | --- |
| TextParser | `.txt` | overlapping chunks with file metadata | filename, file path, size, extension, document id, counts | plain text only | notes, logs, markdown-like text | |
| CSVParser | `.csv` | one document per row | source file, row number, all original columns | row meaning may be flattened into generic text | tables, exports, structured records | |
| PDFParser | `.pdf` | chunk list with source and chunk info | source path, chunk id, total chunks | extraction quality depends on PDF structure | manuals, reports, papers | |
| WordParser | `.docx` | chunk list with document metadata | title, author, created, modified, filename | formatting and complex layout are not preserved | business docs, reports, meeting notes | |

## Reflection Prompts

- Which parser produced the cleanest text?
- Which parser preserved the richest metadata?
- Which parser would you trust least on messy real-world input?
