<h1 id="14/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $T$ count tests up to and including the first failure. By [independence of random variables](../../../../../../independent-random-variables.md), the event $T=j$ requires $j-1$ passes and then a failure. With pass [probability](../../../../../../probability.md) $p=1/2$ and failure [probability](../../../../../../probability.md) $q=1/2$, this is the [geometric distribution](../../../../../../geometric-distribution.md)

$$
\mathbb P(T=j)=q p^{j-1},\qquad j=1,2,\ldots.
$$

Using part (iii), its [expected value](../../../../../../expected-value-split.md) is

$$
\boxed{\mathbb E[T]=q\sum_{j=1}^{\infty}jp^{j-1}
=\frac{q}{(1-p)^2}=\frac1q=2.}
$$

This counts the test that discovers the fault. The expected number of earlier passing tests alone would be one.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [14](../../../14.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
