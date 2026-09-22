<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the preceding argument to the two product observation laws and the real-valued [estimator](../../../../../../estimator.md) $T=\widehat\psi_n$. Alternatively, directly use

$$
(T-\theta)^2+(T-\tau)^2
=2\left(T-\frac{\theta+\tau}{2}\right)^2+\frac{(\theta-\tau)^2}{2}
\geq\frac{(\theta-\tau)^2}{2}.
$$

The average of the two [mean squared errors](../../../../../../mean-squared-error.md) is at least $(\theta-\tau)^2/4$ times the overlap of the two joint [probability density functions](../../../../../../probability-density-function.md). Their overlap equals

$$
\int\min(p_f^{(n)},p_g^{(n)})\,d\mu^{(n)}
=\frac12\int(p_f^{(n)}+p_g^{(n)}-|p_f^{(n)}-p_g^{(n)}|)\,d\mu^{(n)}
=1-\frac12\|P_f^{(n)}-P_g^{(n)}\|_1.
$$

Taking the infimum over [estimators](../../../../../../estimator.md) therefore yields

$$
\boxed{R_n^*\geq\frac{(\theta-\tau)^2}{4}\left(1-\frac12\|P_f^{(n)}-P_g^{(n)}\|_1\right).}
$$

Here $R_n^*$ is the [minimax risk](../../../../../../minimax-risk.md) for this functional. The factor $\frac12\|P_f^{(n)}-P_g^{(n)}\|_1$ is the [total variation distance](../../../../../../total-variation-distance.md), so the same [metric squared-loss two-point bound](../../../../../../metric-squared-loss-two-point-bound.md) applies to a functional even when distinct density parameters have the same functional value.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
