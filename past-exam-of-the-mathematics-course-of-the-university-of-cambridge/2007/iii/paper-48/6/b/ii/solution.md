<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fit the [finite Gaussian mixture with a common variance](../../../../../../../finite-gaussian-mixture-with-a-common-variance.md) for candidate values $k=1,\ldots,K$, using several initializations of the [expectation-maximization algorithm](../../../../../../../expectation-maximization-algorithm.md) for each, and retain the best likelihood value found. Maximized likelihood alone cannot select the number of components: a smaller mixture embeds in a larger one by giving an added component zero weight, so its likelihood cannot decrease.

There are $k-1$ free [mixture weights](../../../../../../../mixture-weight.md), $k$ means and one common variance, hence

$$
d_k=(k-1)+k+1=2k.
$$

A standard working choice is the [Bayesian information criterion](../../../../../../../bayesian-information-criterion.md):

$$
\boxed{\widehat k=\underset{1\leq k\leq K}{\operatorname{argmin}}\left\{-2\ell(\widehat\theta_k)+2k\log N\right\}.}
$$

The penalty balances fit against parameter count. The [Akaike information criterion](../../../../../../../akaike-information-criterion.md) instead uses $-2\ell(\widehat\theta_k)+4k$ and is another possible comparison, particularly when predictive fit is the goal. The parameter count would differ if component variances were separate, but that is not this model.

Likelihood fitting must first be made well posed. Even a shared variance does not prevent all degeneracy: if $k=N$, choose $\mu_j=x_j$, $\alpha_j=1/N$ and let the common variance tend to zero. Each observed density is at least $1/(N\sqrt{2\pi\sigma^2})$, so the full [log-likelihood function](../../../../../../../log-likelihood.md) tends to $+\infty$. The same construction works when $k$ reaches the number of distinct observed values. Thus one must not feed infinite fitted likelihoods into an information criterion. Restrict candidate sizes to a sensible range below that degeneracy, or impose a fixed positive variance floor and use that same constrained model in every comparison. Under a variance floor $\varepsilon$, the M-step variance becomes $\max\{\varepsilon,R/N\}$.

There is also [nonregular mixture model selection](../../../../../../../nonregular-mixture-model-selection.md): at a missing component its weight is on a boundary and its mean is unidentified, while permuting labels leaves the distribution unchanged. Consequently an ordinary chi-squared calibration for a [likelihood-ratio test](../../../../../../../likelihood-ratio-test.md) between successive component counts is not generally justified. Information criteria are practical comparisons, not an automatic universal proof that the true number has been recovered. Predictive [cross-validation](../../../../../../../cross-validation.md) or a suitably constructed parametric bootstrap comparison can supplement them. **Select the component count by a penalized, well-defined mixture fit, rather than by unpenalized likelihood increase.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 48](../../../../paper-48-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
