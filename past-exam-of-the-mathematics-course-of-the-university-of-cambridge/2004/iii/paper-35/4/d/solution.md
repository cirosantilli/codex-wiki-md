<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Three useful methods are [antithetic variates](../../../../../../antithetic-variates.md), a [control variate](../../../../../../control-variates.md), and [stratified sampling](../../../../../../stratified-sampling.md). Their purpose is to reduce sampling [variance](../../../../../../variance-split.md) at comparable computational cost, rather than merely to take more samples.

For [antithetic variates](../../../../../../antithetic-variates.md), generate independent pairs $(U,1-U)$ and average both payoffs. Since the call integrand is increasing, the two values have nonpositive [covariance](../../../../../../covariance.md). Indeed, for an independent copy $U'$, twice that covariance is the expectation of $[g(U)-g(U')][g(1-U)-g(1-U')]$, which is nonpositive pointwise. With $N=2m$ evaluations, the paired average has [variance](../../../../../../variance-split.md)

$$
\frac{\operatorname{Var}(g(U))+\operatorname{Cov}(g(U),g(1-U))}{N}\leq\frac{\operatorname{Var}(g(U))}{N}.
$$

For a [control variate](../../../../../../control-variates.md), use the same simulated discounted stock value $Y=e^{-r\tau}S_T$, whose known mean is $S$. Replace the discounted call payoff $H$ by $H-\beta(Y-S)$, preserving its mean. Minimizing its quadratic variance gives

$$
\beta^*=\frac{\operatorname{Cov}(H,Y)}{\operatorname{Var}(Y)},\qquad
\operatorname{Var}(H-\beta^*(Y-S))=\operatorname{Var}(H)(1-\operatorname{Corr}(H,Y)^2).
$$

A predetermined coefficient or an independent pilot estimate preserves exact unbiasedness; fitting the coefficient from the same observations requires care.

For [stratified sampling](../../../../../../stratified-sampling.md), divide $[0,1]$ into $q$ equal intervals, sample independently and uniformly within each, and average their $q$ payoffs. If $v_j$ is the conditional [variance](../../../../../../variance-split.md) in interval $j$, this unbiased estimator has [variance](../../../../../../variance-split.md) $q^{-2}\sum_jv_j$. The [law of total variance](../../../../../../law-of-total-variance.md) gives $\operatorname{Var}(H)\geq q^{-1}\sum_jv_j$, so this is at most the [variance](../../../../../../variance-split.md) $\operatorname{Var}(H)/q$ of $q$ ordinary independent samples. Stratification removes randomness in how many samples fall in each region, which is particularly valuable when conditional payoff means vary strongly.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
