<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S=\sum_iX_i$. For the [exponential distribution](../../../../exponential-distribution.md) with [mean](../../../../expected-value-split.md) $\theta$, the [likelihood function](../../../../likelihood-function.md) is $L(\theta)=\theta^{-n}e^{-S/\theta}$ on positive observations. Fix any $0<\theta_1<\theta_0$. The alternative-to-null [likelihood ratio](../../../../likelihood-ratio.md) is

$$
\frac{L(\theta_1)}{L(\theta_0)}
=\left(\frac{\theta_0}{\theta_1}\right)^n
\exp\!\left\{-\left(\frac1{\theta_1}-\frac1{\theta_0}\right)S\right\}.
$$

Since $1/\theta_1-1/\theta_0>0$, this is strictly decreasing in $S$. The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) says to reject for small $S$. Under the [null hypothesis](../../../../null-hypothesis.md), the given sum rule yields $S\sim\operatorname{Gamma}(n,1/\theta_0)$, where the second argument is a rate, and hence

$$
\frac{2S}{\theta_0}\sim\chi^2_{2n}.
$$

Let $q_\alpha$ be the lower $\alpha$ [quantile](../../../../quantile-function.md) of this [chi-squared distribution](../../../../chi-squared-distribution.md). The required [critical region](../../../../rejection-region.md) is

$$
\boxed{\frac{2\sum_iX_i}{\theta_0}<q_\alpha,\qquad
q_\alpha=F^{-1}_{\chi^2_{2n}}(\alpha).}
$$

Its [test size](../../../../size-of-a-statistical-test.md) is exactly $\alpha$ because the [null distribution](../../../../null-distribution.md) is continuous. Its cutoff is the same for every $\theta_1<\theta_0$, so it is simultaneously most powerful against every such value: it is a [uniformly most powerful test](../../../../uniformly-most-powerful-test.md). Equivalently, reject if $S$ is below the lower $\alpha$ [quantile](../../../../quantile-function.md) of the specified [gamma distribution](../../../../gamma-distribution.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
