<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Both fits use the same [Gamma distribution](../../../../../../gamma-distribution.md) mean model and inverse [link function](../../../../../../link-function.md). Their coefficient estimates, fitted means and hence their weight matrices coincide: the common [dispersion parameter](../../../../../../dispersion-parameter.md) only multiplies the likelihood score by a scalar and therefore does not change its zero. The displayed calls likewise show the same family and formula; fixing dispersion in a summary changes the uncertainty calculation, not these coefficient estimates.

For $V(\mu)=\mu^2$ and $g'(\mu)=-\mu^{-2}$, the [Fisher information](../../../../../../fisher-information-matrix.md) weights are

$$
W_{ii}=\{a_i\mu_i^2\mu_i^{-4}\}^{-1}=\mu_i^2/a_i.
$$

Thus the common matrix $(X^TWX)^{-1}$ is multiplied by dispersion $1$ in the exponential case and by $\widehat\phi=0.3103711$ in the fitted gamma case. Taking square roots of the diagonal [covariances](../../../../../../covariance.md) gives

$$
\boxed{SE_{\mathrm{mod2}}(\widehat\beta_j)=\sqrt{0.3103711}\,SE_{\mathrm{mod1}}(\widehat\beta_j)\approx0.5571\,SE_{\mathrm{mod1}}(\widehat\beta_j).}
$$

For instance $0.03607\times0.5571\approx0.02009$ for the intercept, and the same factor applies to all the coefficients. The [standard errors](../../../../../../standard-error.md) are smaller because the fitted [dispersion parameter](../../../../../../dispersion-parameter.md) is below one, not because a different mean function was fitted.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
