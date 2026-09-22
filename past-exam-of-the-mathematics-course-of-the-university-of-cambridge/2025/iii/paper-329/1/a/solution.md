<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) writes a homogeneous [Stokes flow](../../../../../../stokes-flow-split.md) in terms of a [harmonic vector field](../../../../../../harmonic-function.md) $\boldsymbol\Phi$ and a harmonic scalar $\chi$ as

$$
\mu\mathbf u=\boldsymbol\Phi-\frac12\nabla(\mathbf x\mathbin\cdot\boldsymbol\Phi)+\nabla\chi,
\qquad
p=-\nabla\mathbin\cdot\boldsymbol\Phi.
$$

For translation, rotational symmetry and decay at infinity restrict the trial harmonic fields to the fundamental harmonic $1/r$ and its directional derivatives contracted with $\mathbf U$. For rotation, the only decaying isotropic axial-vector field with the required boundary value is proportional to $\boldsymbol\Omega\times\mathbf x/r^3$. Matching the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) $\mathbf u=\mathbf U+\boldsymbol\Omega\times\mathbf x$ at $r=a$ gives the superposition of the [translating sphere in Stokes flow](../../../../../../translating-sphere-in-stokes-flow.md) and the [rotating sphere in Stokes flow](../../../../../../rotating-sphere-in-stokes-flow.md):

$$
\boxed{
\mathbf u=
\frac{3a}{4r}\left(\mathbf I+\frac{\mathbf x\mathbf x}{r^2}\right)\mathbf U
+\frac{a^3}{4r^3}\left(\mathbf I-3\frac{\mathbf x\mathbf x}{r^2}\right)\mathbf U
+\frac{a^3}{r^3}\boldsymbol\Omega\times\mathbf x,
\qquad
p=\frac{3\mu a}{2r^3}\mathbf U\mathbin\cdot\mathbf x .}
$$

Each term decays at infinity, and direct substitution at $r=a$ gives the prescribed rigid velocity.

When $\mathbf U=0$, the pressure is constant and may be set to zero. Differentiating the rotational velocity and using the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) gives

$$
\boxed{
\boldsymbol\sigma
=-\frac{3\mu a^3}{r^5}
\left[(\boldsymbol\Omega\times\mathbf x)\mathbf x
+\mathbf x(\boldsymbol\Omega\times\mathbf x)\right].}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
