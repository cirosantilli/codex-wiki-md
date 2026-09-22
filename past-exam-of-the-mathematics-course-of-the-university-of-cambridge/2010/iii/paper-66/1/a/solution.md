<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in the frame in which the distant fluid is stationary, and take the [pressure](../../../../../../pressure.md) at infinity as zero. In the [Unscaled Papkovich–Neuber representation](../../../../../../unscaled-papkovich-neuber-representation.md), choose the harmonic potentials

$$
\boldsymbol\Phi=-\frac{3a}{4r}\mathbf V,\qquad
\chi=\frac{a^3}{4}\frac{\mathbf V\cdot\mathbf x}{r^3}.
$$

Both are harmonic away from the sphere's centre: $1/r$ is harmonic there and $\mathbf V\cdot\mathbf x/r^3=-\mathbf V\cdot\nabla(1/r)$. Substitution into $\mathbf u=\nabla(\mathbf x\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi$, $p=2\mu\nabla\cdot\boldsymbol\Phi$, gives the [translating sphere in Stokes flow](../../../../../../translating-sphere-in-stokes-flow.md):

$$
\boxed{\mathbf u=\left[\frac{3a}{4r}(\mathbf I+\mathbf n\mathbf n)+\frac{a^3}{4r^3}(\mathbf I-3\mathbf n\mathbf n)\right]\mathbf V,\qquad
p=\frac{3\mu a}{2r^2}\mathbf V\cdot\mathbf n.}
$$

Here $\mathbf n=\mathbf x/r$. At $r=a$ the coefficients of $\mathbf I$ sum to one and those of $\mathbf n\mathbf n$ sum to zero, so the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) is satisfied. The field decays at infinity. The [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) enforces the [Stokes equation](../../../../../../stokes-equation.md) and [incompressibility](../../../../../../incompressible-flow.md), and [Uniqueness of Stokes flow](../../../../../../uniqueness-of-stokes-flow.md) identifies the physical solution.

Differentiate radially at fixed direction $\mathbf n$:

$$
\left.\partial_r\mathbf u\right|_{a}
=\left[-\frac{3}{4a}(\mathbf I+\mathbf n\mathbf n)-\frac{3}{4a}(\mathbf I-3\mathbf n\mathbf n)\right]\mathbf V
=\boxed{\frac{3}{2a}(\mathbf n\mathbf n-\mathbf I)\mathbf V.}
$$

On the surface, multiplying the specified [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) by the outward normal from the solid gives

$$
\boldsymbol\sigma\mathbf n=\frac{3\mu}{2a}\left[(\mathbf V\cdot\mathbf n)\mathbf n-\mathbf V-\mathbf n(\mathbf V\cdot\mathbf n)\right]
=-\frac{3\mu}{2a}\mathbf V.
$$

Thus the [surface traction in translating-sphere Stokes flow](../../../../../../surface-traction-in-translating-sphere-stokes-flow.md) is uniform and the fluid's [force](../../../../../../force.md) on the sphere is

$$
\boxed{\mathbf F_{\rm fluid}=\int_{r=a}\boldsymbol\sigma\mathbf n\,dS=-6\pi\mu a\mathbf V.}
$$

This is the [Stokes drag law](../../../../../../stokes-s-law.md); an external [force](../../../../../../force.md) of the opposite sign maintains the motion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
