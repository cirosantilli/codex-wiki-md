<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Exponential martingale for Brownian motion](../../../../../../exponential-martingale-for-brownian-motion.md) is a true [martingale](../../../../../../martingale-split.md): independent increments and the [normal distribution](../../../../../../normal-distribution.md) identity $\mathbb E e^{aN}=e^{a^2v/2}$ for $N\sim N(0,v)$ give $\mathbb E[Z_t\mid\mathcal F_s]=Z_s$. Its second moment is

$$
\mathbb E Z_t^2=e^{\mu^2t},\qquad
\boxed{\sup_{0\leq t\leq T}\mathbb E Z_t^2=e^{\mu^2T}<\infty.}
$$

The [uniform integrability from bounded second moments](../../../../../../uniform-integrability-from-bounded-second-moments.md) criterion now applies: for $K>0$,

$$
\sup_{t\leq T}\mathbb E[Z_t\mathbf1_{\{Z_t>K\}}]\leq\frac{e^{\mu^2T}}K\longrightarrow0.
$$

Thus $\{Z_t:0\leq t\leq T\}$ has [uniform integrability](../../../../../../uniform-integrability.md). In fact, all values stopped at [stopping times](../../../../../../stopping-time.md) bounded by $T$ have [uniform integrability](../../../../../../uniform-integrability.md), since $Z_\tau=\mathbb E[Z_T\mid\mathcal F_\tau]$ and [uniform integrability of conditional expectations](../../../../../../uniform-integrability-of-conditional-expectations.md) applies. This is a finite-horizon assertion, not an assertion of [uniform integrability](../../../../../../uniform-integrability.md) over all $t\geq0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
