<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $T<\infty$. By [uniform continuity](../../../../../../uniform-continuity.md) of each path of the [continuous local martingale](../../../../../../continuous-local-martingale.md) on $[0,T+1]$, its modulus

$$
\eta_n=\sup_{\substack{u,v\in[0,T+1]\\|u-v|\le h_n}}|X_u-X_v|
$$

tends to zero [almost surely](../../../../../../almost-sure-convergence.md). For every $s\le T$, comparison of powers of each increment gives

$$
V_s^{n,|\cdot|^p}\le\eta_n^{p-2}V_T^{n,|\cdot|^2}.
$$

The squared-increment sum converges in [probability](../../../../../../probability.md) to $[X]_T$, by the dyadic definition of [quadratic variation](../../../../../../quadratic-variation.md). Including the last full grid interval instead of the last partial interval changes that sum by a quantity bounded by $2\eta_n^2$, so the ceiling convention has the same limit. In particular these squared-increment sums are bounded in [probability](../../../../../../probability.md).

Since $p-2>0$, a quantity tending to zero [almost surely](../../../../../../almost-sure-convergence.md) multiplied by a family bounded in [probability](../../../../../../probability.md) tends to zero in [probability](../../../../../../probability.md). Hence

$$
\boxed{\sup_{s\le T}V_s^{n,|\cdot|^p}\xrightarrow{\mathbb P}0\quad\text{for every }T<\infty.}
$$

This is [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md), and proves the superquadratic case of [dyadic power variation of a continuous local martingale](../../../../../../dyadic-power-variation-of-a-continuous-local-martingale.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
