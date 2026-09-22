<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the [gamma distribution](../../../../gamma-distribution.md) uses a rate [statistical parameter](../../../../statistical-parameter.md) $\theta$, with known shape $\lambda$. Write $S=\sum_iX_i$ and $a=n\lambda$. For each fixed $\theta_1>\theta_0$, the alternative-to-null [likelihood ratio](../../../../likelihood-ratio.md) is

$$
\frac{L(\theta_1)}{L(\theta_0)}
=\left(\frac{\theta_1}{\theta_0}\right)^a
\exp\{-(\theta_1-\theta_0)S\},
$$

strictly decreasing in $S$. The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) therefore gives the same lower-tail [critical region](../../../../rejection-region.md) $S<c_\alpha$ for every larger rate. Since $S$ has a continuous [gamma distribution](../../../../gamma-distribution.md) under the [null hypothesis](../../../../null-hypothesis.md), there is a unique positive $c_\alpha$ satisfying

$$
\mathbb P_{\theta_0}(S<c_\alpha)=\alpha.
$$

Thus **reject when $S<c_\alpha$** is a [uniformly most powerful test](../../../../uniformly-most-powerful-test.md) of exact [test size](../../../../size-of-a-statistical-test.md) $\alpha$. If $G_a$ denotes the unit-rate [gamma distribution](../../../../gamma-distribution.md) [cumulative distribution function](../../../../cumulative-distribution-function.md) with shape $a$, then

$$
c_\alpha=\frac{G_a^{-1}(\alpha)}{\theta_0},\qquad
\pi(\theta)=G_a(\theta c_\alpha).
$$

This is the [uniformly most powerful test for a gamma rate](../../../../uniformly-most-powerful-test-for-a-gamma-rate.md).

When $\lambda=1/n$, the sum has shape one and hence an [exponential distribution](../../../../exponential-distribution.md) with rate $\theta$. Therefore

$$
1-e^{-\theta_0c_\alpha}=\alpha,\qquad
\boxed{c_\alpha=-\frac{\log(1-\alpha)}{\theta_0}},\qquad
\boxed{\pi(\theta)=1-(1-\alpha)^{\theta/\theta_0}}.
$$

In particular $\pi(\theta_0)=\alpha$, and the [power function](../../../../power-function-of-a-statistical-test.md) is strictly increasing, exceeding $\alpha$ for $\theta>\theta_0$ and tending to one as $\theta\to\infty$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
