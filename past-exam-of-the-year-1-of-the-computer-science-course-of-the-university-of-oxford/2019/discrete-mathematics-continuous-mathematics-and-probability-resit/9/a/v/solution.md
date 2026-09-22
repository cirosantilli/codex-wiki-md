<h1 id="9/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

This is the ordinary [factorial](../../../../../../factorial.md) of $X$, rather than a falling-factorial [moment](../../../../../../moment.md). Substituting the [probability mass function](../../../../../../probability-mass-function.md) of the [Poisson distribution](../../../../../../poisson-distribution.md) gives the nonnegative [series](../../../../../../series-mathematics.md)

$$
\mathbb E[X!]=\sum_{k=0}^\infty k!e^{-\lambda}\frac{\lambda^k}{k!}=e^{-\lambda}\sum_{k=0}^\infty\lambda^k.
$$

The [geometric series](../../../../../../geometric-series.md) converges exactly when $0<\lambda<1$. Therefore **$\displaystyle\mathbb E[X!]=\frac{e^{-\lambda}}{1-\lambda}$ for $0<\lambda<1$**. For $\lambda\geq1$, its terms fail to tend to zero and the [expectation](../../../../../../expected-value-split.md) is infinite. This is the [factorial of a Poisson random variable](../../../../../../factorial-of-a-poisson-random-variable.md).

## ↑ Ancestors (13)

1. [V](../v.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
