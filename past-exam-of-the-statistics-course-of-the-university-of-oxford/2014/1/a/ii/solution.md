<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $z=\Phi^{-1}(1-\alpha/2)$, where $\Phi$ is the [standard normal distribution](../../../../../standard-normal-distribution.md)'s [cumulative distribution function](../../../../../cumulative-distribution-function.md). [Statistical consistency](../../../../../consistency-statistics.md) and [Slutsky's theorem](../../../../../slutsky-theorem.md) allow replacement of $I_1(\theta)$ by $I_1(\widehat\theta)$:

$$
\sqrt{nI_1(\widehat\theta)}(\widehat\theta-\theta)\ \xrightarrow{d}\ N(0,1).
$$

Thus the probability that this standardized [estimation error](../../../../../estimation-error.md) lies between $-z$ and $z$ tends to $1-\alpha$. Rearranging gives the [Wald confidence interval](../../../../../wald-confidence-interval.md)

$$
\boxed{\left[\widehat\theta-\frac{z}{\sqrt{nI_1(\widehat\theta)}},\quad
\widehat\theta+\frac{z}{\sqrt{nI_1(\widehat\theta)}}\right].}
$$

The [coverage probability](../../../../../coverage-probability.md) is approximate, with limiting value $1-\alpha$; it is a repeated-sampling statement about the random [confidence interval](../../../../../confidence-interval.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
