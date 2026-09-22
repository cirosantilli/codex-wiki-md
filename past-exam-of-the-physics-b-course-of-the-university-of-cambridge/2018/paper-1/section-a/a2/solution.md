<h1 id="section-a/a2/solution">Solution</h1>

↑ **Parent:** [A2](../a2.md)

Let the signed axial [velocity](../../../../../velocity.md) on the axis be $w(z)$. Smooth [axisymmetric flow](../../../../../axisymmetric-flow.md) has $u_z(r,z)=w(z)+O(r^2)$ and regular radial velocity at $r=0$. The [incompressible flow](../../../../../incompressible-flow.md) condition in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) is

$$
\frac1r\frac{\partial(ru_r)}{\partial r}+\frac{\partial u_z}{\partial z}=0.
$$

To leading order near the axis, integrate $\partial_r(ru_r)=-rw'(z)$ from zero to $r$. The integration constant vanishes by regularity, giving the [near-axis radial velocity in incompressible axisymmetric flow](../../../../../near-axis-radial-velocity-in-incompressible-axisymmetric-flow.md),

$$
u_r=-\frac r2w'(z)+O(r^3).
$$

With the usual signed interpretation $w(z)=A/z^3$,

$$
\boxed{u_r(r,z)\simeq\frac{3Ar}{2z^4},\qquad r\ll|z|.}
$$

For $A>0$ this is outward: the outward axial flow slows as its distance from the origin grows, and incompressibility requires radial spreading. Here $A$ has units $\mathrm{m^4\,s^{-1}}$, so the answer is a speed.

The source specifies a magnitude rather than an unambiguous signed component. On $z>0$, reversing the axial flow while keeping its magnitude would reverse the radial answer. The general relation $u_r=-rw'/2$ makes that dependence explicit; the boxed expression adopts $u_z=A/z^3$, outward on both halves of the axis.

## ↑ Ancestors (14)

1. [A2](../a2.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
