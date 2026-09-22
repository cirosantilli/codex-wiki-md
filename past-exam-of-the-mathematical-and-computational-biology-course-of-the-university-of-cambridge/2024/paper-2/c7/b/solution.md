<h1 id="c7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the number of alignment columns, including gap columns, as the denominator. A column contributes to [sequence identity](../../../../../sequence-identity.md) when its two nongap letters are equal, to [sequence similarity](../../../../../sequence-similarity.md) when its two nongap letters have a strictly positive [BLOSUM62](../../../../../blosum62.md) score, and to the [gap fraction](../../../../../gap-fraction.md) when either letter is a gap. A zero substitution score is not counted as similar.

The implementation in part (a) computes each numerator directly during its final pass through the aligned strings:

```
for name, a in alignments.items():
    print(name, a["alignment_length"], a["identities"],
          a["similarities"], a["gaps"])
    print(a["identity_percent"], a["similarity_percent"], a["gap_percent"])
```

| Query | Columns | Identical | Similar | Gap columns |
| --- | --- | --- | --- | --- |
| baboon | 66 | 63 (95.45%) | 65 (98.48%) | 1 (1.52%) |
| squirrel monkey | 58 | 49 (84.48%) | 50 (86.21%) | 4 (6.90%) |
| dingo | 71 | 57 (80.28%) | 59 (83.10%) | 10 (14.08%) |
| goldfish | 72 | 34 (47.22%) | 50 (69.44%) | 14 (19.44%) |

Identical columns also count as similar for these data, so these percentages are overlapping summaries rather than three categories summing to 100%.

## ↑ Ancestors (13)

1. [B](../b.md)
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
