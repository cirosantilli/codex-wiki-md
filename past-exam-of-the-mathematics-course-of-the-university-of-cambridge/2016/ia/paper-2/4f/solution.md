<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The [moment-generating function](../../../../../moment-generating-function.md) of a [random variable](../../../../../random-variable-split.md) $Z$ is $m_Z(\theta)=\mathbb E[e^{\theta Z}]$, at the real values of $\theta$ for which that [expectation](../../../../../expected-value.md) is finite. For a [standard normal distribution](../../../../../standard-normal-distribution.md) variable $X$, combining the exponentials in its [probability density function](../../../../../probability-density-function.md) yields

$$
\mathbb E[e^{\theta X^2}]=\frac1{\sqrt{2\pi}}\int_{-\infty}^{\infty}e^{-(1-2\theta)x^2/2}\,dx=(1-2\theta)^{-1/2},\qquad \theta<\tfrac12.
$$

The last equality follows by scaling the [Gaussian integral](../../../../../gaussian-integral.md). The variables $X_i^2$ are [independent random variables](../../../../../independent-random-variables.md), so the [expectation](../../../../../expected-value.md) of their product factorizes. Therefore

$$
\boxed{m_Z(\theta)=\prod_{i=1}^n\mathbb E[e^{\theta X_i^2}]=(1-2\theta)^{-n/2},\qquad \theta<\tfrac12.}
$$

This is the [moment-generating function of a chi-squared distribution](../../../../../moment-generating-function-of-a-chi-squared-distribution.md) with $n$ degrees of freedom. For positive $n$ the defining [integral](../../../../../integral.md) diverges at and above $\theta=1/2$.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
