<h1 id="o/o2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a fixed true parameter $0<p<1$, the usual [asymptotic normality of maximum likelihood estimators](../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) gives

$$
\sqrt n(\widehat p-p)\ \xrightarrow{d}\ N\!\left(0,\frac{p^2(1-p)}r\right).
$$

Equivalently, for a large sample, $\widehat p$ is approximately [normally distributed](../../../../../normal-distribution.md) with mean $p$ and [variance](../../../../../variance-split.md) $p^2(1-p)/(nr)$. Replacing the unknown [variance](../../../../../variance-split.md) by its consistent plug-in estimate gives the [Wald confidence interval](../../../../../wald-confidence-interval.md)

$$
\boxed{\widehat p\ \pm\ z_{1-\alpha/2}\widehat p\sqrt{\frac{1-\widehat p}{nr}}}.
$$

Here $z_{1-\alpha/2}$ is a standard-normal [quantile](../../../../../quantile-function.md). Intersect with the physical parameter range $(0,1)$ if needed. This is an interior, large-sample approximation; the degenerate estimate $\widehat p=1$ from $S=0$ does not justify a zero-width finite-sample [interval](../../../../../interval-mathematics.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [O2](../../o2.md)
3. [O](../../../o.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
