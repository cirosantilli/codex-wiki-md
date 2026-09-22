<h1 id="16/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume that wrong-note events are [independent events](../../../../../independent-events.md) and that each note has the same error [probability](../../../../../probability.md) $p$, with $0\leq p\leq1$. Then their count $N$ has a [binomial distribution](../../../../../binomial-distribution.md). Choose the $n$ mistaken positions in $\binom{100}{n}$ ways and multiply the probabilities of the errors and correct notes:

$$
\boxed{\mathbb P(N=n)=\binom{100}{n}p^n(1-p)^{100-n},\qquad n=0,1,\ldots,100.}
$$

The endpoint cases $p=0$ or $p=1$ are understood by continuity, giving deterministic counts. More than half means at least $51$ mistakes, so

$$
\boxed{\mathbb P(\text{booing})=\sum_{n=51}^{100}\binom{100}{n}p^n(1-p)^{100-n}.}
$$

The single-note error [probability](../../../../../probability.md) alone would not determine this count distribution if mistakes were correlated; [independence](../../../../../independent-random-variables.md) is the additional standard modeling assumption.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [16](../../16.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
