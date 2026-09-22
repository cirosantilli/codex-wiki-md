<h1 id="7/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Compute fitted responses $\widehat y_i=\widehat\alpha+\widehat\beta x_i$ and [regression residuals](../../../../../../../regression-residual.md) $e_i=y_i-\widehat y_i$. A conventional [residual plot](../../../../../../../residual-plot.md) shows $e_i$ against $\widehat y_i$ or $x_i$; plotting against observation order additionally looks for runs. One checks for curvature, changing spread and other structure rather than random scatter around zero.

**An ordinary [residual plot](../../../../../../../residual-plot.md) need not reveal this failure of [independence](../../../../../../../independent-random-variables.md).** The errors have constant [mean](../../../../../../../expected-value-split.md) zero, constant [variance](../../../../../../../variance-split.md) one and zero pairwise [covariances](../../../../../../../covariance.md), so the usual trend and changing-[variance](../../../../../../../variance-split.md) clues need not appear. A visually patternless [residual plot](../../../../../../../residual-plot.md) cannot validate [independence](../../../../../../../independent-random-variables.md); fitted [regression residuals](../../../../../../../regression-residual.md) themselves also share the fitted coefficients even when the true errors are [independent](../../../../../../../independent-random-variables.md).

There is detectable dependence in the magnitudes. The [Gaussian fourth moment](../../../../../../../gaussian-fourth-moment.md) is $\mathbb E\eta_i^4=3$, giving for every adjacent pair

$$
\boxed{\operatorname{Cov}(\epsilon_i^2,\epsilon_{i+1}^2)=3-1=2.}
$$

For $i=1$, the product is $\eta_1^4\eta_2^2$; for $i\ge2$, it is $\eta_{i-1}^2\eta_i^4\eta_{i+1}^2$, with the same [expected value](../../../../../../../expected-value-split.md) 3. Large magnitudes tend to occur together. A lagged plot of squared [regression residuals](../../../../../../../regression-residual.md) or a test directed at dependence in their squares is more informative. Thus recognition is possible with suitable diagnostics, but is not guaranteed by the standard [residual plot](../../../../../../../residual-plot.md) requested here.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
