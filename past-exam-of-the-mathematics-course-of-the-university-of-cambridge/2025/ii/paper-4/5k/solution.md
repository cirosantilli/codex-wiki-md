<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

For a model with $k$ fitted parameters, the [Akaike information criterion](../../../../../akaike-information-criterion.md) is

$$
\operatorname{AIC}=-2\ell(\widehat\theta)+2k,
$$

where $\ell$ is the log-likelihood evaluated at the maximum-likelihood estimate.

In the normal linear model with known $\sigma^2$,

$$
-2\ell(\beta)
=n\log(2\pi\sigma^2)+\frac1{\sigma^2}\|Y-X\beta\|^2.
$$

The maximum-likelihood estimator is the ordinary least-squares estimator, with fitted mean $\widehat\mu=HY$, where

$$
H=X(X^TX)^{-1}X^T.
$$

Since only the $p$ components of $\beta$ are fitted,

$$
\operatorname{AIC}
=n\log(2\pi\sigma^2)
+\frac1{\sigma^2}\|Y-\widehat\mu\|^2+2p.
$$

After multiplying by $\sigma^2$ and discarding the model-independent constant, this is exactly [Mallows Cp](../../../../../mallows-s-cp.md):

$$
\boxed{C_p=\|Y-\widehat\mu\|^2+2p\sigma^2}.
$$

To compare it with prediction error, write $Y=\mu+\varepsilon$ and $Y^*=\mu+\varepsilon^*$, where $\mu=X\beta$, the two errors are independent, and both have covariance $\sigma^2I$. Since $H\mu=\mu$, $H$ is an orthogonal projection of rank $p$, and

$$
Y^*-\widehat\mu=\varepsilon^*-H\varepsilon.
$$

The cross term has zero expectation, so

$$
\operatorname{MSPE}
=\mathbb E\|\varepsilon^*\|^2
+\mathbb E\|H\varepsilon\|^2
=n\sigma^2+p\sigma^2.
$$

On the other hand,

$$
\mathbb E\|Y-\widehat\mu\|^2
=\mathbb E\|(I-H)\varepsilon\|^2
=\sigma^2\operatorname{tr}(I-H)
=(n-p)\sigma^2.
$$

Therefore the [unbiased prediction-error identity for ordinary least squares](../../../../../unbiased-prediction-error-identity-for-ordinary-least-squares.md) gives

$$
\mathbb E(C_p)=(n-p)\sigma^2+2p\sigma^2
=(n+p)\sigma^2
=\boxed{\operatorname{MSPE}}.
$$

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
