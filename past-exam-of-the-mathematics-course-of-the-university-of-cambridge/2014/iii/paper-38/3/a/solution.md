<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [discount factor](../../../../../../discount-factor.md) as $D_t=B_t^{-1}=\exp(-\int_0^t r_sds)$. Splitting the time integral at $t$ gives

$$
\frac{P(t,T)}{B_t}
=\mathbb E^{\mathbb Q}[D_T\mid\mathcal F_t].
$$

The random variable $D_T$ lies in $(0,1]$ because the [short rate](../../../../../../short-rate.md) is nonnegative and continuous on the finite maturity interval. A process of [conditional expectations](../../../../../../conditional-expectation.md) of an [integrable](../../../../../../integrability.md) terminal variable is a [martingale](../../../../../../martingale-split.md), by the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md). Therefore

$$
\boxed{D_tP(t,T)\text{ is a bounded }\mathbb Q\text{-martingale}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
