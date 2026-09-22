<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Count unordered sets of distinct labelled fish: there are $\binom NM$ possible hauls. To obtain exactly $j$ trout, choose $j$ labels from the $K$ trout and $M-j$ from the $N-K$ carp, giving $\binom Kj\binom{N-K}{M-j}$ possibilities. Uniform [sampling without replacement](../../../../../sampling-without-replacement.md) therefore gives the [hypergeometric distribution](../../../../../hypergeometric-distribution.md)

$$
\boxed{p_j=\frac{\binom Kj\binom{N-K}{M-j}}{\binom NM},
\quad\max(0,M-N+K)\leq j\leq\min(M,K).}
$$

Outside this integer range the [probability](../../../../../probability.md) is zero. If ordered catches were counted instead, every haul would have $M!$ orders and that factor would cancel from the [probability](../../../../../probability.md) ratio.

Here equal catchability means equal selection [probability](../../../../../probability.md) for each individual remaining fish. It does not [mean](../../../../../expected-value-split.md) that the two species have [probability](../../../../../probability.md) $1/2$ on each draw regardless of their populations. This interpretation is the one that yields the stated hypergeometric law.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
