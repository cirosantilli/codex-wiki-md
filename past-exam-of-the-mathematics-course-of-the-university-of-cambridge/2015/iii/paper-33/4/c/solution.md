<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An intercept-unpenalized [Lasso](../../../../../../lasso.md) estimator solves the constrained optimization

$$
\boxed{\min_{\alpha,\beta}\ \|Y-\alpha\mathbf1-X\beta\|_2^2
\quad\text{subject to}\quad\sum_{j=1}^6|\beta_j|\leq t.}
$$

For centered predictors, eliminate the intercept as in [ridge regression](../../../../../../ridge-regression.md) and minimize $\|Y_c-X\beta\|_2^2$ under the same constraint. Equivalently, with a suitable tuning parameter $\lambda\geq0$, use $\|Y-\alpha\mathbf1-X\beta\|_2^2+\lambda\sum_j|\beta_j|$. The constraint radius and penalty parameter are different parametrizations; larger radius permits less shrinkage.

The [Lasso](../../../../../../lasso.md) plot parametrizes the [Lasso regularization path](../../../../../../lasso-regularization-path.md) by the fraction of the maximum $l_1$ norm of the standardized slopes. Unlike the ridge quadratic penalty, the corners of the $l_1$ constraint can place some slopes exactly at zero, providing [variable selection](../../../../../../variable-selection.md). The maximum norm refers to the path's unpenalized endpoint; centering and scaling conventions must match those used to construct that path.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
