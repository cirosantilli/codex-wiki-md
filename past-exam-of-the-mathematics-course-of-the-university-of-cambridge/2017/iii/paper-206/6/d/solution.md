<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [universal kriging](../../../../../../universal-kriging.md) model has a linear drift in $y$ and a zero-mean Gaussian residual field:

$$
Z(x,y)=\beta_0+\beta_1y+W(x,y),\qquad \operatorname{Cov}(W(s),W(t))=\sigma^2e^{-(\|s-t\|/a)^2}+\tau^2\mathbf1_{\{s=t\}}.
$$

The `Gau` range parameter in this software is $a=1/\phi$, since its [semivariogram](../../../../../../semivariogram.md) uses $1-e^{-(h/a)^2}$. The output gives $\widehat\tau^2=0$, $\widehat\sigma^2=0.4726257$, and $\widehat a=1.112235$, hence $\widehat\phi\simeq0.899091$. The exact Gaussian range is infinite; the 95-percent [practical range](../../../../../../practical-range.md) is approximately $1.92508$ in the coordinate distance units.

The [`BLUE=TRUE` option](https://r-spatial.github.io/gstat/reference/predict.gstat.html) asks for the [best linear unbiased estimator](../../../../../../best-linear-unbiased-estimator.md) of the drift, rather than the full field [kriging](../../../../../../kriging.md) prediction. Thus the two printed fitted trends give $\widehat\beta_0=20.13793$ at $y=0$ and $\widehat\beta_0+\widehat\beta_1=22.08399$ at $y=1$. Therefore

$$
\boxed{\widehat m(x,y)=20.13793+1.94606y,\quad\widehat\tau^2=0,\quad\widehat\sigma^2=0.4726257,\quad\widehat a=1.112235.}
$$

There is no $x$ coefficient in the drift. The reported [variances](../../../../../../variance-split.md) $0.09456496$ and $0.06097459$ are the [variances](../../../../../../variance-split.md) of the corresponding estimated trend values, not full-field prediction [variances](../../../../../../variance-split.md). They do not determine the slope [variance](../../../../../../variance-split.md) without its [covariance](../../../../../../covariance.md) with the intercept. The interpolated map can still vary with $x$ through the correlated residual prediction, even though the fitted deterministic drift depends only on $y$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
