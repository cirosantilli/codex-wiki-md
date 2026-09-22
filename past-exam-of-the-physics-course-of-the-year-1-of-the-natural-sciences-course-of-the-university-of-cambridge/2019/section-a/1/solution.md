<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Rearrange the supplied form of [Kepler's third law](../../../../kepler-s-third-law.md) to make the [gravitational constant](../../../../gravitational-constant.md) the subject:

$$
G=\frac{4\pi^2a^3}{MT^2}.
$$

Convert the [semi-major axis](../../../../semi-major-axis.md) and [orbital period](../../../../orbital-period.md) to [SI](../../../../international-system-of-units.md) units before substitution:

$$
a=1.491\times10^{11}\,\mathrm m,\qquad
T=365.3\times86400\,\mathrm s=3.156192\times10^7\,\mathrm s.
$$

The central value is therefore

$$
G=\frac{4\pi^2(1.491\times10^{11})^3}
{(1.99\times10^{30})(3.156192\times10^7)^2}
=6.60105\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}.
$$

For [monomial uncertainty propagation](../../../../monomial-uncertainty-propagation.md), [logarithmic differentiation](../../../../logarithmic-differentiation.md) gives

$$
\frac{dG}{G}=3\frac{da}{a}-\frac{dM}{M}-2\frac{dT}{T}.
$$

If the quoted errors are [independent](../../../../independent-random-variables.md) [standard uncertainties](../../../../standard-uncertainty.md), the [variances](../../../../variance-split.md) of these contributions add:

$$
\left(\frac{\sigma_G}{G}\right)^2
=9\left(\frac{1.1}{149.1}\right)^2+(0.01)^2
+4\left(\frac{0.5}{365.3}\right)^2
=(0.0244408)^2.
$$

Thus $\sigma_G=1.61335\times10^{-12}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$, and the measured result under that statistical convention is

$$
\boxed{G=(6.60\pm0.16)\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}.}
$$

The [semi-major axis](../../../../semi-major-axis.md) measurement supplies the largest individual contribution to the relative uncertainty.

The paper does not specify whether its errors are statistical uncertainties or bounds. If they are maximum input errors, the first-order worst-case [error propagation](../../../../propagation-of-uncertainty.md) estimate adds magnitudes:

$$
\frac{\Delta G}{G}\lesssim3\frac{1.1}{149.1}+0.01+2\frac{0.5}{365.3}
=0.0348703,
\qquad
\boxed{\Delta G\simeq0.23\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}.}
$$

[Correlation](../../../../pearson-correlation-coefficient.md) between input errors would instead require the [covariance](../../../../covariance.md) terms in the general [propagation of uncertainty](../../../../propagation-of-uncertainty.md) formula; they are not specified.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
