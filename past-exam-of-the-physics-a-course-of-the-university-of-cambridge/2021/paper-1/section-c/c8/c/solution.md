<h1 id="section-c/c8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume independent approximately Gaussian log-rate errors with known common [standard deviation](../../../../../../standard-deviation.md) $s=0.15$. The [weighted least squares](../../../../../../weighted-least-squares.md) objective is

$$
\chi^2(m,c)=\frac1{s^2}\sum_{i=1}^{6}(y_i-mx_i-c)^2.
$$

Since all weights agree, the [normal equations for linear least squares](../../../../../../normal-equations-for-linear-least-squares.md) reduce to

$$
\widehat m=\frac{S_{xy}}{S_{xx}},\qquad
\widehat c=\bar y-\widehat m\bar x,
\quad S_{xx}=\sum_i(x_i-\bar x)^2,\quad
S_{xy}=\sum_i(x_i-\bar x)(y_i-\bar y).
$$

For these data, $\bar x=1.5\,\mathrm{ps}$, $\bar y=4.1596533$, $S_{xx}=4.375\,\mathrm{ps}^2$ and $S_{xy}=-10.3782409\,\mathrm{ps}$. Hence $\widehat m=-2.3721693\,\mathrm{ps}^{-1}$ and $\widehat c=7.7179073$.

The [covariance matrix](../../../../../../covariance-matrix.md) of the fitted slope and intercept follows from the inverse weighted [design matrix](../../../../../../design-matrix.md) product, or directly by writing both estimates as linear combinations of the independent $y_i$:

$$
\operatorname{Var}(\widehat m)=\frac{s^2}{S_{xx}},\qquad
\operatorname{Var}(\widehat c)=s^2\left(\frac16+\frac{\bar x^2}{S_{xx}}\right),\qquad
\operatorname{Cov}(\widehat m,\widehat c)=-\frac{s^2\bar x}{S_{xx}}.
$$

This gives

$$
\boxed{\widehat m=(-2.372\pm0.072)\,\mathrm{ps}^{-1},\qquad
\widehat c=7.718\pm0.124.}
$$

The parameter conversion and first-order [propagation of uncertainty](../../../../../../propagation-of-uncertainty.md) are

$$
\widehat\tau=-\frac1{\widehat m},\quad
\sigma_\tau=\frac{\sigma_m}{\widehat m^2},\qquad
\widehat R_0=R_*e^{\widehat c},\quad
\sigma_{R_0}=\widehat R_0\sigma_c.
$$

Consequently,

$$
\boxed{\widehat\tau=(0.4216\pm0.0127)\,\mathrm{ps},\qquad
\widehat R_0=(2.25\pm0.28)\times10^3\,\mathrm{counts\,day^{-1}}.}
$$

These are one-[standard deviation](../../../../../../standard-deviation.md) errors. The estimates are correlated, since $\operatorname{Cov}(\widehat m,\widehat c)=-0.0077143\,\mathrm{ps}^{-1}$. The minimum is $\chi^2_{\min}=4.6537$ for four residual degrees of freedom. Because $s$ is supplied as a known measurement uncertainty, it should not be rescaled by the observed reduced $\chi^2$. This is a [log-linear exponential-decay fit](../../../../../../log-linear-exponential-decay-fit.md).

<a id="section-c/c8/c/image-log-rate-fit-and-the-effect-of-imposing-the-alternative-lifetime"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1-lifetime-fit.png)

**[Figure 3](#section-c/c8/c/image-log-rate-fit-and-the-effect-of-imposing-the-alternative-lifetime). Log-rate fit and the effect of imposing the alternative lifetime**. Original calculation from the exam measurements. The solid line fits both lifetime and normalization; the dashed line fixes $\tau=0.478\,\mathrm{ps}$ and refits its normalization. The lower panel shows standardized log-rate residuals for the two fits. No error bar is assigned to proper time.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
