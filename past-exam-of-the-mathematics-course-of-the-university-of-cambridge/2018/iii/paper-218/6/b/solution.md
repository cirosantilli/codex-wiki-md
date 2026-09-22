<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two predictors have [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) $\rho=0.9813846$, so there is severe [multicollinearity](../../../../../../multicollinearity.md). Their centered slope [Gram matrix](../../../../../../gram-matrix.md) is

$$
G=n\begin{pmatrix}1&\rho\\\rho&1\end{pmatrix},\qquad G^{-1}=\frac1{n(1-\rho^2)}\begin{pmatrix}1&-\rho\\-\rho&1\end{pmatrix}.
$$

Thus either partial slope has [variance](../../../../../../variance-split.md) $\sigma^2/[n(1-\rho^2)]$. Relative to a univariate regression with the same error variance, the [two-predictor variance inflation](../../../../../../two-predictor-variance-inflation.md) factor and standard-error factor are

$$
\boxed{\frac1{1-\rho^2}\approx27.11,\qquad\frac1{\sqrt{1-\rho^2}}\approx5.21.}
$$

The small [eigenvalue](../../../../../../eigenvalue.md) $n(1-\rho)$ makes the contrast between the two slope effects particularly poorly estimated. The univariate regressions test marginal association with the response; the bivariate tests ask whether one predictor adds an effect while holding its nearly identical companion fixed. Their much larger standard errors therefore make the partial tests insignificant without contradicting the marginal significance. The two fits also estimate slightly different residual variances, explaining why the reported standard-error ratio is not exactly 5.21.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
