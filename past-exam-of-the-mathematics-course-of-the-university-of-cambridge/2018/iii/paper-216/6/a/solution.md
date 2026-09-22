<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $h(\beta)=\Phi(x_{\mathrm{test}}^T\beta)$. To distinguish the number of posterior draws from the training-sample size, write it as $N$; in the question's sample notation $N=n$. The [Monte Carlo estimator](../../../../../../monte-carlo-estimator.md) of the requested [posterior mean](../../../../../../posterior-mean.md) is

$$
\boxed{\widehat\mu_N=\frac1N\sum_{j=1}^N\Phi(x_{\mathrm{test}}^T\beta^{(j)}).}
$$

For independent exact posterior draws it is unbiased, and

$$
\operatorname{Var}(\widehat\mu_N)=\frac1N\operatorname{Var}(h(\beta)\mid Y).
$$

The features are conditioned on as fixed data. The estimated probability concerns a future genuine banknote under the [posterior predictive probability](../../../../../../posterior-predictive-probability.md), not an indicator sampled from that predictive distribution.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
