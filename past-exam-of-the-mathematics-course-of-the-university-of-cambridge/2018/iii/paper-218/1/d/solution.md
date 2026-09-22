<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There are two defects. The mixed fit supplies a [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md), whereas the ordinary fit supplies an ordinary [log-likelihood](../../../../../../log-likelihood.md), so their difference is not a [likelihood-ratio test statistic](../../../../../../likelihood-ratio-test-statistic.md). Also, $H_0:\tau^2=0$ lies on the boundary of $\tau^2\geq0$; the usual [Wilks theorem](../../../../../../wilks-theorem.md) does not give a $\chi_1^2$ null law.

A valid approach first refits the mixed model by ordinary [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md), setting REML to false, and fits the same fixed effects under $H_0$. For $V=\tau^2ZZ^T+\sigma^2I$, maximize

$$
\ell(\beta,\tau^2,\sigma^2)=-\frac{176}{2}\log(2\pi)-\frac12\log\det V-\frac12(Y-X\beta)^TV^{-1}(Y-X\beta)
$$

over $\beta,\sigma^2>0,\tau^2\geq0$, and separately over $\beta,\sigma^2>0$ with $\tau^2=0$. Set $T=2(\widehat\ell_1-\widehat\ell_0)\geq0$.

For finite-sample calibration, use the [location-scale invariant simulation test for a Gaussian variance component](../../../../../../location-scale-invariant-simulation-test-for-a-gaussian-variance-component.md). With the actual $X,Z$ fixed, simulate $B$ independent vectors $Y^{(b)}\sim N(0,I_{176})$, refit both models by ordinary [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) to each, and calculate $T_b$ in exactly the same way. Under $H_0$, $Y=X\beta+\sigma z$. Translating by a vector in the [column space](../../../../../../column-space.md) of $X$ and multiplying by a positive scalar preserves the statistic: both maximized log-likelihoods acquire the same scale constant. Thus this simulation has the correct null law without knowing $\beta$ or $\sigma$. A conservative Monte Carlo [p-value](../../../../../../p-value.md) is

$$
\boxed{p_{MC}=\frac{1+\sum_{b=1}^B\mathbf1_{\{T_b\geq T\}}}{B+1};\qquad\text{reject if }p_{MC}\leq0.05.}
$$

In the usual regular limit with increasing independent groups, a [variance-component likelihood-ratio test at a boundary](../../../../../../variance-component-likelihood-ratio-test-at-a-boundary.md) instead uses $\tfrac12\delta_0+\tfrac12\chi_1^2$: for $T>0$, its approximate tail probability is $\tfrac12\Pr(\chi_1^2\geq T)$, and at $T=0$ the nonrandomized p-value is one. This approximation is not an exact guarantee for sixteen rats. Alternatively one can compare consistently defined restricted likelihoods with the same $X$ and simulate their restricted-ratio null distribution, as in [the RLRsim documentation](https://search.r-project.org/CRAN/refmans/RLRsim/html/exactRLRT.html).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
