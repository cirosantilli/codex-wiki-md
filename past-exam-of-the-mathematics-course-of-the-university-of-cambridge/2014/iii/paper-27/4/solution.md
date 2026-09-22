<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Since the density [martingale](../../../../../martingale-split.md) is [uniformly integrable](../../../../../uniform-integrability.md), $Z_t=\mathbb E_{\mathbb P}[Z_\infty\mid\mathcal F_t]$. Equivalence of measures, as stipulated, means $Z_\infty>0$ almost surely. Write $L=\int Z^{-1}\,dZ$ for the [stochastic logarithm](../../../../../stochastic-logarithm.md). The [Itô formula](../../../../../ito-s-lemma.md) gives $\log Z=L-\langle L\rangle/2$, and hence the [quadratic covariation](../../../../../quadratic-covariation.md) in the drift correction is

$$
C_t=\langle\log Z,X\rangle_t=\int_0^t Z_s^{-1}\,d\langle Z,X\rangle_s.
$$

It involves the local-[martingale](../../../../../martingale-split.md) part of $\log Z$; its continuous finite-variation part has zero covariation.

With $Y=X-C$, the [Itô product rule](../../../../../ito-product-rule.md) now gives an exact cancellation:

$$
d(ZY)=Y\,dZ+Z\,dX-Z\,dC+d\langle Z,X\rangle=Y\,dZ+Z\,dX.
$$

Thus $ZY$ is a P-[local martingale](../../../../../local-martingale.md). To transfer this conclusion rigorously, set $\tau_n=\inf\{t:|Y_t|\geq n\}$. The same computation for the stopped $Y$ gives

$$
d(Z_tY_{t\wedge\tau_n})=Y_{t\wedge\tau_n}\,dZ_t+\mathbf1_{\{t\leq\tau_n\}}Z_t\,dX_t.
$$

This is again a P-[local martingale](../../../../../local-martingale.md). Moreover its absolute value is at most $nZ_t$. [Uniform integrability](../../../../../uniform-integrability.md) of $Z$ makes the family over bounded [stopping times](../../../../../stopping-time.md) [uniformly integrable](../../../../../uniform-integrability.md), so the product is a true [martingale](../../../../../martingale-split.md). This is the [bounded-process density-product criterion](../../../../../bounded-process-density-product-criterion.md).

The [Bayes formula for conditional expectation](../../../../../bayes-formula-for-conditional-expectation.md) therefore gives, for $s\leq t$,

$$
\mathbb E_{\mathbb Q}[Y_{t\wedge\tau_n}\mid\mathcal F_s]
=\frac{\mathbb E_{\mathbb P}[Z_tY_{t\wedge\tau_n}\mid\mathcal F_s]}{Z_s}
=Y_{s\wedge\tau_n}.
$$

Continuity gives $\tau_n\uparrow\infty$, proving **$X-\langle\log Z,X\rangle$ is a Q-[local martingale](../../../../../local-martingale.md)**. This proves the needed [Girsanov theorem](../../../../../girsanov-theorem.md) rather than invoking it.

For the Brownian-filtration conclusion, use this precise [Brownian martingale representation theorem](../../../../../brownian-martingale-representation-theorem.md): every [continuous local martingale](../../../../../continuous-local-martingale.md) in the usual augmentation of the natural Brownian filtration is an Itô integral with a predictable integrand locally square integrable in time. In particular

$$
Z_t=1+\int_0^tH_s\,dW_s,\qquad\int_0^tH_s^2\,ds<\infty\quad\text{a.s.}
$$

Define

$$
\boxed{\alpha_s=H_s/Z_s.}
$$

On each finite horizon a strictly positive continuous $Z$ has a positive pathwise minimum. Thus $\int_0^t\alpha_s^2\,ds<\infty$ almost surely, and

$$
\langle\log Z,W\rangle_t=\int_0^t\alpha_s\,ds.
$$

The already proved measure-change result makes $\widehat W=W-\int\alpha\,ds$ a continuous Q-[local martingale](../../../../../local-martingale.md). Its [quadratic variation](../../../../../quadratic-variation.md) is $t$, unchanged by its finite-variation correction. The [Lévy characterization of Brownian motion](../../../../../levy-characterization-of-brownian-motion.md) proves

$$
\boxed{\widehat W_t=W_t-\int_0^t\alpha_s\,ds\text{ is Q-Brownian motion}.}
$$

No additional exponential-integrability condition is needed, since the equivalent [uniformly integrable](../../../../../uniform-integrability.md) density process is already given.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
