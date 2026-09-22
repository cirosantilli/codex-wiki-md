<h1 id="11a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Rotational symmetry of the [vector field](../../../../../../vector-field.md) means $\mathbf F(r\mathbf n)=h(r)\mathbf n$: rotations fixing $\mathbf n$ force the field to be parallel to $\mathbf n$, and rotations between directions make its magnitude depend only on $r$. Its [flux integral](../../../../../../flux-integral.md) over the radius-$r$ [sphere](../../../../../../sphere.md) is $4\pi r^2h(r)$. Applying the flux identity from part (i) to the ball, with the spherically symmetric source, gives

$$
4\pi r^2h(r)=4\pi\int_0^r f(s)s^2\,ds.
$$

Therefore the [origin-regular spherical Poisson flux law](../../../../../../origin-regular-spherical-poisson-flux-law.md) is

$$
\boxed{\mathbf F(\mathbf x)=\frac{\mathbf x}{|\mathbf x|^3}
\int_0^{|\mathbf x|}f(s)s^2\,ds.}
$$

Only source values at $s\le|\mathbf x|$ occur. Changing the exterior source can change the scalar potential by an interior constant, but cannot change this radial [gradient](../../../../../../gradient.md). Regularity on all of $\mathbb R^3$, inherited from the [Poisson equation](../../../../../../poisson-equation.md) setting, matters: on a punctured domain alone an additional $C\mathbf x/r^3$ would have zero [divergence](../../../../../../divergence.md) away from the origin and would not be fixed by the local source. It is excluded here by the origin regularity needed for the ball flux identity.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
