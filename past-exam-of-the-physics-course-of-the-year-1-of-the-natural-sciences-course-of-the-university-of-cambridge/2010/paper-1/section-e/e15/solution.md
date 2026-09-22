<h1 id="section-e/e15/solution">Solution</h1>

↑ **Parent:** [E15](../e15.md)

For [point masses](../../../../../point-mass.md), Newton's [force](../../../../../force-split.md) is attractive along their separation with magnitude $Gm_1m_2/r^2$. Treat the narrow rod as uniform, with [linear mass density](../../../../../linear-mass-density.md) $\mu=M/(2a)$; a [mass](../../../../../mass.md) profile would otherwise be needed beyond total [mass](../../../../../mass.md) and [length](../../../../../length.md).

For [axial and transverse gravity of a uniform rod](../../../../../axial-and-transverse-gravity-of-a-uniform-rod.md), on the axis at $b>a$, integrating the element [force](../../../../../force-split.md) gives

$$
\boxed{F_1=Gm\mu\int_{-a}^a\frac{dx}{(b-x)^2}=\frac{GMm}{b^2-a^2},}
$$

directed toward the rod. On the perpendicular bisector, axial components cancel and transverse components add:

$$
\boxed{F_2=Gm\mu r\int_{-a}^a\frac{dx}{(x^2+r^2)^{3/2}}=\frac{GMm}{r\sqrt{r^2+a^2}}.}
$$

At $r=b\gg a$,

$$
F_1=\frac{GMm}{b^2}\left[1+\frac{a^2}{b^2}+O(a^4/b^4)\right],\quad
F_2=\frac{GMm}{b^2}\left[1-\frac{a^2}{2b^2}+O(a^4/b^4)\right].
$$

Both approach the point-mass [force](../../../../../force-split.md), but $F_1/F_2=1+3a^2/(2b^2)+O(a^4/b^4)$, so the axial attraction is slightly larger.

For a [circular orbit perpendicular to a uniform rod](../../../../../circular-orbit-perpendicular-to-a-uniform-rod.md), rotational [symmetry](../../../../../symmetry-physics.md) about the rod makes a centred [circular orbit](../../../../../circular-orbit.md) possible in its perpendicular-bisector plane. With $m\ll M$, centrifugal balance gives

$$
\boxed{v(r)=\sqrt{\frac{GM}{\sqrt{r^2+a^2}}}
=\sqrt{\frac{GM}{a}}[1+(r/a)^2]^{-1/4}.}
$$

For $r\gg a$, it is Keplerian, $v\sim\sqrt{GM/r}$. For rod thickness $\ll r\ll a$, the [force](../../../../../force-split.md) approximates that of an infinite line and **$v\to\sqrt{GM/a}$**, a flat [speed](../../../../../speed.md) limit rather than a divergence.

<a id="section-e/e15/image-circular-speed-around-a-uniform-rod"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1-ia2010-rod-orbit.png)

**[Figure 5](#section-e/e15/image-circular-speed-around-a-uniform-rod). Circular speed around a uniform rod**. Original orbital speed normalized by sqrt(GM/a), against perpendicular orbit radius divided by the rod half-length. The small-radius plateau and large-radius Kepler asymptote are marked; the zero-thickness rod approximation requires orbit radius larger than the physical rod thickness.

## ↑ Ancestors (13)

1. [E15](../e15.md)
2. [Section E](../../section-e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
