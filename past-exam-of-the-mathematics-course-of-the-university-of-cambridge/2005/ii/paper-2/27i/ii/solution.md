<h1 id="27i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $I,J\geq2$. The additive two-way model has dimension $1+(I-1)+(J-1)=I+J-1$; the null model, with no exam effects, has dimension $I$. Write row, column and grand means as $\overline X_{i\cdot},\overline X_{\cdot j},\overline X_{\cdot\cdot}$. [Orthogonal projection](../../../../../../orthogonal-projection.md) onto the full model gives fitted values $\overline X_{i\cdot}+\overline X_{\cdot j}-\overline X_{\cdot\cdot}$, while the null fit is $\overline X_{i\cdot}$. The added exam sum of squares and full residual sum of squares are

$$
SS_E=I\sum_{j=1}^J(\overline X_{\cdot j}-\overline X_{\cdot\cdot})^2,
$$



$$
SS_R=\sum_{i,j}(X_{ij}-\overline X_{i\cdot}-\overline X_{\cdot j}+\overline X_{\cdot\cdot})^2.
$$

The preceding orthogonal-projection result gives [independent](../../../../../../independent-random-variables.md) null chi-squares with $J-1$ and $(I-1)(J-1)$ [degrees of freedom](../../../../../../degree-of-freedom.md). Therefore

$$
\boxed{F=\frac{SS_E/(J-1)}{SS_R/[(I-1)(J-1)]}\sim F_{J-1,(I-1)(J-1)}.}
$$

Reject the no-exam-effect hypothesis for a large value. The printed alternative repeats the identifying constraint $\sum_j\beta_j=0$; a genuine alternative additionally has at least one nonzero $\beta_j$. No interaction term is being fitted; the [independent](../../../../../../independent-random-variables.md) equal-variance Gaussian error assumption is what makes this exact test valid.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [27I](../../27i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
