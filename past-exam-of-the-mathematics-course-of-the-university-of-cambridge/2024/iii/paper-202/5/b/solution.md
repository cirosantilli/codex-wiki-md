<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work first under [Wiener measure](../../../../../../wiener-measure.md) $P$ with coordinate [Brownian motion](../../../../../../brownian-motion-split.md) $X$. Boundedness of $b$ implies the [Novikov condition](../../../../../../novikov-s-condition.md), so

$$
Z_T=\exp\!\left(\int_0^Tb(X_s)dX_s-\frac12\int_0^Tb(X_s)^2ds\right)
$$

has expectation one. Define $Q$ by $dQ=Z_TdP$. The [Girsanov theorem](../../../../../../girsanov-theorem.md) makes

$$
W_t=X_t-\int_0^tb(X_s)ds
$$

a $Q$-Brownian motion, and hence $(X,W,Q)$ is a [weak solution of a stochastic differential equation](../../../../../../weak-solution-of-a-stochastic-differential-equation.md).

For [uniqueness in law](../../../../../../uniqueness-in-law.md), start with any weak solution under $Q$ and apply the inverse [change of measure](../../../../../../change-of-measure.md) with density $\mathcal E(-\int b(X_s)dW_s)_T$. Boundedness again gives the [Novikov condition](../../../../../../novikov-s-condition.md), and under the resulting measure $P$ the process $X$ is Brownian. Reversing the density expresses the law of $X$ under $Q$ as the same functional $Z_T$ of a Wiener path. It is therefore independent of the chosen weak solution. This proves the [Weak existence and uniqueness in law for an additive-noise SDE with bounded drift](../../../../../../weak-existence-and-uniqueness-in-law-for-an-additive-noise-sde-with-bounded-drift.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
