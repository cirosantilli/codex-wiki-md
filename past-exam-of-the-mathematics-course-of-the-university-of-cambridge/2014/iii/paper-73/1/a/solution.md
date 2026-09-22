<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A convenient normalization of the [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) uses a harmonic vector $\mathbf h$ and harmonic scalar $\phi$:

$$
\boxed{\mathbf u=\mathbf h-\tfrac12\nabla(\mathbf x\cdot\mathbf h+\phi),
\qquad p=-\mu\nabla\cdot\mathbf h.}
$$

Indeed, $\Delta(\mathbf x\cdot\mathbf h)=2\nabla\cdot\mathbf h$, so $\nabla\cdot\mathbf u=0$ and $\mu\Delta\mathbf u=\nabla p$. This is a rescaling of the usual harmonic-potential representation of [Stokes flow](../../../../../../stokes-flow-split.md).

Measure $\mathbf x$ from the sphere center, set $r=|\mathbf x|$ and $\mathbf n=\mathbf x/r$. A translational vector harmonic $\mathbf U/r$ provides the decaying $1/r$ [force](../../../../../../force.md) field, while the scalar dipole $(\mathbf U\cdot\mathbf x)/r^3$ adjusts the surface [velocity](../../../../../../velocity.md) without changing that leading far field. For rotation, $(\boldsymbol\Omega\times\mathbf x)/r^3$ is harmonic, divergence-free and perpendicular to $\mathbf x$. Thus try

$$
\mathbf h=A\frac{\mathbf U}{r}+B\frac{\boldsymbol\Omega\times\mathbf x}{r^3},
\qquad\phi=C\frac{\mathbf U\cdot\mathbf x}{r^3}.
$$

The translational [velocity](../../../../../../velocity.md) is $\frac A{2r}(I+\mathbf n\mathbf n)\mathbf U-\frac C{2r^3}(I-3\mathbf n\mathbf n)\mathbf U$. Matching its independent tangential and radial components at $r=a$ gives $A=3a/2$, $C=-a^3/2$; matching rotation gives $B=a^3$. Consequently

$$
\boxed{\mathbf u=\left[\frac{3a}{4r}(I+\mathbf n\mathbf n)
+\frac{a^3}{4r^3}(I-3\mathbf n\mathbf n)\right]\mathbf U
+\frac{a^3}{r^3}\boldsymbol\Omega\times\mathbf x,\qquad
p=\frac{3\mu a}{2r^3}\mathbf U\cdot\mathbf x.}
$$

This superposes the [translating sphere in Stokes flow](../../../../../../translating-sphere-in-stokes-flow.md) and the [rotating sphere in Stokes flow](../../../../../../rotating-sphere-in-stokes-flow.md). It is exactly $\mathbf U+\boldsymbol\Omega\times\mathbf x$ at the sphere and tends to zero at infinity; the additive ambient [pressure](../../../../../../pressure.md) is set to zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
