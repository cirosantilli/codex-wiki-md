<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $A=A_\lambda$ be the [influence matrix](../../../../../../smoothing-matrix.md), so $\widehat y=Ay$. Its [trace](../../../../../../matrix-trace.md) is the [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md), accounting for shrinkage of the fitted smooth rather than just counting basis coefficients. The [generalised cross-validation](../../../../../../generalized-cross-validation.md) score is

$$
\boxed{\operatorname{GCV}(\lambda)=\frac{\|y-A_\lambda y\|^2/n}{\{1-\operatorname{tr}(A_\lambda)/n\}^2}
=\frac{n\sum_i(y_i-\widehat y_i)^2}{\{n-\operatorname{tr}(A_\lambda)\}^2}.}
$$

For a fixed [smoothing parameter](../../../../../../smoothing-parameter.md), the exact leave-one-out residual of this penalized linear fit is $(y_i-\widehat y_i)/(1-A_{ii})$, obtained by removing its observation's contribution to the normal equations. Thus [Leave-one-out cross-validation](../../../../../../leave-one-out-cross-validation.md) uses the average of their squared values. [GCV](../../../../../../generalized-cross-validation.md) replaces the individual leverages $A_{ii}$ by their average $\operatorname{tr}(A)/n$. This avoids separate refits and gives a criterion balancing the small training residuals of a flexible fit against its larger complexity.

Evaluate the score across positive $\lambda$, or optimize it numerically, and choose $\widehat\lambda$ minimizing [GCV](../../../../../../generalized-cross-validation.md). Then refit or retain the [spline](../../../../../../spline-mathematics.md) at this value. In the full natural smoothing-spline family the [trace](../../../../../../matrix-trace.md) decreases from $n$ towards $2$ as smoothing increases. The selected parameter is intended to give good prediction, rather than necessarily to pass through every point.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
