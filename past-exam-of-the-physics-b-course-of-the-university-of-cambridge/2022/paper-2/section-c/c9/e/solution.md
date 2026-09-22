<h1 id="section-c/c9/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

[Kirchhoff's law of thermal radiation](../../../../../../kirchhoff-s-law-of-thermal-radiation.md) equates spectral absorptivity and [spectral emissivity](../../../../../../spectral-emissivity.md) at the same [wavelength](../../../../../../wavelength.md) and direction. A surface that is a poor absorber in the thermal [infrared](../../../../../../infrared.md) is also a poor emitter there; a coating cannot be assigned its solar absorption independently of its thermal emission spectrum.

**(i) All-wavelength black paint.** It absorbs the sunlight and also radiates maximally at the spacecraft's own [temperature](../../../../../../temperature-split.md). With the isothermal-sphere assumptions of (d), the limiting black-surface distance is

$$
\boxed{\frac{R_{\min,\rm black}}r=\frac12\left(\frac{T_S}{T_{\max}}\right)^2=\frac12\left(\frac{6000}{600}\right)^2=50.}
$$

The spacecraft can operate at $R\geq50r$ in this model. A surface already assumed to be a [blackbody](../../../../../../blackbody.md) is not improved by another black coating; relative to option (ii), however, this paint permits closer operation.

**(ii) Black at short [wavelengths](../../../../../../wavelength.md) and grey in the [infrared](../../../../../../infrared.md).** By [Wien's displacement law](../../../../../../wien-s-displacement-law.md), changing the [black-body radiation](../../../../../../black-body-radiation.md) [temperature](../../../../../../temperature-split.md) from $6000\,\mathrm K$ to $600\,\mathrm K$ shifts the [wavelength](../../../../../../wavelength.md) peak from about $0.5\,\mu\mathrm m$ to about $5\,\mu\mathrm m$. Most solar [power](../../../../../../power.md) is therefore in the highly absorbing short-wavelength band, whereas most spacecraft emission lies beyond $2\,\mu\mathrm m$, where the [spectral emissivity](../../../../../../spectral-emissivity.md) is reduced. The coating retains most of the heating but suppresses much of the cooling. Under the intended two-band [grey body](../../../../../../grey-body.md) approximation, **option (ii) makes the spacecraft hotter at the same distance and requires a larger minimum distance than black paint.**

To express the comparison without inventing a grey absorptivity, let $\bar\alpha_S$ be [radiometric absorptance](../../../../../../radiometric-absorptance.md) averaged over the solar spectrum and $\bar\epsilon_T$ be emissivity averaged over the spacecraft's own thermal spectrum. The [radiative equilibrium](../../../../../../radiative-equilibrium.md) equation becomes

$$
\bar\alpha_S\sigma T_S^4\frac{r^2}{R^2}=4\bar\epsilon_T\sigma T^4,
\qquad
T=T_S\sqrt{\frac r{2R}}\left(\frac{\bar\alpha_S}{\bar\epsilon_T}\right)^{1/4}.
$$

At the failure threshold,

$$
\boxed{\frac{R_{\min}}r=50\sqrt{\frac{\bar\alpha_S}{\bar\epsilon_{600}}}.}
$$

For an ideal two-band coating take a constant [radiometric absorptance](../../../../../../radiometric-absorptance.md) $g<1$ beyond $\lambda_c=2\,\mu\mathrm m$, and unity below it. If $f(T)$ is the fraction of the [power](../../../../../../power.md) emitted by a [blackbody](../../../../../../blackbody.md) below $\lambda_c$, [Planck's law](../../../../../../planck-s-law.md) gives

$$
f(T)=\frac{15}{\pi^4}\int_{hc/(\lambda_ck_BT)}^\infty\frac{x^3}{e^x-1}\,dx,
\qquad
\bar\alpha_S=g+(1-g)f(T_S),\quad
\bar\epsilon_{600}=g+(1-g)f(600\,\mathrm K).
$$

Since $f(T_S)>f(600\,\mathrm K)$, this model has $\bar\alpha_S>\bar\epsilon_{600}$ and hence $R_{\min}>50r$. The paper supplies neither a numerical value of $g$ nor a detailed spectrum, so no unique numerical distance for the grey paint follows. If its long-wavelength absorption is not approximately grey, the spectrum must be integrated explicitly rather than inferred from a peak alone. A coating designed to improve close approach would instead reflect much of the solar radiation while retaining strong thermal [infrared](../../../../../../infrared.md) emission.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [C9](../../c9.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
