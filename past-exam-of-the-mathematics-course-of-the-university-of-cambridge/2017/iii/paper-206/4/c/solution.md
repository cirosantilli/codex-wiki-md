<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The marginal [Akaike information criterion](../../../../../../akaike-information-criterion.md) is $\operatorname{AIC}=-2\ell(\widehat\vartheta_{\rm ML})+2k$, where $k$ counts estimated population parameters. Here they are $\beta_0,\beta_1,\sigma^2,\tau^2$, so $k=4$. The realized incubator slopes have been integrated out of the [likelihood function](../../../../../../likelihood-function.md); they are not four additional free population coefficients. From the marginal Gaussian [log-likelihood](../../../../../../log-likelihood.md), the expression is

$$
\boxed{\operatorname{AIC}_{\rm ML}=n\log(2\pi)+\log\det\widehat V+(Y-X\widehat\beta)^T\widehat V^{-1}(Y-X\widehat\beta)+8.}
$$

All hats here denote the ordinary [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) fit.

The displayed value $14041.1$ is instead a [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md) criterion. Thus it cannot simply be substituted for the ordinary maximum-likelihood deviance. The [`logLik` method](https://lme4.github.io/lme4/reference/merMod-class.html) defaults to the fitting convention. If one applies `AIC(fly.model)` directly to the displayed REML object, the default restricted [log-likelihood](../../../../../../log-likelihood.md) and the same parameter count give the software's restricted-likelihood-based value $14041.1+8=14049.1$. This number should be labelled as such; it is not the ordinary marginal AIC derived above. To obtain the latter, refit and calculate
```
AIC(update(fly.model, REML=FALSE))
```
The output does not contain that numerical answer. In particular, restricted criteria must not be used to compare models with different fixed-effect designs. A conditional AIC targeting predictions for existing groups is yet another criterion and does not follow by counting each latent slope as an ordinary parameter.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
