<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the predictable process

$$
\theta_s=\frac{\nu_s-\mu_s}{\sigma_s}\mathbf1_{[0,T]}(s),\qquad L_t=\int_0^t\theta_s\,dB_s.
$$

The value at zero is irrelevant to the Brownian integral. The numerator is bounded and $\sigma_s\geq\delta>0$, so $\theta$ is bounded and $[L]_\infty=\int_0^T\theta_s^2ds$ has a deterministic bound. Part (a) supplies a [uniformly integrable](../../../../../../uniform-integrability.md) density [martingale](../../../../../../martingale-split.md). Define a measure on the entire given sigma-algebra by

$$
\boxed{\mathbb Q(A)=\mathbb E_{\mathbb P}\left[\mathbf1_A\exp\left(\int_0^T\frac{\nu_s-\mu_s}{\sigma_s}\,dB_s-\frac12\int_0^T\left(\frac{\nu_s-\mu_s}{\sigma_s}\right)^2ds\right)\right],\quad A\in\mathcal F.}
$$

Its density is positive and has [expectation](../../../../../../expected-value.md) one, so $\mathbb Q$ is a probability measure equivalent to $\mathbb P$. The [Girsanov theorem](../../../../../../girsanov-theorem.md) makes $\widetilde B_t=B_t-\int_0^{t\wedge T}(\nu_s-\mu_s)/\sigma_s\,ds$ a [Brownian motion](../../../../../../brownian-motion-split.md) under $\mathbb Q$. For $t\leq T$, substitute $dB=d\widetilde B+\theta\,dt$:

$$
\boxed{X_t=\int_0^t\nu_s\,ds+\int_0^t\sigma_s\,d\widetilde B_s.}
$$

Continuity of $\sigma$ gives pathwise local square integrability, even though it is not assumed bounded. Equivalence preserves this property. This is [finite-horizon drift replacement by a change of measure](../../../../../../finite-horizon-drift-replacement-by-a-change-of-measure.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
