<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\mu_t=(\mu_t^{(1)},\ldots,\mu_t^{(d)})^T$ and define the market price of risk

$$
\theta_t=\sigma_t^{-1}(\mu_t-r_t\mathbf1).
$$

It is bounded by hypothesis. The stochastic exponential

$$
Z_t=\exp\left(-\int_0^t\theta_s^T dW_s-\frac12\int_0^t|\theta_s|^2ds\right)
$$

is a true martingale by the [Novikov condition](../../../../../../novikov-s-condition.md). Define the equivalent measure $Q$ by $dQ=Z_TdP$. The [Girsanov theorem](../../../../../../girsanov-theorem.md) makes

$$
W_t^Q=W_t+\int_0^t\theta_sds
$$

a Brownian motion under $Q$. After discounting by the bank account, every risky price has zero drift and is a $Q$-local martingale.

The discounted wealth of an admissible self-financing strategy is a nonnegative local martingale and hence a [supermartingale](../../../../../../supermartingale.md). If an arbitrage existed, its zero initial value would imply nonpositive expected terminal discounted wealth under $Q$, while that wealth is nonnegative and positive with positive $Q$-probability. This contradiction proves that the market has no arbitrage; it is the needed direction of the [equivalent local martingale measure](../../../../../../equivalent-local-martingale-measure.md) criterion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
