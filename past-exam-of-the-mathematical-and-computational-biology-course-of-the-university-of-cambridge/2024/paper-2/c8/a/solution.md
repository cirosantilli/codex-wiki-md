<h1 id="c8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Convert the supplied [multiple sequence alignment](../../../../../multiple-sequence-alignment.md) to an ordinary array so that reducing over rows returns one value per column. With nine sequences, fewer than 30% gaps means at most two gaps in a column:

```
from collections import Counter
A = np.asarray(msa_matrix)
gap_fraction = np.mean(A == ".", axis=0)
match_mask = gap_fraction < .30
match_columns = np.flatnonzero(match_mask)
print(match_columns + 1)  # human-readable, one-based alignment columns
```

**There are 72 [match states](../../../../../match-state.md): alignment columns 1–21 and 29–79**, using one-based numbering. The seven remaining columns, 22–28, form one contiguous insertion region. The strict inequality is applied to the actual fraction, rather than to rounded percentages.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [C8](../../c8.md)
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
