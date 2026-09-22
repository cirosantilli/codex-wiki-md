<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First propagate terminal nonnegativity backwards; it is not necessary to assume nonnegative wealth at intermediate dates. Suppose $Y_t\geq0$ and define

$$
A_j=\{|Y_{t-1}|\leq j,\ |K_t|\leq j\}\in\mathcal F_{t-1}.
$$

These events increase to the whole space up to a null set. On $A_j$, both the old value and the coefficient are bounded, so $\mathbf1_{A_j}Y_t$ is [integrable](../../../../../../integrability.md) and

$$
\mathbb E[\mathbf1_{A_j}Y_t\mid\mathcal F_{t-1}]
=\mathbf1_{A_j}Y_{t-1}.
$$

The left side is nonnegative; hence $Y_{t-1}\geq0$ on every $A_j$, and therefore almost surely. Starting from $t=T$, induction gives $Y_t\geq0$ for every $0\leq t\leq T$.

The process stopped at $T$ is now a nonnegative discrete-time [local martingale](../../../../../../local-martingale.md). Part (b) makes it a [martingale](../../../../../../martingale-split.md) with initial value zero. Consequently $\mathbb E Y_T=0$, and a nonnegative random variable with zero [expectation](../../../../../../expected-value.md) vanishes almost surely:

$$
\boxed{Y_T=0\quad\text{almost surely}.}
$$

This is the [terminal nonnegativity criterion for a finite-horizon martingale transform](../../../../../../terminal-nonnegativity-criterion-for-a-finite-horizon-martingale-transform.md). A finite deterministic horizon is essential to the backward induction.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
