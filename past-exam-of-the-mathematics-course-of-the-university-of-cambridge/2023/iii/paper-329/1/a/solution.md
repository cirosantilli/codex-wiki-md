<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) writes a homogeneous incompressible [Stokes flow](../../../../../../stokes-flow-split.md) in terms of a harmonic vector field $\boldsymbol\Phi$ and harmonic scalar $\chi$:

$$
2\mu\mathbf u
=\nabla(\mathbf x\mathbin\cdot\boldsymbol\Phi+\chi)
-2\boldsymbol\Phi,
\qquad
p=\nabla\mathbin\cdot\boldsymbol\Phi,
$$

with $\nabla^2\boldsymbol\Phi=0$ and $\nabla^2\chi=0$. The representation satisfies incompressibility because $\nabla^2(\mathbf x\mathbin\cdot\boldsymbol\Phi)=2\nabla\mathbin\cdot\boldsymbol\Phi$, and substitution then verifies the [Stokes equation](../../../../../../stokes-equation.md).

For a sphere translating with constant vector velocity $\mathbf U$, rotational covariance and decay at infinity suggest a harmonic vector monopole and scalar dipole:

$$
\boldsymbol\Phi=-\frac{3\mu a}{2r}\mathbf U,
\qquad
\chi=\frac{\mu a^3}{2}\frac{\mathbf U\mathbin\cdot\mathbf x}{r^3}.
$$

Substitution gives the [translating sphere in Stokes flow](../../../../../../translating-sphere-in-stokes-flow.md)

$$
\boxed{
\mathbf u(\mathbf x)=
\frac{3a}{4r}\left(\mathbf I+
\frac{\mathbf x\mathbf x}{r^2}\right)\mathbf U
+\frac{a^3}{4r^3}\left(\mathbf I-3
\frac{\mathbf x\mathbf x}{r^2}\right)\mathbf U},
$$



$$
\boxed{p(\mathbf x)=
\frac{3\mu a}{2r^3}\mathbf U\mathbin\cdot\mathbf x}.
$$

At $r=a$ the radial tensor terms cancel and $\mathbf u=\mathbf U$, while $\mathbf u\to0$ as $r\to\infty$, so the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) and far-field condition hold. The resulting traction integrates to the [Stokes drag law](../../../../../../stokes-s-law.md) $6\pi\mu a\mathbf U$ in magnitude.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
