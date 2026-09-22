<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Gaussian linear mixed model](../../../../../../gaussian-linear-mixed-model.md), temporarily regard $\beta,D,R$ as known, with $R=\sigma^2I$ here and $V=ZDZ^T+R$. The joint [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) is

$$
\begin{pmatrix}b\\Y\end{pmatrix}\sim
N\!\left(\begin{pmatrix}0\\X\beta\end{pmatrix},
\begin{pmatrix}D&DZ^T\\ZD&V\end{pmatrix}\right).
$$

By the [conditional multivariate normal distribution](../../../../../../conditional-multivariate-normal-distribution.md) formula,

$$
b\mid Y\sim N\!\left(DZ^TV^{-1}(Y-X\beta),\ D-DZ^TV^{-1}ZD\right).
$$

A nonsingular Gaussian density has its mode at its mean. Thus the [conditional mode of Gaussian random effects](../../../../../../conditional-mode-of-gaussian-random-effects.md) equals the [conditional expectation](../../../../../../conditional-expectation.md). Replacing the unknown parameters by fitted values gives

$$
\boxed{\widehat b=\widehat D Z^T\widehat V^{-1}(Y-X\widehat\beta).}
$$

For positive-definite $D$ and $R$, an equivalent derivation minimizes the negative conditional log density,

$$
(Y-X\beta-Zb)^TR^{-1}(Y-X\beta-Zb)+b^TD^{-1}b.
$$

Differentiation yields

$$
\boxed{\widehat b=(Z^T\widehat R^{-1}Z+\widehat D^{-1})^{-1}
Z^T\widehat R^{-1}(Y-X\widehat\beta).}
$$

The inverse-covariance penalty shrinks furnace intercepts and slopes toward the population effects. For furnace $j$, set $Z_j=(\mathbf1,t_j)$ and $D_j=\operatorname{diag}(\tau_0^2,\tau_1^2)$; the same formula provides its two-component conditional mode from that furnace's observations, conditional on the fitted common parameters. If a [variance component](../../../../../../variance-component.md) is zero, the covariance form remains meaningful and its corresponding [random effect](../../../../../../random-effect.md) is zero, whereas the formula with $D^{-1}$ needs a limiting interpretation. With known covariance parameters these are [best linear unbiased predictors](../../../../../../best-linear-unbiased-prediction.md); plug-in variance estimates give their empirical version.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
