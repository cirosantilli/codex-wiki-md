<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $a=0$ and $b>0$, the recurrence is $p_n=(b/n)p_{n-1}$. Iteration gives $p_n=p_0b^n/n!$. Since $\sum_{n\ge0}b^n/n!=e^b$, normalization gives

$$
\boxed{N\sim\operatorname{Poisson}(b),\qquad p_n=e^{-b}\frac{b^n}{n!}.}
$$

Hence the [claim count distribution](../../../../../../claim-count-distribution.md) is a [Poisson distribution](../../../../../../poisson-distribution.md) of mean $b$, and the [Panjer recursion](../../../../../../panjer-recursion.md) begins at $g_0=e^{-b}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
