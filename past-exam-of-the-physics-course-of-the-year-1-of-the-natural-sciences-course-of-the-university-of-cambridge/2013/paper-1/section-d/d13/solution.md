<h1 id="section-d/d13/solution">Solution</h1>

↑ **Parent:** [D13](../d13.md)

Substitution into the [wave equation](../../../../../wave-equation-split.md) gives $\partial_x^2\psi+\partial_y^2\psi=-(k_x^2+k_y^2)\psi$ and $\partial_t^2\psi=-\omega^2\psi$. Therefore $\omega^2=c^2(k_x^2+k_y^2)$. The fixed edges at zero are automatically satisfied by the sine factors; the opposite edges require

$$
k_x=\frac{p\pi}{a},\quad k_y=\frac{q\pi}{b},\quad p,q=1,2,\ldots,\qquad
\boxed{f_{pq}=\frac c2\sqrt{\frac{p^2}{a^2}+\frac{q^2}{b^2}}.}
$$

Neither integer may vanish, because that would make the entire displacement zero.

The element's [mass](../../../../../mass.md) is $\rho\,dx\,dy$, and its [speed](../../../../../speed.md) is $-\omega A\sin(k_xx)\sin(k_yy)\sin(\omega t)$. Squaring and multiplying by half its [mass](../../../../../mass.md) gives the requested [energy](../../../../../energy-split.md) [density](../../../../../density.md). The two sine-squared spatial integrals are $a/2$ and $b/2$, so

$$
\boxed{K(t)=\frac{\rho ab\omega^2A^2}{8}\sin^2(\omega t),\qquad
\overline K=\frac{\rho ab\omega^2A^2}{16}.}
$$

There is no [dissipation](../../../../../dissipation.md). The total [mechanical energy](../../../../../mechanical-energy.md) equals the maximum [kinetic energy](../../../../../kinetic-energy.md), giving

$$
\boxed{U(t)=\frac{\rho ab\omega^2A^2}{8}\cos^2(\omega t).}
$$

Equivalently, integrate the small-slope tension [energy](../../../../../energy-split.md) $\rho c^2|\nabla\psi|^2/2$ and use the [dispersion relation](../../../../../dispersion-relation-split.md).

For $b=4a/5$, the two lowest [modes](../../../../../mode-statistics.md) are $(p,q)=(1,1)$ and $(2,1)$:

$$
\boxed{f_{11}=\frac{\sqrt{41}\,c}{8a},\qquad
f_{21}=\frac{\sqrt{89}\,c}{8a}.}
$$

The fundamental has one [antinode](../../../../../antinode.md) at $(a/2,b/2)$ and no interior nodal line. The next [mode](../../../../../mode-statistics.md) has a [node](../../../../../node-dynamical-systems.md) along $x=a/2$ and opposite-sign [antinodes](../../../../../antinode.md) at $(a/4,b/2)$ and $(3a/4,b/2)$. Every boundary is a [node](../../../../../node-dynamical-systems.md).

<a id="section-d/d13/image-original-displacement-maps-for-the-two-lowest-modes-of-a-rectangular-membrane-showing-nodal-lines-and-signed-antinodes"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1-ia2013-membrane-modes.png)

**[Figure 3](#section-d/d13/image-original-displacement-maps-for-the-two-lowest-modes-of-a-rectangular-membrane-showing-nodal-lines-and-signed-antinodes). Original displacement maps for the two lowest modes of a rectangular membrane, showing nodal lines and signed antinodes**.

The square fundamental has $f=c\sqrt2/(2\beta a)$. Equating it to $f_{11}$ gives

$$
\boxed{\beta=\sqrt{\frac{32}{41}}=0.88345.}
$$

At the same peak displacement [amplitude](../../../../../wave-amplitude.md) and [frequency](../../../../../frequency.md), time-averaged [kinetic energy](../../../../../kinetic-energy.md) is proportional to membrane area. Therefore

$$
\boxed{\frac{\overline K_{\rm square}}{\overline K_{\rm rectangle}}
=\frac{\beta^2a^2}{a(0.8a)}=\frac{40}{41}.}
$$

The reciprocal ratio is $41/40$ if the rectangle is placed first.

## ↑ Ancestors (13)

1. [D13](../d13.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
