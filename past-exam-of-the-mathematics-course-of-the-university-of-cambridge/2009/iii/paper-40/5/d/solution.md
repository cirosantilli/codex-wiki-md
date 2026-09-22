<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Tune the proposal scale using pilot runs on a grid of candidate $\sigma_q$ values. After allowing for initial transients, compare the [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md) per unit computation time for representative functions, such as both coordinates and a quadratic function. Equivalently inspect their [integrated autocorrelation time](../../../../../../integrated-autocorrelation-time.md), using $\operatorname{ESS}\approx n/(1+2\sum_{k\ge1}\operatorname{Corr}(h(Z_0),h(Z_k)))$. Choose a useful scale and keep it fixed for the production run. Another pilot criterion is the average squared accepted displacement, possibly in coordinates standardized by the target [covariance](../../../../../../covariance.md), which balances move size and rejection.

Acceptance alone is not an efficiency criterion. As $\sigma_q\downarrow0$, proposals are almost the current state, so acceptance tends to one while exploration becomes arbitrarily slow. Very large scales propose mostly low-density states and produce long sequences of identical values. The [proposal scale and random-walk Metropolis efficiency](../../../../../../proposal-scale-and-random-walk-metropolis-efficiency.md) trade-off requires both movement and acceptance; neither maximizing nor merely reporting the acceptance probability guarantees a useful sample. With strong correlation, an isotropic proposal also struggles with the target's narrow direction; [covariance](../../../../../../covariance.md)-scaled proposals can improve this geometry beyond tuning one scalar [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
