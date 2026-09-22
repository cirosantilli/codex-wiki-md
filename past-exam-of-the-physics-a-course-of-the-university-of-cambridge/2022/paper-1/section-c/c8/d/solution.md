<h1 id="section-c/c8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume independent [normally distributed](../../../../../../normal-distribution.md) [angle](../../../../../../angle.md) errors with known [standard deviation](../../../../../../standard-deviation.md) $\sigma_y=0.002$. The relevant [chi-squared test](../../../../../../chi-squared-test.md) uses the sum of squared standardized residuals,

$$
\chi^2=\sum_i\frac{(y_i-y_{\mathrm{fit},i})^2}{\sigma_y^2}.
$$

For the model through the origin, the predictions and residuals, expressed in milliradians, are

$$
\begin{array}{c|rrrr}
r\ (\mathrm{mm})&16&18&22&32\\\hline
\hat c x\ (\mathrm{mrad})&70.6715&55.8392&37.3800&17.6679\\
y-\hat c x\ (\mathrm{mrad})&-4.6715&-0.8392&6.6200&7.3321
\end{array}
$$

Consequently $\chi_0^2=30.0280$. There are $4-1=3$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md). The upper-tail [P-value](../../../../../../p-value.md) is approximately $1.36\times10^{-6}$; equivalently the value greatly exceeds the $5\%$ critical value $7.815$. The zero-intercept model is strongly rejected under the stated errors.

For the alternative [linear regression](../../../../../../linear-regression-split.md), minimize $\sum_i(y_i-c'x_i-d)^2$. Setting both partial [derivatives](../../../../../../derivative.md) to zero gives the [normal equations](../../../../../../normal-equation.md), whose solution is

$$
\hat c'=\frac{\sum_i(x_i-\bar x)(y_i-\bar y)}{S_{xx}},
\qquad \hat d=\bar y-\hat c'\bar x,
\qquad S_{xx}=\sum_i(x_i-\bar x)^2.
$$

For these data $\bar x=2508.83699\,\mathrm{m^{-2}}$, $\bar y=0.0475$, and $S_{xx}=4.830232\times10^6\,\mathrm{m^{-4}}$. This yields

$$
\boxed{\hat c'=1.37074\times10^{-5}\,\mathrm{m^2},\qquad
\hat d=0.0131105=13.1105\,\mathrm{mrad}.}
$$

The new predictions are $(66.6548,55.4171,41.4315,26.4966)\,\mathrm{mrad}$, with residuals $(-0.6548,-0.4171,2.5685,-1.4966)\,\mathrm{mrad}$. Therefore

$$
\boxed{\chi_1^2=2.35998,\qquad \nu=4-2=2,\qquad p=0.307.}
$$

The affine model is compatible with the data. Allowing for its additional fitted parameter, the decrease $\Delta\chi^2=27.668$ has a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with one [statistical degree of freedom](../../../../../../statistical-degrees-of-freedom.md) under the nested zero-intercept hypothesis, corresponding to $p\simeq1.44\times10^{-7}$. Thus **the model with a fitted intercept provides the better description**, rather than merely lowering the residual by adding a parameter.

With the measurement variance treated as known, the coefficient uncertainties are

$$
\sigma_{c'}=\frac{\sigma_y}{\sqrt{S_{xx}}}=9.10\times10^{-7}\,\mathrm{m^2},
\qquad
\sigma_d=\sigma_y\sqrt{\frac14+\frac{\bar x^2}{S_{xx}}}=0.0024925.
$$

Hence **$d=(13.11\pm2.49)\,\mathrm{mrad}$**, about $5.26$ [standard deviations](../../../../../../standard-deviation.md) above zero. A positive constant [systematic error](../../../../../../systematic-error.md) in the angular zero, or an additional nearly constant [torque](../../../../../../torque.md), could account for it. Its presence is evidence against the ideal zero-intercept model; four points alone do not identify the physical cause uniquely. A calibration error in $\kappa$ only rescales the inferred [gravitational constant](../../../../../../gravitational-constant.md) and cannot remove this residual pattern.

Using the fitted slope after allowing for this offset would give $G'=\kappa\hat c'/(mML)=(7.27\pm0.51)\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$, with the period and slope errors combined in quadrature. This is conditional on the constant-offset model.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
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
