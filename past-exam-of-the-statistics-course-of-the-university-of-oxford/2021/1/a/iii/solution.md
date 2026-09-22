<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $A=-\sum_i\log X_i>0$, with $\log$ the [natural logarithm](../../../../../natural-logarithm.md). The [likelihood function](../../../../../likelihood-function.md) and [log-likelihood function](../../../../../log-likelihood.md) are

$$
L(\theta)=\theta^n\exp\{-(\theta-1)A\},\qquad
\ell(\theta)=n\log\theta-(\theta-1)A.
$$

The [score function](../../../../../informant-function.md) is $\ell'(\theta)=n/\theta-A$ and the second [derivative](../../../../../derivative.md) is $\ell''(\theta)=-n/\theta^2<0$. Thus the [log-likelihood function](../../../../../log-likelihood.md) is strictly [concave](../../../../../concave-function.md), its stationary point is the unique global maximum, and the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{T_2=\widehat\theta=\frac nA=-\frac n{\sum_i\log X_i}}.
$$

The one-observation [Fisher information](../../../../../fisher-information-matrix.md) is $I(\theta)=1/\theta^2$. The [support of a probability distribution](../../../../../support-of-a-probability-distribution.md) here is independent of $\theta>0$, so the regular [asymptotic normality of a maximum likelihood estimator](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) gives

$$
\boxed{\sqrt n(T_2-\theta)\xrightarrow dN(0,\theta^2)},\qquad
T_2\ \mathrel{\dot\sim}\ N(\theta,\theta^2/n),\qquad v(T_2)=\theta^2/n.
$$

There is also a direct check: $U_i=-\log X_i$ has an [exponential distribution](../../../../../exponential-distribution.md) with rate $\theta$, since $\mathbb P(U_i>u)=\mathbb P(X_i<e^{-u})=e^{-\theta u}$ for $u>0$. Its [mean](../../../../../expected-value-split.md) and [variance](../../../../../variance-split.md) are $1/\theta$ and $1/\theta^2$. Apply the [central limit theorem](../../../../../central-limit-theorem.md) to $A/n$ and the [delta method](../../../../../delta-method.md) to $h(u)=1/u$ to obtain the same result.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
