<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expanding the exponent, the [log-likelihood function](../../../../../log-likelihood.md) is

$$
\ell(\theta)=C-\frac{\sum_i y_i}{2\theta^2}+\frac n\theta,
$$

where $C$ is independent of $\theta$. Its [score function](../../../../../informant-function.md) and second derivative are

$$
\ell'(\theta)=\frac{\sum_i y_i-n\theta}{\theta^3},\qquad
\ell''(\theta)=-\frac{3\sum_i y_i}{\theta^4}+\frac{2n}{\theta^3}.
$$

The first is positive below $\bar y$ and negative above it, so the unique [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta=\bar Y}.
$$

Using $\mathbb E\sum_iY_i=n\theta$, the one-observation [Fisher information](../../../../../fisher-information-matrix.md) is $I(\theta)=-n^{-1}\mathbb E\ell''(\theta)=\theta^{-3}$. The support does not depend on the interior parameter $\theta>0$, and the regular [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) gives

$$
\boxed{\sqrt n(\widehat\theta-\theta)\xrightarrow d N(0,\theta^3)},\qquad
\widehat\theta\ \mathrel{\dot\sim}\ N(\theta,\theta^3/n).
$$

This is [Inverse Gaussian mean estimation](../../../../../inverse-gaussian-mean-estimation.md) with known shape one. Equivalently, the [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md) has [variance](../../../../../variance-split.md) $\theta^3$, so the same result follows directly from the [central limit theorem](../../../../../central-limit-theorem.md) applied to its [sample mean](../../../../../sample-mean.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
