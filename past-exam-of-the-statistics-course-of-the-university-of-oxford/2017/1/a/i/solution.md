<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [independent](../../../../../independent-random-variables.md) [statistical sample](../../../../../statistical-sample.md), write the [likelihood function](../../../../../likelihood-function.md) and [log-likelihood function](../../../../../log-likelihood.md) as

$$
L_n(\theta)=\prod_{i=1}^nf(X_i;\theta),\qquad
\ell_n(\theta)=\sum_{i=1}^n\log f(X_i;\theta).
$$

The expected [Fisher information](../../../../../fisher-information-matrix.md) in the whole [statistical sample](../../../../../statistical-sample.md) is

$$
\boxed{I_n(\theta)=\mathbb E_\theta\!\left[\left\{\frac{\partial\ell_n(\theta)}{\partial\theta}\right\}^2\right]
=nI_1(\theta),\qquad
I_1(\theta)=\int\left\{\partial_\theta\log f(x;\theta)\right\}^2 f(x;\theta)\,dx.}
$$

Under the regularity conditions that permit [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md), the [score function](../../../../../informant-function.md) has [expected value](../../../../../expected-value-split.md) zero and

$$
I_n(\theta)=-\mathbb E_\theta\ell_n''(\theta).
$$

For an interior [statistical parameter](../../../../../statistical-parameter.md), assuming [identifiability](../../../../../identifiability.md) and $0<I_1(\theta)<\infty$, the regular [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) states

$$
\boxed{\sqrt n(\widehat\theta_n-\theta)\xrightarrow dN\!\left(0,I_1(\theta)^{-1}\right).}
$$

Thus the large-sample [normal approximation](../../../../../normal-approximation.md) is $\widehat\theta_n\mathrel{\dot\sim}N(\theta,I_n(\theta)^{-1})$. The inverse information is the leading sampling [variance](../../../../../variance-split.md) approximation; the displayed convergence specifies its precise asymptotic meaning.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
