<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Conditional on $\theta$, the future [Bernoulli random variable](../../../../../bernoulli-distribution.md) is independent of the observed [statistical sample](../../../../../statistical-sample.md) and has success [probability](../../../../../probability.md) $\theta$. Its [posterior predictive probability](../../../../../posterior-predictive-probability.md) is therefore the [posterior mean](../../../../../posterior-mean.md) of $\theta$. Put $A=a+s$ and $B=b+n-s$. Then

$$
\begin{aligned}
\mathbb P(X_{n+1}=1\mid x)
&=\int_0^1\theta\,\pi(\theta\mid x)\,d\theta\\
&=\frac{B(A+1,B)}{B(A,B)}
=\frac{\Gamma(A+1)\Gamma(A+B)}{\Gamma(A)\Gamma(A+B+1)}
=\frac A{A+B},
\end{aligned}
$$

using the [beta-gamma identity](../../../../../beta-gamma-identity.md) and the [Gamma function recurrence](../../../../../gamma-function-recurrence.md). Hence

$$
\boxed{\mathbb P(X_{n+1}=1\mid X_1,\ldots,X_n)=\frac{a+\sum_iX_i}{a+b+n}.}
$$

The whole [posterior predictive distribution](../../../../../posterior-predictive-distribution.md) of $X_{n+1}$ is the [Bernoulli distribution](../../../../../bernoulli-distribution.md) with this success [probability](../../../../../probability.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
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
