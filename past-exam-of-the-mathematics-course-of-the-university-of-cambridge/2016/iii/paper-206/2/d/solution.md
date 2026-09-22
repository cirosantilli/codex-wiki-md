<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Box–Cox transformation](../../../../../../box-cox-transformation.md) searches over transformations of the positive response,

$$
T_\lambda(y)=\begin{cases}(y^\lambda-1)/\lambda,&\lambda\ne0,\\\log y,&\lambda=0.\end{cases}
$$

The plotted horizontal coordinate is $\lambda$ and the vertical coordinate is its maximized [profile likelihood](../../../../../../profile-likelihood.md) on the log scale. The likelihood includes the transformation [Jacobian determinant](../../../../../../jacobian-determinant.md); omitting it would compare response scales incorrectly. For the Gaussian regression it is, up to constants,

$$
\ell_p(\lambda)=-\frac n2\log\bigl(\mathrm{RSS}_\lambda/n\bigr)
+(\lambda-1)\sum_i\log y_i.
$$

The maximum occurs around $\lambda=2$. The horizontal 95% line is approximately $\ell_p(\widehat\lambda)-\chi^2_{1,0.95}/2$, and its intersections give an approximate interval roughly $1.2$ to $2.8$, read visually. In particular, $\lambda=1$ is below the line, and $\lambda=0$ is far below it.

**Square the response:** a convenient transformation is $Y_i^2$, equivalent up to affine rescaling to $T_2(Y_i)=(Y_i^2-1)/2$. Transform energy, not the sunny-days or latitude predictors. Refit and check the [normal linear model](../../../../../../normal-linear-model.md) on the transformed scale; the plot is evidence for a transformation, not proof that the transformed residual assumptions hold. Inference on transformed means cannot be inverted naively to obtain original-scale conditional means.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
