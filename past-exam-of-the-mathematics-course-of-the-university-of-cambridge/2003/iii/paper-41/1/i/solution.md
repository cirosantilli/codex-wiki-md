<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the mean parameter $\theta=1/\lambda>0$, the [log-likelihood](../../../../../../log-likelihood.md) is $\ell(\theta)=-n\log\theta-\sum_iY_i/\theta$. Its derivative is $n(\bar Y-\theta)/\theta^2$, positive below $\bar Y$ and negative above it. Therefore $\boxed{\widehat\theta=\bar Y}$ is the unique [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md).

The [exponential distribution](../../../../../../exponential-distribution.md) has mean $\theta$ and [variance](../../../../../../variance-split.md) $\theta^2$. The [central limit theorem](../../../../../../central-limit-theorem.md) gives the pivot

$$
T_n=\sqrt n\,\frac{\bar Y-\theta}{\theta}\ \Rightarrow\ N(0,1).
$$

Let $z=\Phi^{-1}(1-\alpha/2)$ for fixed $0<\alpha<1$. For $n>z^2$, the event $-z<T_n<z$ is exactly

$$
\frac{\bar Y}{1+z/\sqrt n}<\theta<\frac{\bar Y}{1-z/\sqrt n}.
$$

Both denominators are then positive, so the algebra neither reverses the ordering nor changes the parameter domain. Taking probabilities and using continuity of the limiting normal distribution proves the [exponential-mean confidence interval by pivot inversion](../../../../../../exponential-mean-confidence-interval-by-pivot-inversion.md) has [coverage probability](../../../../../../coverage-probability.md) tending to $\boxed{1-\alpha}$. This is inversion of the pivot with the true mean in its denominator; it is not the ordinary symmetric Wald interval centered at $\bar Y$. For a small sample with $n\leq z^2$, the displayed finite positive upper endpoint is not valid, although the large-sample claim is unaffected.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
