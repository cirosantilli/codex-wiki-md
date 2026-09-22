<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [ridge regression](../../../../../../ridge-regression.md) penalty is quadratic, whereas the [Lasso](../../../../../../lasso.md) uses an absolute-value penalty. To make the constants explicit, compare

$$
\|Y-X\beta\|_2^2+\lambda\|\beta\|_2^2\qquad\text{and}\qquad\|Y-X\beta\|_2^2+2t\|\beta\|_1.
$$

Both trade goodness of fit against coefficient size, and both require sensible predictor scaling and tuning. Ridge continuously shrinks coefficient directions and generally retains all variables. The Lasso's nonsmooth penalty can set coefficients exactly to zero, so it performs variable selection as well as shrinkage. When $X^TX=I$, let $z=X^TY$. The distinction is especially transparent:

$$
\boxed{\widehat\beta_j^{\mathrm{ridge}}=\frac{z_j}{1+\lambda},\qquad\widehat\beta_j^{\mathrm{Lasso}}=\operatorname{sign}(z_j)(|z_j|-t)_+.}
$$

The second formula is [soft thresholding](../../../../../../soft-thresholding.md). For general designs, the [Karush-Kuhn-Tucker conditions for the Lasso](../../../../../../karush-kuhn-tucker-conditions-for-the-lasso.md) give $X_j^T(Y-X\widehat\beta)=t\operatorname{sign}(\widehat\beta_j)$ for a nonzero coefficient and $|X_j^T(Y-X\widehat\beta)|\le t$ for a zero coefficient. The latter interval permits exact zeros; the ridge equation instead is $X^T(Y-X\widehat\beta)=\lambda\widehat\beta$.

Ridge is especially useful for stable prediction when many predictors carry small effects or are highly correlated. Its strictly convex penalty gives unique coefficients for $\lambda>0$ even in a rank-deficient design. It shares an effect among identical predictor columns: for a fixed coefficient sum the minimum quadratic penalty splits that sum equally. The Lasso can give a simpler sparse model when many effects are absent, but selection among strongly correlated predictors can be unstable. With identical columns, any same-sign split of a selected coefficient sum has the same absolute-value penalty and the same fitted values, so the coefficient vector need not be unique. This is a possible design degeneracy, not a claim that every Lasso fit is nonunique.

The penalties also encode different prior shapes: the Gaussian prior yields ridge, while independent double-exponential priors yield a Lasso posterior mode under Gaussian noise. A Lasso mode is not generally its posterior mean. Practically, sparse interpretability favors the Lasso, while stable distributed effects can favor ridge; prediction performance should be checked with [cross-validation](../../../../../../cross-validation.md), and neither method universally dominates the other.

## ↑ Ancestors (11)

1. [C](../c.md)
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
