<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The observer is static at $r_0$, with [four-velocity](../../../../four-velocity.md) $U=f_0^{-1/2}\partial_t$, where $f_0=1-2m/r_0$. Angles are measured in the observer's [rest frame](../../../../rest-frame.md), using the positive spatial [metric tensor](../../../../metric-tensor.md)

$$
d\ell_{\mathrm{space}}^2=f_0^{-1}dr^2+r_0^2d\phi^2
$$

on the equatorial plane. One cannot directly normalize a photon tangent with the full [Lorentzian metric](../../../../lorentzian-metric.md) to define an angle, because that tangent is null.

At the observer the spatial direction of an outward-moving grazing ray is proportional to $w=A\partial_r+\partial_\phi$, with $A=(dr/d\phi)_{r_0}$. Its angle $\psi=\alpha/2$ to the outward radial direction equals the corresponding sky angle to the inward center of the image. Taking the spatial [inner product](../../../../inner-product-split.md) with $e_r=\partial_r$,

$$
\cos\psi
=\frac{|\langle w,e_r\rangle|}
{\sqrt{\langle w,w\rangle\langle e_r,e_r\rangle}}
=\frac{|A|}{\sqrt{A^2+f_0r_0^2}}.
$$

Consequently

$$
\boxed{
\cos\frac\alpha2
=\left(1+\frac{f_0r_0^2}{A^2}\right)^{-1/2}.
}
$$

The limiting value $A=0$ is understood by continuity.

For a grazing ray the [areal radius](../../../../areal-radius.md) has a turning point at the stellar surface $R$, so $\dot r=0$ there. The radial equation gives

$$
C=\frac{f(R)}{R^2}.
$$

Since $R=4m>3m$, the surface lies outside the [photon sphere](../../../../photon-sphere.md). The function $f/r^2$ decreases for $r>3m$, so this tangential ray can escape to every $r_0>R$ and correctly defines the image's rim. For the specified surface,

$$
f(R)=\frac12,\qquad
C=\frac1{32m^2},\qquad
b=\frac R{\sqrt{f(R)}}=4\sqrt2\,m.
$$

Also $dr/d\phi=-r^2\,du/d\phi$, hence

$$
\boxed{
A^2=r_0^4\left(\frac1{32m^2}-\frac{f_0}{r_0^2}\right),
\qquad
A=\pm r_0\sqrt{\frac{r_0^2}{32m^2}-f_0}.
}
$$

Its sign depends on the orientation of the ray and of $\phi$, and does not affect the [angular diameter](../../../../angular-diameter.md). Substitution gives

$$
\boxed{
\cos\frac\alpha2
=\sqrt{1-\frac{32m^2}{r_0^2}\left(1-\frac{2m}{r_0}\right)},
\qquad
\alpha=2\arcsin\left[
\frac{4\sqrt2\,m}{r_0}\sqrt{1-\frac{2m}{r_0}}
\right].
}
$$

This [apparent angular radius of a spherical star in Schwarzschild spacetime](../../../../apparent-angular-radius-of-a-spherical-star-in-schwarzschild-spacetime.md) has useful limiting checks. As $r_0\downarrow R$, the star occupies a hemisphere, $\alpha\to\pi$. Far away, $\alpha\simeq2b/r_0=8\sqrt2\,m/r_0$: [Schwarzschild light deflection](../../../../schwarzschild-light-deflection.md) increases the apparent radius by a factor $\sqrt2$ relative to the flat-space value $R/r_0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
