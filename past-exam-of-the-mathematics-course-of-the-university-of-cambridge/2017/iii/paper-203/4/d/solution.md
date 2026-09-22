<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Before the [Loewner swallowing time](../../../../../../interior-point-swallowing-time-for-a-loewner-chain.md) $T_z$, put $Z_t=g_t(z)-U_t=X_t+iY_t$ and $\theta_t=\arg Z_t\in(0,\pi)$. The [Itô formula](../../../../../../ito-s-lemma.md) applied to the [holomorphic logarithm](../../../../../../holomorphic-logarithm.md) in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) gives

$$
d\log Z_t=\frac{2-\kappa/2}{Z_t^2}\,dt-\frac{\sqrt\kappa}{Z_t}\,dB_t.
$$

Taking imaginary parts yields the [SLE angle process](../../../../../../sle-angle-process.md)

$$
d\theta_t=(\kappa-4)\frac{X_tY_t}{|Z_t|^4}\,dt+\sqrt\kappa\frac{Y_t}{|Z_t|^2}\,dB_t.
$$

For $\kappa=4$ the drift vanishes, so

$$
\boxed{\theta_t=\arg z+2\int_0^t\frac{Y_s}{|Z_s|^2}\,dB_s}
$$

is a continuous [local martingale](../../../../../../local-martingale.md). Since $0<\theta_t<\pi$, every localized stopped version is a bounded true [martingale](../../../../../../martingale-split.md). After resolving the lifetime issue below, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) applied to [conditional expectations](../../../../../../conditional-expectation.md) removes localization and gives a true bounded [martingale](../../../../../../martingale-split.md).

For completeness, there is no finite lifetime ambiguity for a fixed [interior](../../../../../../interior-topology.md) $z$ in this parameter range. The preceding [Bessel process](../../../../../../bessel-process.md) and [Conformal Markov property of SLE](../../../../../../conformal-markov-property-of-sle.md) argument gives a simple trace staying in the [interior](../../../../../../interior-topology.md), so no point is swallowed in a disconnected pocket. If $T_z$ were finite, the trace would have to reach $z$, forcing the [Loewner conformal radius](../../../../../../conformal-radius-under-a-chordal-loewner-flow.md) to tend to zero by the [Koebe quarter theorem](../../../../../../koebe-quarter-theorem.md). But

$$
\log\frac{\Upsilon_t}{\Upsilon_0}=-4\int_0^t\frac{Y_s^2}{|Z_s|^4}\,ds=-[\theta]_t.
$$

The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) says that a bounded continuous [local martingale](../../../../../../local-martingale.md) cannot have infinite [quadratic variation](../../../../../../quadratic-variation.md) before a finite terminal time: that would require a [Brownian motion](../../../../../../brownian-motion-split.md) to stay in a bounded interval for all clock times. Therefore $\Upsilon_t$ cannot tend to zero at a finite $T_z$, a contradiction. Thus $T_z=\infty$ almost surely for each fixed $z$. This proves the [SLE4 angle martingale](../../../../../../sle4-angle-martingale.md) assertion: **the angle is a bounded continuous [martingale](../../../../../../martingale-split.md)**. In particular $\mathbb E[\theta_t]=\arg z$. The upper-half-plane branch of the argument is used throughout.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
