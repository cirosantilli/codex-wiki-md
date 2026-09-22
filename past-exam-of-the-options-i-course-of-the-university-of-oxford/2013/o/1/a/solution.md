<h1 id="o/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $S=\sum_{j=1}^n|X_j|$. The [log-likelihood](../../../../../log-likelihood.md) for the [Laplace distribution](../../../../../laplace-distribution.md) is

$$
\ell(\theta)=-n\log(2\theta)-S/\theta,\qquad\ell'(\theta)=-n/\theta+S/\theta^2.
$$

For $S>0$ the derivative is positive for $\theta<S/n$ and negative for $\theta>S/n$, so the unique [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta=\frac1n\sum_{j=1}^n|X_j|.}
$$

The exceptional data set $S=0$ has [probability](../../../../../probability.md) zero; there the likelihood has its supremum at the excluded boundary $\theta=0$. For the [Fisher information](../../../../../fisher-information-matrix.md), $|X_j|$ has exponential density $\theta^{-1}e^{-y/\theta}$ for $y>0$, hence mean $\theta$. Since $\ell''(\theta)=n/\theta^2-2S/\theta^3$,

$$
\boxed{I_n(\theta)=-\mathbb E_\theta\ell''(\theta)=\frac n{\theta^2}.}
$$

This also follows from the score [variance](../../../../../variance-split.md), because $\operatorname{Var}(S)=n\theta^2$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [O](../../../o.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
