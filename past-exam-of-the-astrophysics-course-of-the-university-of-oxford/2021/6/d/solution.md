<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the uniform thin [galactic disk](../../../../galactic-disk.md) have outer radius $R_d$ and [surface mass density](../../../../projected-surface-mass-density.md) $\Sigma=M/(\pi R_d^2)$, where $M$ is the [mass](../../../../mass.md) calculated in [a](../a.md). If the redistribution retains the stated outer radius, set $R_d=16\ \mathrm{kpc}$; otherwise $M$ alone does not determine both $R_d$ and $\Sigma$.

A ring of radius $s$ and width $ds$ has [mass](../../../../mass.md) $dM=2\pi\Sigma s\,ds$. By axial symmetry its transverse gravitational force components cancel. At signed height $z$, its vertical force on a [star](../../../../star.md) of [mass](../../../../mass.md) $m$ is

$$
dF_z=-\frac{Gm\,z\,dM}{(s^2+z^2)^{3/2}}.
$$

Integrating the rings gives, for $z\ne0$,

$$
\begin{aligned}
F_z&=-2\pi Gm\Sigma z\int_0^{R_d}\frac{s\,ds}{(s^2+z^2)^{3/2}}\\
&=-2\pi Gm\Sigma z\left(\frac1{|z|}-\frac1{\sqrt{z^2+R_d^2}}\right).
\end{aligned}
$$

Thus

$$
\boxed{\mathbf F(z)=-2\pi Gm\Sigma\left[\operatorname{sgn}z-\frac z{\sqrt{z^2+R_d^2}}\right]\hat{\mathbf z}.}
$$

For a positive distance above the plane, this is $\mathbf F=-2\pi Gm\Sigma[1-z/\sqrt{z^2+R_d^2}]\hat{\mathbf z}$, directed toward the disk. With $R_d=16\ \mathrm{kpc}$, the inferred $\Sigma\simeq178.3M_\odot\,\mathrm{pc^{-2}}$ sets its normalization.

The far-field expansion gives $F_z\simeq-GMm\operatorname{sgn}(z)/z^2$, as required for a point-like total [mass](../../../../mass.md). Close to either face, $F_z\to\mp2\pi Gm\Sigma$, the infinite-sheet limit. The ideal zero-thickness model has a jump in gravitational field at $z=0$; the formula is understood through its one-sided limits. Its symmetric mean is zero on the plane, and a disk of finite thickness resolves the discontinuity.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
