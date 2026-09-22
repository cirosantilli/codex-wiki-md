<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $X_0=x$ and a finite horizon $T$. Begin under [Wiener measure](../../../../../../wiener-measure.md) $\mathbb P$ with $X_t=x+W_t$, and let $K$ bound $|b|$. The bounded [progressively measurable process](../../../../../../progressive-measurability.md) $b(X)$ is an admissible [Itô integral](../../../../../../ito-integral.md) integrand. Put

$$
Z_T=\exp\left\{\int_0^T b(X_s)\,dW_s-\frac12\int_0^T b(X_s)^2ds\right\}.
$$

The [Novikov condition](../../../../../../novikov-s-condition.md) follows from $\int_0^T b(X_s)^2ds\leq K^2T$. With $d\mathbb Q=Z_Td\mathbb P$, the [Girsanov theorem](../../../../../../girsanov-theorem.md) says that $B=W-\int_0^\cdot b(X_s)ds$ is [Brownian motion](../../../../../../brownian-motion-split.md). Therefore **a [weak stochastic solution](../../../../../../weak-solution-of-a-stochastic-differential-equation.md) exists**, since

$$
\boxed{X_t=x+B_t+\int_0^t b(X_s)ds.}
$$

Consistent finite-horizon densities on canonical continuous path space give a solution for all finite times. No uniform integrability at infinite time is needed for this extension.

For **[uniqueness in law](../../../../../../uniqueness-in-law.md)**, take any [weak stochastic solution](../../../../../../weak-solution-of-a-stochastic-differential-equation.md) under a measure $\mathbb Q$ and reverse the [change of measure](../../../../../../change-of-measure.md):

$$
R_T=\exp\left\{-\int_0^T b(X_s)\,dB_s-\frac12\int_0^T b(X_s)^2ds\right\},\qquad d\mathbb P=R_Td\mathbb Q.
$$

Again the [Novikov condition](../../../../../../novikov-s-condition.md) holds. Under $\mathbb P$, $W=B+\int b(X_s)ds=X-x$ is [Brownian motion](../../../../../../brownian-motion-split.md), so the law of $X$ is the fixed shifted [Wiener measure](../../../../../../wiener-measure.md). Substitution of $dB=dX-b(X)dt$ gives

$$
\boxed{R_T^{-1}=\exp\left\{\int_0^T b(X_s)\,dX_s-\frac12\int_0^T b(X_s)^2ds\right\}.}
$$

Under shifted [Wiener measure](../../../../../../wiener-measure.md), the [stochastic integral](../../../../../../stochastic-integral.md) on the right has a fixed [measurable](../../../../../../measurability.md) version as a functional of the canonical path. It can be defined by [simple predictable processes](../../../../../../simple-predictable-process.md) converging in the integrand $L^2$ norm and an almost surely convergent subsequence of their integrals. Equivalence of the two finite-horizon measures preserves that version. Thus for every bounded [measurable](../../../../../../measurability.md) path functional $F$,

$$
\mathbb E_{\mathbb Q}F(X)=\mathbb E_{\text{shifted Wiener measure}}\left[F(X)\exp\left\{\int_0^T b(X_s)dX_s-\tfrac12\int_0^T b(X_s)^2ds\right\}\right].
$$

The right-hand side depends only on $b,x,T$, not on the chosen solution. This proves [uniqueness in law](../../../../../../uniqueness-in-law.md) on every finite horizon, and hence on the whole continuous path space. This is [Weak existence and uniqueness in law for an additive-noise SDE with bounded drift](../../../../../../weak-existence-and-uniqueness-in-law-for-an-additive-noise-sde-with-bounded-drift.md). For merely [measurable](../../../../../../measurability.md) $b$, one should not assume that naive deterministic left-endpoint samples of $b(X)$ converge; the predictable $L^2$ approximation is the appropriate definition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
