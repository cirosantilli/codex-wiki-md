<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The exponential map is a conformal bijection from the strip

$$
\mathcal S=\{z:-\alpha<\operatorname{Im}z<\beta\}
$$

to the wedge containing the starting point $1$. The restriction $\alpha+\beta<2\pi$ makes it injective. A [planar Brownian motion](../../../../../../planar-brownian-motion.md) $U+iV$ started at zero in this strip maps, after the [conformal Brownian clock](../../../../../../conformal-brownian-clock.md), to the required [Brownian motion](../../../../../../brownian-motion-split.md) in the wedge.

Let $\sigma$ be the first time $V$ exits $(-\alpha,\beta)$. It is finite [almost surely](../../../../../../almost-sure-convergence.md), and $V_{t\wedge\sigma}$ is a bounded [martingale](../../../../../../martingale-split.md). The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
0=\mathbb E V_\sigma
=\beta p-\alpha(1-p),
\qquad p=\mathbb P(V_\sigma=\beta).
$$

The strip exit maps to the corresponding bounding ray. The exponential clock is finite at $\sigma$, because its integrand is continuous on the compact time interval $[0,\sigma]$. Thus it does not remove or reverse the exit event. We obtain

$$
\boxed{\mathbb P(S_\beta<S_{-\alpha})=\frac{\alpha}{\alpha+\beta}.}
$$

This is the [Brownian wedge-exit probability](../../../../../../brownian-wedge-exit-probability.md) obtained directly from the strip, using [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
