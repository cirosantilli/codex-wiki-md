<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $I_1(\theta)$ for the [Fisher information](../../../../../fisher-information-matrix.md) in one observation:

$$
I_1(\theta)=\mathbb E_\theta\!\left[\left\{\frac{\partial}{\partial\theta}\log f(X;\theta)\right\}^2\right]
=-\mathbb E_\theta\!\left[\frac{\partial^2}{\partial\theta^2}\log f(X;\theta)\right].
$$

Under the stipulated regularity assumptions, the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) is [consistent](../../../../../consistency-statistics.md) and has [asymptotic normality](../../../../../asymptotic-normality.md):

$$
\boxed{\sqrt n(\widehat\theta-\theta)\ \xrightarrow{d}\ N\!\left(0,I_1(\theta)^{-1}\right).}
$$

Equivalently, its large-sample [normal approximation](../../../../../normal-approximation.md) has [mean](../../../../../expected-value-split.md) $\theta$ and [variance](../../../../../variance-split.md) $1/[nI_1(\theta)]$. The information for the whole [random sample](../../../../../independent-and-identically-distributed-random-variables.md) is $nI_1(\theta)$; keeping the one-observation convention explicit prevents an extra factor of $n$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
