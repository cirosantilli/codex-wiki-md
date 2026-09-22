<h1 id="section-e/14/solution">Solution</h1>

↑ **Parent:** [14](../14.md)

**Field of discrete masses.** [Newton's law of universal gravitation](../../../../newton-s-law-of-universal-gravitation-split.md) and [superposition](../../../../superposition-principle.md) give the [gravitational field](../../../../gravitational-field.md) away from the source points:

$$
\boxed{\mathbf g(\mathbf r)=-G\sum_{i=1}^N
M_i\frac{\mathbf r-\mathbf r_i}{|\mathbf r-\mathbf r_i|^3}.}
$$

It is the [force](../../../../force-split.md) per unit test [mass](../../../../mass.md), with units $\mathrm{N\,kg^{-1}}=\mathrm{m\,s^{-2}}$, and points toward each positive source [mass](../../../../mass.md).

**Infinite circular cylindrical rod.** Let $b$ be the radius of the circular cross-section, so $A=\pi b^2$, and write $\lambda=\rho A$ for the [linear mass density](../../../../linear-mass-density.md). Choose a coaxial cylindrical [Gaussian surface](../../../../gaussian-surface.md) with radius $r>b$ and length $L$. Translation and rotation symmetry make $\mathbf g=g_r(r)\widehat{\mathbf r}$. The end caps have zero field [flux](../../../../flux.md) because their normals are axial; on the curved surface the outward-normal component is the constant negative value $g_r$. [Gauss's law for gravity](../../../../gauss-s-law-for-gravity.md) therefore gives

$$
\oint\mathbf g\cdot d\mathbf S=2\pi rL g_r
=-4\pi G(\rho AL),
\qquad
\boxed{\mathbf g(r)=-\frac{2G\rho A}{r}\widehat{\mathbf r}\quad(r>b).}
$$

The [gravitational field of an infinite uniform cylinder](../../../../gravitational-field-of-an-infinite-uniform-cylinder.md) inside the material instead has enclosed [mass](../../../../mass.md) $\rho\pi r^2L$, giving $g_r=-2\pi G\rho r$. The exterior result assumes a circular cylindrical rod; area by itself would not specify the exact near field of a noncircular cross-section.

<a id="section-e/14/image-gaussian-cylinder-cross-section-for-an-infinite-rod-and-the-circular-speed-curve-of-a-finite-line-rod"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018-ia-physics-q14-rod-orbits.png)

**[Figure 4](#section-e/14/image-gaussian-cylinder-cross-section-for-an-infinite-rod-and-the-circular-speed-curve-of-a-finite-line-rod). Gaussian-cylinder cross-section for an infinite rod and the circular-speed curve of a finite line rod**.

In the left panel the dashed circle is a transverse section of the coaxial [Gaussian surface](../../../../gaussian-surface.md); the field points inward and the surface normals outward. Its side area is $2\pi rL$.

For an exterior [circular orbit](../../../../circular-orbit.md), [Newton's second law](../../../../newton-s-second-law.md) equates the [force](../../../../force-split.md) required for [centripetal acceleration](../../../../centripetal-acceleration.md) to gravity:

$$
\frac{mv^2}{r}=m\frac{2G\rho A}{r},\qquad
\boxed{v=\sqrt{2G\rho A}=\sqrt{2G\lambda}.}
$$

The orbital [speed](../../../../speed.md) is independent of radius and of the orbiting object's [mass](../../../../mass.md), for orbits outside the infinite rod.

**Finite rod.** Taking the supplied field as the [gravitational field of a finite uniform line segment](../../../../gravitational-field-of-a-finite-uniform-line-segment.md), the corresponding balance at radius $R$ is

$$
\frac{v^2}{R}=\frac{GM}{R\sqrt{R^2+a^2}},\qquad
\boxed{v(R)=\left(\frac{GM}{\sqrt{R^2+a^2}}\right)^{1/2}
=\frac{\sqrt{GM}}{(R^2+a^2)^{1/4}}.}
$$

Since $M=2a\rho A=2a\lambda$, its two limits are

$$
\boxed{R\ll a:\quad v\simeq\sqrt{\frac{GM}{a}}=\sqrt{2G\rho A},
\qquad R\gg a:\quad v\simeq\sqrt{\frac{GM}{R}}.}
$$

The first reproduces the infinite-rod result: a nearby observer sees a very long source. The second is the familiar [circular orbit](../../../../circular-orbit.md) speed about a [point mass](../../../../point-mass.md), since a distant observer cannot resolve the rod's length. The dimensionless curve is

$$
\frac{v}{\sqrt{GM/a}}=[1+(R/a)^2]^{-1/4}.
$$

It starts at a constant plateau and decreases smoothly, approaching an $R^{-1/2}$ dependence far away. For $R>0$, $dv/dR=-\sqrt{GM}\,R/[2(R^2+a^2)^{5/4}]<0$, consistent with the sketch.

**Derivation of the finite-rod field.** Put the source along $-a<z<a$ on the $z$ axis. In its central perpendicular plane, an element $dm=\lambda\,dz$ is at distance $s=\sqrt{r^2+z^2}$. Its field magnitude is $G\lambda\,dz/s^2$, and its inward radial component has the extra factor $r/s$. The axial components cancel between $z$ and $-z$. Thus

$$
g_r=-G\lambda r\int_{-a}^a\frac{dz}{(r^2+z^2)^{3/2}}
=-G\lambda r\left[\frac{z}{r^2\sqrt{r^2+z^2}}\right]_{-a}^{a}
=-\frac{2aG\lambda}{r\sqrt{r^2+a^2}}.
$$

Replacing $2a\lambda$ by $M$ gives

$$
\boxed{\mathbf g(r)=-\frac{GM}{r\sqrt{r^2+a^2}}\widehat{\mathbf r}.}
$$

The integral treats the source as a [line mass](../../../../line-mass.md). For a finite cylinder of nonzero cross-section, the displayed finite-rod formula is a thin-rod approximation, not an exact field for all $r$. Its near-rod limit should therefore be read as $b\ll R\ll a$, keeping the orbit outside the material; the apparent line-source singularity at $r=0$ does not describe the interior of a real cylinder.

## ↑ Ancestors (12)

1. [14](../14.md)
2. [Section E](../../section-e.md)
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
