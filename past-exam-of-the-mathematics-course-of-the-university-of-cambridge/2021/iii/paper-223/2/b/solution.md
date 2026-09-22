<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $m=\lfloor\alpha n\rfloor$. If at most $m$ observations are replaced arbitrarily, every order statistic retained between ranks $m+1$ and $n-m$ remains between the minimum and maximum of the unreplaced observations. The trimmed mean is therefore bounded as the replacement values diverge.

If more than $m$ observations are replaced by a common value tending to $+\infty$, at least one replacement remains after the largest $m$ observations are trimmed, and the trimmed mean tends to $+\infty$. The analogous construction tends to $-\infty$. Thus the largest fraction of arbitrary replacements for which boundedness is guaranteed is

$$
\boxed{\varepsilon_n^*=\frac{\lfloor\alpha n\rfloor}{n}}.
$$

This is the convention for the finite-sample [replacement breakdown point](../../../../../../replacement-breakdown-point.md) used in the question; the alternative convention based on the smallest breaking fraction reports $(m+1)/n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
