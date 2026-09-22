<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [conditional multivariate normal distribution](../../../../../conditional-multivariate-normal-distribution.md) gives

$$
y\mid z\sim N(z^T\beta,\sigma^2),
\quad
\beta=\Sigma_{-1,-1}^{-1}\Sigma_{-1,1},
\quad
\sigma^2=\Sigma_{11}-\Sigma_{1,-1}\Sigma_{-1,-1}^{-1}\Sigma_{-1,1}>0.
$$

For a jointly Gaussian vector, the residual is independent of the regressor, so $y=z^T\beta+\sigma e$ with $e\sim N(0,1)$ independent of $z$.

The [Square-root Lasso](../../../../../square-root-lasso.md) minimizes

$$
\frac1{\sqrt n}\lVert X-Z\theta\rVert_2+\gamma\lVert\theta\rVert_1,
\qquad \gamma=\sqrt{\frac{2\log p}{n}}.
$$

At a nonzero residual $R$, its KKT condition is

$$
\frac{Z^TR}{\sqrt n\lVert R\rVert_2}=\gamma u,
\qquad\lVert u\rVert_\infty\leq1,
$$

which proves the required inequality.

Writing the response vector as $Y=f+\sigma e$, the reverse triangle inequality gives

$$
\left|\widehat\sigma-\sigma\frac{\lVert e\rVert_2}{\sqrt n}\right|
\leq\frac{\lVert\widehat f-f\rVert_2}{\sqrt n}=o_P(1).
$$

The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives $\lVert e\rVert_2/\sqrt n\to_P1$, hence $\widehat\sigma\to_P\sigma$.

Under $X\perp\!\!\!\perp Y\mid Z$, Gaussianity makes $e$ independent of $(X,Z)$ and hence of $R$. Conditionally on $R$, $R^Te/\lVert R\rVert_2\sim N(0,1)$. The remaining numerator term obeys

$$
\frac{|R^TZ(\beta-\widehat\beta)|}{\lVert R\rVert_2}
\leq\frac{\lVert Z^TR\rVert_\infty}{\lVert R\rVert_2}
\lVert\widehat\beta-\beta\rVert_1
\leq\sqrt{2\log p}\,\lVert\widehat\beta-\beta\rVert_1=o_P(1).
$$

Combining this with $\widehat\sigma\to_P\sigma$ and [Slutsky theorem](../../../../../slutsky-theorem.md) proves the standard-normal limit.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
