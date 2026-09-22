<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand the given translating-sphere [Stokes flow](../../../../stokes-flow-split.md) into its [Stokeslet](../../../../stokeslet.md) and [potential dipole](../../../../potential-dipole.md) parts:

$$
\mathbf u=\frac{3a}{4}\left(\frac{\mathbf U}{r}+\frac{(\mathbf U\cdot\mathbf x)\mathbf x}{r^3}\right)
+\frac{a^3}{4}\left(\frac{\mathbf U}{r^3}-\frac{3(\mathbf U\cdot\mathbf x)\mathbf x}{r^5}\right).
$$

The second parenthesis is $\nabla[(\mathbf U\cdot\mathbf x)/r^3]$ and has zero curl outside the sphere. For the first,

$$
\nabla\times\frac{\mathbf U}{r}=\frac{\mathbf U\times\mathbf x}{r^3},\qquad
\nabla\times\frac{(\mathbf U\cdot\mathbf x)\mathbf x}{r^3}=\frac{\mathbf U\times\mathbf x}{r^3}.
$$

Thus the [vorticity of translating-sphere Stokes flow](../../../../vorticity-of-translating-sphere-stokes-flow.md) is

$$
\boxed{\boldsymbol\omega=\nabla\times\mathbf u=\frac{3a}{2}\frac{\mathbf U\times\mathbf x}{r^3}.}
$$

The result is independent of the irrotational finite-size dipole correction. It holds in the exterior $r>a$; the singular solid harmonics are used only outside their source.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
