<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The force-free [Stokes flow](../../../../../../stokes-flow-split.md) equations are

$$
-\nabla p+\mu\nabla^2\mathbf u=0,
\qquad \nabla\cdot\mathbf u=0.
$$

Put $p=\nabla^2\Pi$. Then $\nabla^2(\mu\mathbf u-\nabla\Pi)=0$, so write

$$
\mu\mathbf u=\nabla\Pi+\boldsymbol\Phi,
\qquad \nabla^2\boldsymbol\Phi=0.
$$

Incompressibility requires $\nabla^2\Pi=-\nabla\cdot\boldsymbol\Phi$. Since $\nabla^2(\mathbf x\cdot\boldsymbol\Phi)=2\nabla\cdot\boldsymbol\Phi$ for harmonic $\boldsymbol\Phi$, take

$$
\Pi=-\frac12\mathbf x\cdot\boldsymbol\Phi+\chi,
\qquad \nabla^2\chi=0.
$$

This gives the [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md)

$$
\boxed{\mu\mathbf u=\boldsymbol\Phi-\frac12\nabla(\mathbf x\cdot\boldsymbol\Phi)+\nabla\chi},
\qquad
\boxed{p=-\nabla\cdot\boldsymbol\Phi}.
$$

For a rotating sphere the boundary data are toroidal, tangent to every concentric sphere, linear in $\boldsymbol\Omega$, and decay at infinity. The harmonic vector field

$$
\boldsymbol\Phi=\mu a^3\frac{\boldsymbol\Omega\times\mathbf x}{r^3},
\qquad \chi=0,
$$

has precisely these symmetries; it is harmonic because its components are derivatives of $1/r$, and $\mathbf x\cdot\boldsymbol\Phi=\nabla\cdot\boldsymbol\Phi=0$. Hence

$$
\boxed{\mathbf u=\frac{a^3}{r^3}\boldsymbol\Omega\times\mathbf x},
\qquad \boxed{p=0}.
$$

The first pressure argument is $p=-\nabla\cdot\boldsymbol\Phi=0$. Independently, this velocity is harmonic, so the Stokes momentum equation gives $\nabla p=0$; matching the ambient pressure sets that constant to zero.

At $r=a$,

$$
\boxed{\frac{\partial\mathbf u}{\partial r}=-2\boldsymbol\Omega\times\mathbf n=-\frac2a\boldsymbol\Omega\times\mathbf x}.
$$

The surface traction is $\boldsymbol\sigma\mathbf n=-3\mu\boldsymbol\Omega\times\mathbf n$. Its moment gives the standard rotational resistance

$$
\boxed{\mathbf G_{\rm fluid}=
\int_{r=a}\mathbf x\times(\boldsymbol\sigma\mathbf n)\,dS
=-8\pi\mu a^3\boldsymbol\Omega}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
