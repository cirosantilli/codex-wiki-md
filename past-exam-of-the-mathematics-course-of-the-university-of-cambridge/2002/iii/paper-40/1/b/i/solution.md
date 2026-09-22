<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [quantile function](../../../../../../../quantile-function.md) $F^{-1}(u)=\inf\{x:F(x)\geq u\}$ for $0<u<1$, so a strictly increasing CDF is not required. For any real $x$, the quantile event $F^{-1}(U)\leq x$ agrees, up to endpoint null sets, with $U\leq F(x)$. Hence

$$
\mathbb P(F^{-1}(U)\leq x)=\mathbb P(U\leq F(x))=F(x).
$$

Thus **$F^{-1}(U)$ has distribution function $F$ and [probability density function](../../../../../../../probability-density-function.md) $f$**. This proves [inverse transform sampling](../../../../../../../inverse-transform-sampling.md), including a [probability density function](../../../../../../../probability-density-function.md) with intervals on which the CDF is constant.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
