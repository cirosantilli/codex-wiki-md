<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At radius $r$, radiation of luminosity $L$ gives matter of flux-mean [opacity](../../../../../../opacity.md) $\kappa$ the outward acceleration

$$
a_{\rm rad}=\frac{\kappa L}{{4\pi r^2c}}.
$$

Equating this with the gravitational acceleration $GM_{\rm BH}/r^2$ gives the [Eddington luminosity](../../../../../../eddington-luminosity.md)

$$
\boxed{L_{\rm Edd}=\frac{4\pi GM_{\rm BH}c}{\kappa}.}
$$

Let $L=fL_{\rm Edd}$ and let $\mathcal M(r)$ be the [radiative force multiplier](../../../../../../radiative-force-multiplier.md) relative to the Compton or electron-scattering acceleration. A steady spherical wind obeys [mass conservation](../../../../../../mass-conservation.md) $\dot M_w=4\pi r^2\rho v$ and the radial [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md)

$$
\boxed{v\frac{dv}{dr}=-\frac1\rho\frac{dP}{dr}
-\frac{GM_{\rm BH}}{r^2}\left[1-f\mathcal M(r)\right].}
$$

When gas pressure is negligible, radiation accelerates the wind locally if $f\mathcal M>1$. Electron scattering alone has $\mathcal M\simeq1$, so it launches a wind only near or above the [Eddington ratio](../../../../../../eddington-ratio.md) $f=1$. Bound-free absorption, spectral lines, or dust can give $\mathcal M\gg1$ and allow a sub-Eddington source to launch a wind, provided the gas is not so highly ionized that those extra opacities disappear. A wind that has already acquired sufficient kinetic energy may coast through a region where $f\mathcal M<1$, but such a region cannot launch a cold wind from rest.

Write the [innermost stable circular orbit](../../../../../../innermost-stable-circular-orbit.md) as

$$
R_{\rm ISCO}=r_{\rm ISCO}(s_{\rm BH})\frac{GM_{\rm BH}}{c^2}.
$$

Estimating the emitting area as $4\pi R_{\rm ISCO}^2$, the [Stefan–Boltzmann law](../../../../../../stefan-boltzmann-law.md) gives

$$
4\pi R_{\rm ISCO}^2\sigma_{\rm SB}T_{\rm BB}^4\sim fL_{\rm Edd},
$$

and hence

$$
\boxed{T_{\rm BB}\sim
\left(\frac{fc^5}{\kappa\sigma_{\rm SB}G M_{\rm BH}}\right)^{1/4}
r_{\rm ISCO}^{-1/2}.}
$$

Thus $T_{\rm BB}\propto M_{\rm BH}^{-1/4}$ at fixed $f$ and opacity: a larger black hole radiates from an area growing as $M_{\rm BH}^2$, faster than its Eddington luminosity grows. Prograde [black-hole spin](../../../../../../black-hole-spin.md) moves the ISCO inward and raises the characteristic temperature, whereas retrograde spin moves it outward and lowers the temperature. Relativistic transfer and the radial temperature profile change the numerical coefficient, not these leading scalings.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
