<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The future levels are independent of the observed maximum. Given $Y_n=z$, the first $k-1$ future levels must be at most $z$, and the $k$th must exceed $z$. Each non-overflow has [probability](../../../../../../probability.md) $F(z)$ and an overflow has [probability](../../../../../../probability.md) $1-F(z)$. Therefore

$$
\boxed{P(\tau=k\mid Y_n=z)=F(z)^{k-1}[1-F(z)],\qquad k\geq1.}
$$

This is a [geometric distribution](../../../../../../geometric-distribution.md) of parameter $1-F(z)$ when $F(z)<1$. Since $Y_n$ has a continuous distribution, conditioning on an exact value is understood via a [regular conditional distribution](../../../../../../regular-conditional-distribution.md), rather than division by $P(Y_n=z)=0$. The formula specifies its usual version. If $F(z)=1$ there is no possible overflow at that threshold, but such thresholds have [probability](../../../../../../probability.md) zero for the random observed maximum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
