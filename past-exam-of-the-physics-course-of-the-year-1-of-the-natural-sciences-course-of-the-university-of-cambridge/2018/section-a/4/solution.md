<h1 id="section-a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**First intensity minimum.** In [Fraunhofer diffraction](../../../../fraunhofer-diffraction.md), the path difference between adjacent slits is $d\sin\theta$, so the relative [wave phase](../../../../phase-waves.md) is $\delta=2\pi d\sin\theta/\lambda_1$. Summing the $N$ equal [complex amplitudes](../../../../complex-amplitude.md) as a [geometric series](../../../../geometric-series.md) gives the [diffraction grating](../../../../diffraction-grating.md) interference factor

$$
I(\theta)\propto
\left|\sum_{j=0}^{N-1}e^{ij\delta}\right|^2
=\frac{\sin^2(N\delta/2)}{\sin^2(\delta/2)}.
$$

The central maximum has $\delta=0$. Its nearest zero occurs at $N\delta/2=\pi$, where the denominator is nonzero. Thus

$$
\sin\theta_{\min}=\frac{\lambda_1}{Nd}
=\frac{640\times10^{-9}}{10(80\times10^{-6})}=8.00\times10^{-4},
\qquad
\boxed{|\theta_{\min}|=8.00\times10^{-4}\,\mathrm{rad}=0.0458^\circ.}
$$

There is a symmetric first zero on each side of the incident direction. The narrow slits are treated as having a sufficiently broad [single-slit diffraction](../../../../single-slit-diffraction.md) envelope.

**Wavelength resolution and the missing order specification.** Adopt the [Rayleigh criterion](../../../../rayleigh-criterion.md): the principal maximum of one [wavelength](../../../../wavelength.md) lies at the adjacent minimum of the other in the same nonzero [diffraction order](../../../../diffraction-order.md) $m$. For $\lambda_2>\lambda_1$ and $m>0$, those directions obey

$$
d\sin\theta=m\lambda_2
=\left(m+\frac1N\right)\lambda_1.
$$

Consequently the ideal [resolving power of a diffraction grating](../../../../resolving-power-of-a-diffraction-grating.md) is $\lambda_1/\Delta\lambda=mN$, giving

$$
\boxed{\Delta\lambda_{\min,m}=\frac{\lambda_1}{mN}
=\frac{64}{m}\,\mathrm{nm}.}
$$

The usual first-order reading therefore gives **$64\,\mathrm{nm}$**. Zero [diffraction order](../../../../diffraction-order.md) cannot separate the two [wavelengths](../../../../wavelength.md), because both central maxima coincide.

The paper does not specify which [diffraction order](../../../../diffraction-order.md) is observed, so $64\,\mathrm{nm}$ is not an order-independent minimum. In the ideal infinitely narrow-slit model, the largest usable order for this positive wavelength separation must satisfy $(m+1/N)\lambda_1\le d$. Since $d/\lambda_1=125$, this permits $m\le124$, giving the formal all-order result

$$
\boxed{\Delta\lambda_{\min,124}=0.516\,\mathrm{nm}.}
$$

That pair meets the criterion at $\theta\simeq83.1^\circ$. Order $125$ of $\lambda_1$ is at grazing incidence and the corresponding longer-wavelength peak cannot propagate. In a real device, finite slit width, weak high-order intensity and screen acceptance may prevent such an extreme order from being used; those data are absent. Thus the specified-order expression, and $64\,\mathrm{nm}$ when first order is intended, are the defensible resolution answers under the stated criterion.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Section A](../../section-a.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
