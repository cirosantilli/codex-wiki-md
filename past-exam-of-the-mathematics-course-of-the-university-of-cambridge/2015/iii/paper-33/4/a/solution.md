<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an [unpenalized intercept in ridge regression](../../../../../../unpenalized-intercept-in-ridge-regression.md). For centered predictor columns, the [ridge regression](../../../../../../ridge-regression.md) optimization is

$$
\min_{\alpha,\beta}\ \|Y-\alpha\mathbf1-X\beta\|_2^2+\lambda\|\beta\|_2^2,\qquad\lambda\geq0.
$$

Differentiating with respect to $\alpha$ gives $\widehat\alpha=\overline Y$. Put $Y_c=Y-\overline Y\mathbf1$. Differentiation with respect to $\beta$ gives the ridge [normal equation](../../../../../../normal-equation.md)

$$
(X^TX+\lambda I_6)\widehat\beta_\lambda=X^TY_c.
$$

Consequently the [closed-form ridge regression estimator](../../../../../../closed-form-ridge-regression-estimator.md) is

$$
\boxed{\widehat\beta_\lambda=(X^TX+\lambda I_6)^{-1}X^TY_c,\qquad\widehat\alpha=\overline Y.}
$$

Because $X^T\mathbf1=0$, the numerator may also be written $X^TY$. For $\lambda>0$ the inverse exists even with [multicollinearity](../../../../../../multicollinearity.md) or deficient column rank; at $\lambda=0$ a unique [ordinary least squares](../../../../../../ordinary-least-squares.md) coefficient vector requires full rank. The quadratic penalty stabilizes nearly singular directions but generally does not set individual coefficients exactly to zero.

For uncentered original predictors, use $X_c=X-\mathbf1\overline x^T$, apply the displayed estimator to $X_c,Y_c$, and recover $\widehat\alpha=\overline Y-\overline x^T\widehat\beta$. Any internal scaling used by `lm.ridge` must be undone to report coefficients on the original predictor scale. Multiplying the objective by a constant changes the numerical penalty convention unless $\lambda$ is rescaled as well.

## ↑ Ancestors (11)

1. [A](../a.md)
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
