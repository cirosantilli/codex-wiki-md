<h1 id="1/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The [standard error](../../../../../standard-error.md) suggested by part (iii) is $\theta/\sqrt n$. Substituting the [consistent estimator](../../../../../consistency-statistics.md) $T_2$ gives $T_2/\sqrt n$; [Slutsky's theorem](../../../../../slutsky-theorem.md) gives

$$
\frac{\sqrt n(T_2-\theta)}{T_2}\xrightarrow dN(0,1).
$$

Using the central [standard normal quantiles](../../../../../standard-normal-quantile.md) $\pm1.96$, an approximate 95% [Wald confidence interval](../../../../../wald-confidence-interval.md) is

$$
\boxed{\left[T_2\left(1-\frac{1.96}{\sqrt n}\right),\quad
T_2\left(1+\frac{1.96}{\sqrt n}\right)\right]\cap(0,\infty)}.
$$

Its [coverage probability](../../../../../coverage-probability.md) approaches 0.95 for each fixed $\theta>0$ as $n\to\infty$. The intersection enforces positivity and does not change whether the true positive [statistical parameter](../../../../../statistical-parameter.md) is covered. The value 1.64 would give the wrong central two-sided [coverage probability](../../../../../coverage-probability.md).

## ↑ Ancestors (13)

1. [V](../v.md)
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
