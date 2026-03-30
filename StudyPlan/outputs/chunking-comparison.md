# Chunking Comparison Sheet

Fill this in after Day 3.

| Method | Boundary Style | Best For | Main Risk | What I Observed |
| --- | --- | --- | --- | --- |
| Fixed | character count | fast baselines, generic corpora | may split ideas mid-sentence | |
| Sliding | overlapping windows | preserving context between nearby chunks | duplication and noisy retrieval | |
| Sentence | sentence boundaries | short answers, precise retrieval | may lose larger context | |
| Paragraph | paragraph boundaries | articles, notes, structured prose | uneven chunk sizes | |
| Section | heading boundaries | manuals, docs with headings | depends on reliable structure | |
| Token | tokenizer boundaries | model-aware chunk budgets | extra dependency and less human-readable boundaries | |

## My Final Picks

- Books and articles:
- Technical docs:
- Structured notes:

## Why

Write 3 to 5 sentences explaining the tradeoff you chose.
