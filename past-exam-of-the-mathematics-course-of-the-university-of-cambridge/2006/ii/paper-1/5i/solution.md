<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

Put $\widehat\beta=(X^TX)^{-1}X^TY$, $\widehat\sigma^2=\|Y-X\widehat\beta\|^2/(n-p)$. Orthogonal projections of the Gaussian error give independent variables

$$
\frac{(\widehat\beta-\beta)^TX^TX(\widehat\beta-\beta)}{\sigma^2}\sim\chi_p^2,\qquad\frac{(n-p)\widehat\sigma^2}{\sigma^2}\sim\chi_{n-p}^2.
$$

Hence the exact $(1-\alpha)$ [confidence set](../../../../../confidence-region.md) is the ellipsoid

$$
\boxed{\left\{b:\frac{(b-\widehat\beta)^TX^TX(b-\widehat\beta)}{p\widehat\sigma^2}\leq F_{p,n-p}(1-\alpha)\right\}.}
$$

Here $F_{p,n-p}(q)$ denotes the $q$ quantile of the [F-distribution](../../../../../f-distribution.md).

Let $\widehat\beta_{(-i)}$ be the fit with observation $i$ removed, when that reduced design retains full rank. [Cook's distance](../../../../../cook-s-distance.md) is

$$
D_i=\frac{(\widehat\beta_{(-i)}-\widehat\beta)^TX^TX(\widehat\beta_{(-i)}-\widehat\beta)}{p\widehat\sigma^2}
=\frac{e_i^2}{p\widehat\sigma^2}\frac{h_{ii}}{(1-h_{ii})^2},
$$

where $e_i$ is its residual and $h_{ii}=x_i^T(X^TX)^{-1}x_i$ is its [leverage](../../../../../regression-leverage.md). Thus $D_i$ measures the deleted estimate's distance from the full estimate in exactly the metric of the confidence ellipsoids. The deleted estimate lies on the confidence contour whose $F$ quantile equals $D_i$; this is a geometric influence diagnostic, not an assertion that $D_i$ itself has an $F$ law.

For $p=2,n=50$, $0.70<1.3<2.42$, so deletion moves the estimate outside the 50% [confidence ellipsoid](../../../../../confidence-ellipsoid.md) but inside the 90% one. **The observation warrants investigation for influence**: the shift is substantial, though the supplied figures do not justify calling it outside the 90% region. The reciprocal $F_{48,2}$ and the approximate chi-square figures are unnecessary.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
