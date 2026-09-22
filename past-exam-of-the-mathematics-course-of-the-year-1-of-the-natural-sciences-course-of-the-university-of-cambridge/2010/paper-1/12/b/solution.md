<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After $j$ choices, let $C_j$ be the number of forward moves. The two unwrapped positions are $C_j$ and $F-(j-C_j)$, whose gap is $F-j$. It follows that the first subsequent meeting occurs exactly at step $F$, regardless of the order of the choices. Its [position](../../../../../position.md) is the number of forward moves in that block.

That count has a [binomial distribution](../../../../../binomial-distribution.md) with parameters $F,p$. Therefore

$$
\boxed{p_n^{\rm meet}=\binom Fn p^nq^{F-n},\qquad 0\leq n\leq F.}
$$

The two endpoint labels $0$ and $F$ represent the same physical seat reached by different complete circuits; the unwrapped convention distinguishes their [probabilities](../../../../../probability.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
