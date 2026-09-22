<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Build an [FM-index](../../../../../fm-index.md): store the [Burrows-Wheeler transform](../../../../../burrows-wheeler-transform.md), cumulative character counts $C$, and a structure supporting fast [rank queries](../../../../../rank-query.md) for $\operatorname{Occ}(c,r)$. Then each step of [backward search](../../../../../backward-search.md) uses two [rank queries](../../../../../rank-query.md) instead of rescanning the last column. A [wavelet tree](../../../../../wavelet-tree.md) or suitably checkpointed counts can supply these queries while keeping memory manageable. The counting cost is proportional to query length times the [rank query](../../../../../rank-query.md) cost, rather than repeatedly scanning the whole [genome](../../../../../genome.md).[§2, LF-mapping; §§3.1–3.2, counting and locating occurrences](../../../../../opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others.md)

To recover genomic positions, store a sampled [suffix array](../../../../../suffix-array.md) and follow the [last-to-first mapping](../../../../../last-to-first-mapping.md) to a sampled position, adding the number of steps taken. More samples trade storage for faster position recovery. **Index character counts and sample positions**, rather than storing the quadratic-size full [cyclic rotation](../../../../../cyclic-rotation.md) [matrix](../../../../../matrix.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
