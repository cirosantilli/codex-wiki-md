<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an $n\times p$ [design matrix](../../../../../../design-matrix.md), distinguish the coefficient vector from the fitted-response vector. The [ridge regression](../../../../../../ridge-regression.md) objective and its solution are

$$
\boxed{Q_\lambda(\beta)=\|Y-X\beta\|_2^2+\lambda\|\beta\|_2^2,\qquad \widehat\beta_\lambda=(X^TX+\lambda I_p)^{-1}X^TY.}
$$

The [gradient](../../../../../../gradient.md) is $2(X^TX+\lambda I_p)\beta-2X^TY$. For $\lambda>0$, $X^TX+\lambda I_p$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), so this is the unique minimizer even if $X$ is rank deficient. The expression with an additional leading $X$ is instead the $n$-vector of [fitted values](../../../../../../fitted-values.md),

$$
\widehat Y_\lambda=X\widehat\beta_\lambda=X(X^TX+\lambda I_p)^{-1}X^TY.
$$

This distinction corrects the dimensional mismatch in the printed coefficient-estimator notation.

The quadratic penalty discourages large coefficients, exchanging some bias for lower variance. If $X=UDV^T$ is a reduced [singular value decomposition](../../../../../../singular-value-decomposition.md), with positive singular values $d_k$, then

$$
\widehat\beta_\lambda=V\operatorname{diag}\left(\frac{d_k}{d_k^2+\lambda}\right)U^TY,\qquad \widehat Y_\lambda=U\operatorname{diag}\left(\frac{d_k^2}{d_k^2+\lambda}\right)U^TY.
$$

The [principal-component shrinkage by ridge regression](../../../../../../principal-component-shrinkage-by-ridge-regression.md) therefore shrinks directions with small $d_k^2$ most strongly. These are precisely the poorly determined directions created by [multicollinearity](../../../../../../multicollinearity.md), where ordinary least-squares coefficients can have large variance or fail to be uniquely determined. A positive penalty stabilizes their inversion and sets coefficients in the null space to zero. It does not make the predictors independent or provide a universal risk improvement for every signal. Because the penalty depends on coefficient units, predictors are ordinarily standardized before choosing $\lambda$ by [cross-validation](../../../../../../cross-validation.md). An [unpenalized intercept in ridge regression](../../../../../../unpenalized-intercept-in-ridge-regression.md) is handled separately by centering; the displayed objective either has no intercept or applies the penalty to every component included in $\beta$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
