<h1 id="c7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The maximum-scoring cell records the inclusive end position in each sequence. During traceback, moving left consumes a reference residue, moving up consumes a query residue, and moving diagonally consumes both; when traceback stops, the remaining prefix lengths are one less than the corresponding one-based starts. Consequently `i+1` and `j+1` are the correct starts returned in part (a), without counting any inserted gaps as sequence residues.

The following report joins these coordinates to the alignments and [sequence identity](../../../../../sequence-identity.md)/[sequence similarity](../../../../../sequence-similarity.md) values already calculated:

```
for name, a in alignments.items():
    print(f"{name}: query length={a['query_length']}, "
          f"reference length={a['reference_length']}, "
          f"alignment columns={a['alignment_length']}, score={a['score']}")
    print(f"Query {a['query_start']} {a['query']} {a['query_end']}")
    print(f"Ref   {a['reference_start']} {a['reference']} {a['reference_end']}")
    print(f"Identity {a['identity_percent']:.2f}%; "
          f"similarity {a['similarity_percent']:.2f}%; "
          f"gaps {a['gap_percent']:.2f}%")
```

All reference sequences have length **508**. The following are one-based inclusive coordinates; the aligned strings and all percentages are given in parts (a) and (b).

| Query | Query length | Query interval | Reference interval | Columns | Score |
| --- | --- | --- | --- | --- | --- |
| baboon | 65 | 1–65 | 241–306 | 66 | 314 |
| squirrel monkey | 56 | 1–56 | 61–116 | 58 | 278 |
| dingo | 66 | 1–66 | 1–66 | 71 | 301 |
| goldfish | 63 | 2–63 | 248–315 | 72 | 190 |

For example, the goldfish [local sequence alignment](../../../../../local-sequence-alignment.md) excludes its first query residue and aligns residues 2–63. As a check, removing gaps from each aligned string gives exactly the sequence slice determined by its reported interval.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [C7](../../c7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
