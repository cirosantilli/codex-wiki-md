<h1 id="c8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Columns 22–28 form one run between alignment columns 21 and 29, corresponding to [match states](../../../../../match-state.md) $M_{21}$ and $M_{22}$. A self-repeating [insertion state](../../../../../insertion-state.md) can emit a variable number of residues, so these seven alignment columns require **one populated [insertion state](../../../../../insertion-state.md)**, not seven successive mandatory states.

Pool all nongap residues in this run to estimate its [emission probabilities](../../../../../emission-probability.md):

```
insert_columns = np.flatnonzero(~match_mask)
runs = np.split(insert_columns, np.flatnonzero(np.diff(insert_columns) > 1) + 1)
insert_emissions = []
for run in runs:
    if len(run):
        counts, n = emission_counts(A[:, run].ravel())
        insert_emissions.append({aa: count/n for aa, count in counts.items()})
        print(run+1, n, insert_emissions[-1])
```

There are **24 emitted residues**, giving

$$
\begin{array}{c|rrrrrrrrrrr}
a&A&D&E&G&H&I&L&N&P&T&V\\\hline
24\,p_I(a)&1&3&7&1&2&1&2&2&1&1&3
\end{array}
$$

All other [amino acids](../../../../../amino-acid.md) have probability zero in this empirical [emission probabilities](../../../../../emission-probability.md). A conventional full architecture may provide an optional [insertion state](../../../../../insertion-state.md) at every boundary, including the two ends, giving $72+1=73$ possible insertion positions; only one has an observed insertion here and is required by this alignment's populated insertion region.

## ↑ Ancestors (13)

1. [D](../d.md)
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
