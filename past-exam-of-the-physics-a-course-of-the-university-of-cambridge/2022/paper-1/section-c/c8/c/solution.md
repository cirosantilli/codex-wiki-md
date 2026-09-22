<h1 id="section-c/c8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

All four [angle](../../../../../../angle.md) measurements have the same [standard uncertainty](../../../../../../standard-uncertainty.md), so [ordinary least squares](../../../../../../ordinary-least-squares.md) minimizes

$$
S(c)=\sum_{i=1}^4(y_i-cx_i)^2.
$$

[Differentiation](../../../../../../differentiation.md) gives

$$
\frac{dS}{dc}=-2\sum_i x_i(y_i-cx_i)=0,
\qquad \frac{d^2S}{dc^2}=2\sum_i x_i^2>0.
$$

Thus the unique minimum is

$$
\boxed{\hat c=\frac{\sum_i x_iy_i}{\sum_i x_i^2}
=\frac{\overline{xy}}{\overline{xx}}.}
$$

The overbars denote [sample means](../../../../../../sample-mean.md) over the four observations. Numerically,

$$
\sum_i x_iy_i=542.888740\,\mathrm{m^{-2}},\qquad
\sum_i x_i^2=3.00072844\times10^7\,\mathrm{m^{-4}},
$$

so

$$
\boxed{\hat c=1.80919\times10^{-5}\,\mathrm{m^2},\qquad
\hat G=\frac{\kappa\hat c}{mML}=9.59\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}.}
$$

The fixed $x_i$ have negligible uncertainty. Assuming [independent](../../../../../../independent-random-variables.md) errors in the four $y_i$, [propagation of uncertainty](../../../../../../propagation-of-uncertainty.md) in quadrature gives

$$
\sigma_{\hat c}^2=\sum_i\left(\frac{\partial\hat c}{\partial y_i}\right)^2\sigma_y^2
=\frac{\sigma_y^2\sum_i x_i^2}{(\sum_i x_i^2)^2}
=\frac{\sigma_y^2}{\sum_i x_i^2}.
$$

Hence

$$
\boxed{\sigma_{\hat c}=3.65\times10^{-7}\,\mathrm{m^2},\qquad
\hat c=(1.809\pm0.037)\times10^{-5}\,\mathrm{m^2}.}
$$

If the period measurement is [independent](../../../../../../independent-random-variables.md) of the [angle](../../../../../../angle.md) measurements, including its calibration uncertainty gives

$$
\frac{\sigma_G}{\hat G}=\sqrt{\left(\frac{\sigma_{\hat c}}{\hat c}\right)^2+
\left(\frac{\sigma_\kappa}{\kappa}\right)^2}=0.0314,
\qquad \hat G=(9.59\pm0.30)\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}.
$$

This last uncertainty includes the stated random measurement errors only. Whether the model describes the data must be checked before treating it as a reliable measurement of the [gravitational constant](../../../../../../gravitational-constant.md).

## ↑ Ancestors (15)

1. [C](../c.md)
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
