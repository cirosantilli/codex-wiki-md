<h1 id="o/o2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $n>2$, the usual [unbiased estimator](../../../../../unbiased-estimator.md) of variance is

$$
\boxed{s^2=\frac{\operatorname{RSS}}{n-2},\qquad
\operatorname{RSS}=\sum_i(Y_i-\widehat\alpha-\widehat\beta x_i)^2.}
$$

The fitted mean lies in the two-dimensional span of the constant design vector and $x$. [Orthogonal projection](../../../../../orthogonal-projection.md) of the Gaussian error onto its complement gives $n-2$ independent standardized normal coordinates. Hence

$$
\boxed{(n-2)s^2/\sigma^2=\operatorname{RSS}/\sigma^2\sim\chi^2_{n-2}.}
$$

This residual projection is independent of the fitted-coefficient projection. If maximum likelihood for variance is intended instead, its estimator is $\widehat\sigma^2_{\rm ML}=\operatorname{RSS}/n$, with $n\widehat\sigma^2_{\rm ML}/\sigma^2\sim\chi^2_{n-2}$; the denominator differs, not the residual [degrees of freedom](../../../../../degree-of-freedom.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [O2](../../o2.md)
3. [O](../../../o.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
