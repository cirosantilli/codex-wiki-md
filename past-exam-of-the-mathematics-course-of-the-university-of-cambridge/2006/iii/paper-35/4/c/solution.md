<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $\widetilde{\mathbb P}$ for the reference measure under which $X$ is a [Brownian motion](../../../../../../brownian-motion-split.md). Pathwise, $B_t=X_t-\int_0^tX_sds$. Put $h_s=X_s\mathbf1_{\{s\le T\}}$ and define

$$
Z_t=\exp\left(\int_0^{t\wedge T}X_s\,dX_s-\frac12\int_0^{t\wedge T}X_s^2ds\right).
$$

The stopped integrand has absolute value at most one. The [Novikov condition](../../../../../../novikov-s-condition.md) holds on every finite horizon, so $Z$ is a density [martingale](../../../../../../martingale-split.md). The [Itô formula](../../../../../../ito-s-lemma.md) also gives the more useful identity

$$
\boxed{Z_t=\exp\left(\frac12X_{t\wedge T}^2-\frac12(t\wedge T)
-\frac12\int_0^{t\wedge T}X_s^2ds\right)\le e^{1/2}.}
$$

Thus $Z$ is [uniformly integrable](../../../../../../uniform-integrability.md) over the entire time axis, not just a true [martingale](../../../../../../martingale-split.md) on each finite horizon. Under the reference measure, $\widetilde{\mathbb E}(t\wedge T)=\widetilde{\mathbb E}X_{t\wedge T}^2\le1$, so $T<\infty$ almost surely. Hence $Z_t\to Z_T>0$ and $\widetilde{\mathbb E}Z_T=1$.

Define the [probability measure](../../../../../../probability-measure.md) on the original [sigma-algebra](../../../../../../sigma-algebra.md) by

$$
\boxed{\frac{d\mathbb P}{d\widetilde{\mathbb P}}=Z_T.}
$$

Its restriction to $\mathcal F_t$ has density $Z_t$. The [Girsanov theorem](../../../../../../girsanov-theorem.md) states that subtracting the integrated density integrand from the reference [Brownian motion](../../../../../../brownian-motion-split.md) gives a [Brownian motion](../../../../../../brownian-motion-split.md) under the new measure. Therefore

$$
W_t^{\mathbb P}=X_t-\int_0^{t\wedge T}X_sds
$$

is a [Brownian motion](../../../../../../brownian-motion-split.md) under $\mathbb P$, and $B_{t\wedge T}=W^{\mathbb P}_{t\wedge T}$. This is exactly the requested Brownian property until $T$. The [bounded Girsanov density for exit of an unstable linear diffusion](../../../../../../bounded-girsanov-density-for-exit-of-an-unstable-linear-diffusion.md) also proves global absolute continuity, so a mere collection of unspecified finite-horizon measures is unnecessary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
