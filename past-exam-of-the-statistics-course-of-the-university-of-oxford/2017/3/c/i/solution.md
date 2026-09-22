<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a scalar [statistical parameter](../../../../../statistical-parameter.md) in a regular model with [probability mass function](../../../../../probability-mass-function.md) $f(x\mid\theta)$, define the one-observation expected [Fisher information](../../../../../fisher-information-matrix.md) by

$$
I(\theta)=\mathbb E_\theta\!\left[\{\partial_\theta\log f(X\mid\theta)\}^2\right]
=\sum_x\frac{\{\partial_\theta f(x\mid\theta)\}^2}{f(x\mid\theta)}.
$$

The [Jeffreys prior](../../../../../jeffreys-prior.md) is the [prior density](../../../../../prior-density.md) specified, up to a factor independent of $\theta$, by

$$
\boxed{\pi_J(\theta)\propto\sqrt{I(\theta)}.}
$$

For $n$ independent observations the [Fisher information](../../../../../fisher-information-matrix.md) is $nI(\theta)$, so the factor $\sqrt n$ does not change this [prior distribution](../../../../../prior-probability.md). If $\int\sqrt{I(\theta)}\,d\theta$ is finite, divide by this integral to normalize; otherwise the rule defines an [improper prior](../../../../../improper-prior.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
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
