<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [beta distribution](../../../../../beta-distribution.md) with parameters $(\theta,1)$, the [Euler beta function](../../../../../beta-function.md) gives $B(\theta,1)=1/\theta$. Its [probability density function](../../../../../probability-density-function.md) is therefore $\theta x^{\theta-1}$ on $(0,1)$. Direct [integration](../../../../../integral-split.md) gives the [raw moments](../../../../../raw-moment.md)

$$
\mathbb E_\theta X^r=\theta\int_0^1x^{\theta+r-1}\,dx=\frac{\theta}{\theta+r},\qquad r> -\theta.
$$

In particular, its [mean](../../../../../expected-value-split.md) is $\mu(\theta)=\theta/(\theta+1)$. Equating this to the [sample mean](../../../../../sample-mean.md) and rearranging gives

$$
\theta=\bar X(1+\theta),\qquad
\boxed{T_1=\frac{\bar X}{1-\bar X}}.
$$

The observations lie strictly between zero and one with [probability](../../../../../probability.md) one, so $0<\bar X<1$ and this [method of moments](../../../../../method-of-moments-statistics.md) [estimator](../../../../../estimator.md) is well defined and positive. This is an instance of [estimation of a beta shape parameter](../../../../../estimation-of-a-beta-shape-parameter.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
