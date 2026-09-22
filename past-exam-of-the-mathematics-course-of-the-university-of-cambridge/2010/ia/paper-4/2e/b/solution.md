<h1 id="2e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [exponential series](../../../../../../exponential-series.md) at $1$ gives

$$
\boxed{e=\sum_{n=0}^{\infty}\frac1{n!}.}
$$

For every positive [integer](../../../../../../integer.md) $q$, multiply by the [factorial](../../../../../../factorial.md) $q!$ and separate the integer part:

$$
q!e=\underbrace{\sum_{n=0}^{q}\frac{q!}{n!}}_{I_q\in\mathbb Z}
+R_q,\qquad
R_q=\sum_{j=1}^{\infty}\frac1{(q+1)(q+2)\cdots(q+j)}.
$$

Every term in $R_q$ is positive. Each denominator is at least $(q+1)^j$, and the inequality is strict when $j\ge2$. Comparison with the [geometric series](../../../../../../geometric-series.md) therefore gives

$$
0<R_q<\sum_{j=1}^{\infty}(q+1)^{-j}=\frac1q\le1.
$$

If $e=p/q$ with integers $p$ and $q\ge1$, then $q!e=p(q-1)!$ would be an [integer](../../../../../../integer.md). Since $I_q$ is also an [integer](../../../../../../integer.md), $R_q$ would be an [integer](../../../../../../integer.md) strictly between zero and one, which is impossible. Hence

$$
\boxed{e\text{ is irrational}.}
$$

This proves the [irrationality of e](../../../../../../irrationality-of-e.md) by using its rapidly decreasing series tail.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2E](../../2e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
