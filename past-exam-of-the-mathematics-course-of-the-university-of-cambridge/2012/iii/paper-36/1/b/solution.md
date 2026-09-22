<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $r_t=\sqrt{p_t}-\sqrt p-(t/2)g\sqrt p$. By [differentiability in quadratic mean](../../../../../../differentiability-in-quadratic-mean.md), $\|r_t\|_{L^2(\mu)}=o(|t|)$ and

$$
\frac{\sqrt{p_t}-\sqrt p}{t}\longrightarrow\frac12g\sqrt p,
\qquad
\sqrt{p_t}+\sqrt p\longrightarrow2\sqrt p
$$

in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). The second limit follows because the first gives $\|\sqrt{p_t}-\sqrt p\|_2=O(|t|)$.

Both [probability density functions](../../../../../../probability-density-function.md) integrate to one. Consequently the [L2 inner product](../../../../../../l2-inner-product.md) satisfies

$$
0=\frac1t\int(p_t-p)\,d\mu
=\left\langle\frac{\sqrt{p_t}-\sqrt p}{t},\sqrt{p_t}+\sqrt p\right\rangle_{L^2(\mu)}.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) permits passage to the limit in this [inner product](../../../../../../inner-product.md), giving

$$
\boxed{Pg=\int g\,dP=0.}
$$

Thus every [score function](../../../../../../informant-function.md) is a [mean-zero function](../../../../../../mean-zero-function.md). This proof uses square-root [differentiability in quadratic mean](../../../../../../differentiability-in-quadratic-mean.md), without requiring differentiation under the density [integral](../../../../../../integral.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
