<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a parametric baseline hazard $h_0(t;\eta)$ and fit

$$
h(t\mid z)=h_0(t;\eta)e^{\beta z}.
$$

Under independent [right censoring](../../../../../../right-censoring.md), the full [survival likelihood](../../../../../../survival-likelihood.md) is

$$
L(\eta,\beta)=\prod_{i=1}^n
\bigl[h_0(x_i;\eta)e^{\beta z_i}\bigr]^{v_i}
\exp\!\left[-H_0(x_i;\eta)e^{\beta z_i}\right].
$$

Estimate $(\eta,\beta)$ by [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) and test $H_0:\beta=0$ with a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md), [Wald test](../../../../../../wald-test.md), or [score test](../../../../../../score-test.md). Equality of the two event-time distributions is exactly $\beta=0$ within this model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
