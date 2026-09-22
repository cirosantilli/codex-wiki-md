<h1 id="section-d/12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

**Reflection and central spot.** At a boundary from lower to higher [refractive index](../../../../refractive-index.md), the near-normal electric-field reflection coefficient is negative, $r=(n_1-n_2)/(n_1+n_2)$. This gives a $\pi$ [wave phase](../../../../phase-waves.md) reversal on reflection from the glass plate through the air film. Reflection at the lens's glass-to-air underside has no such reversal. These are consequences of the [Fresnel equations](../../../../fresnel-equations.md) for the reflected [electric field](../../../../electric-field-split.md).

At ideal contact the film thickness is zero, so the two reflected contributions have zero geometrical [optical path difference](../../../../optical-path-difference.md) but a relative $\pi$ phase reversal. They produce [destructive interference](../../../../destructive-interference.md), and the **central spot is dark**. This conclusion concerns the film reflection; other lens surfaces can add a weak background.

**Rings and their radii.** At radial distance $r$, let the air thickness be $t$. The two relevant rays reflect at the upper and lower film interfaces. The lower reflection accumulates an extra round-trip [optical path length](../../../../optical-path-length.md) $2t$, plus the relative $\pi$ reflection shift. As $t$ increases away from contact, alternating constructive and destructive [thin-film interference](../../../../thin-film-interference.md) forms [Newton's rings](../../../../newton-s-rings.md). At near-normal incidence, a bright ring satisfies

$$
\frac{2\pi}{\lambda}(2t)+\pi=2\pi(m+1),\qquad
2t=\left(m+\frac12\right)\lambda,\qquad m=0,1,2,\ldots.
$$

The extended source can illuminate these localized film fringes: each incident contribution interferes with its own two reflected paths; unrelated source points need not be mutually coherent.

For the spherical lens surface, geometry gives $r^2+(R-t)^2=R^2$, so $r^2=2Rt-t^2$. Since $t\ll R$, $t\simeq r^2/(2R)$. Combining the equations yields

$$
\boxed{r_m=\sqrt{R\lambda\left(m+\frac12\right)}.}
$$

The $m=0$ bright ring is the first bright ring around the dark contact point.

**Curvature from ring diameters.** Writing $D_m=2r_m$, subtract the squared diameters to eliminate the unknown initial order:

$$
D_{m+20}^2-D_m^2=4R\lambda(20).
$$

Using [SI](../../../../international-system-of-units.md) units,

$$
\boxed{R=\frac{(7.1\times10^{-3})^2-(3.3\times10^{-3})^2}
{80(500\times10^{-9})}=0.988\,\mathrm m\simeq0.99\,\mathrm m.}
$$

**Liquid-filled film.** With film [refractive index](../../../../refractive-index.md) $n=1.4$, still smaller than both glass indices, there remains exactly one relative reflection phase reversal. The round-trip [optical path length](../../../../optical-path-length.md) is now $2nt$, so

$$
r_m^2=\frac{R\lambda}{n}\left(m+\frac12\right).
$$

Here $\lambda=500\,\mathrm{nm}$ is the illuminating vacuum wavelength, approximately its air value, rather than its shorter value inside the liquid. The ring labelled $m=2$ therefore has diameter

$$
\boxed{D_2=2\sqrt{\frac{(0.988)(500\times10^{-9})(2+1/2)}{1.4}}
=1.878\times10^{-3}\,\mathrm m\simeq1.9\,\mathrm{mm}.}
$$

Filling the gap contracts each ring radius by $1/\sqrt n$ at fixed order and curvature.

## ↑ Ancestors (12)

1. [12](../12.md)
2. [Section D](../../section-d.md)
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
