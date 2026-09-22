<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because the columns of the [design matrix](../../../../../../design-matrix.md) are centred, [ridge regression](../../../../../../ridge-regression.md) with an unpenalized intercept solves

$$
(\widehat\alpha_\lambda,\widehat\beta_\lambda)
=\underset{\alpha\in\mathbb R,\,\beta\in\mathbb R^p}{\operatorname{argmin}}
\left\{\|Y-\alpha\mathbf1-X\beta\|_2^2
+\lambda\|\beta\|_2^2\right\}.
$$

The [normal equations](../../../../../../normal-equation.md) give, for $\lambda>0$,

$$
\widehat\alpha_\lambda=\overline Y,
\qquad
\widehat\beta_\lambda=(X^TX+\lambda I_p)^{-1}X^T(Y-\overline Y\mathbf1)
=(X^TX+\lambda I_p)^{-1}X^TY.
$$

The [fitted values](../../../../../../fitted-values.md) are consequently

$$
\widehat Y_\lambda
=\overline Y\mathbf1+X(X^TX+\lambda I_p)^{-1}X^TY.
$$

If the objective is normalized by $n$, the same formulas hold after replacing $\lambda$ by $n\lambda$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
