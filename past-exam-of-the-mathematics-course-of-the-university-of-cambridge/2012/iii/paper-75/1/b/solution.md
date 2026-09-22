<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) in the convention

$$
\mathbf u=\boldsymbol\Phi-\tfrac12\nabla(\mathbf x\cdot\boldsymbol\Phi+\chi),
\qquad p=-\mu\nabla\cdot\boldsymbol\Phi,
\qquad \nabla^2\boldsymbol\Phi=\mathbf0,\quad\nabla^2\chi=0.
$$

It gives $\nabla\cdot\mathbf u=0$ and $\mu\nabla^2\mathbf u=-\mu\nabla(\nabla\cdot\boldsymbol\Phi)=\nabla p$. Additive pressure constants are immaterial.

Let $q=\mathbf x\cdot\mathbf E\mathbf x$, with $\mathbf E$ symmetric and traceless. The harmonic vector $\mathbf E\mathbf x/r^3$ is a derivative of $1/r$. The scalar $q/r^5$ is a decaying degree-two harmonic because $q$ is a harmonic homogeneous quadratic. These [Papkovich potentials for a strained sphere](../../../../../../papkovich-potentials-for-a-strained-sphere.md) have precisely the strain symmetry and decay required for the disturbance, so try

$$
\boldsymbol\Phi=A\frac{\mathbf E\mathbf x}{r^3},\qquad \chi=B\frac q{r^5}.
$$

Substitution gives

$$
\mathbf u'=\frac{3A}{2}\frac{q\mathbf x}{r^5}-B\frac{\mathbf E\mathbf x}{r^5}
+\frac{5B}{2}\frac{q\mathbf x}{r^7}.
$$

At $r=a$, require $\mathbf u'=-\mathbf E\mathbf x$. The independent vector structures give $B=a^5$ and $A=-5a^3/3$. **The disturbance for a [sphere in a uniform straining Stokes flow](../../../../../../sphere-in-a-uniform-straining-stokes-flow.md) is**

$$
\boxed{\mathbf u'=-\frac{a^5}{r^5}\mathbf E\mathbf x
-\frac{5a^3}{2r^5}\left(1-\frac{a^2}{r^2}\right)q\mathbf x,\qquad
p'=-5\mu a^3\frac q{r^5}.}
$$

It decays at infinity and satisfies no slip exactly at the sphere. Its leading far field is a [stresslet](../../../../../../force-dipole-flow.md), of velocity scale $Ea^3/r^2$.

A force-free sphere in a linear background translates with $\mathbf U_0$, by [Faxén's first law](../../../../../../faxen-s-first-law.md), and a couple-free sphere rotates with the background rigid-body rotation $\boldsymbol\Omega$, by [Faxén's rotational law](../../../../../../faxen-s-rotational-law.md). Uniform translation and solid-body rotation can then be matched without disturbance. The remaining relative boundary velocity is exactly $-\mathbf E\mathbf x$. The [Linearity of Stokes flow](../../../../../../linearity-of-stokes-flow.md) and [Uniqueness of Stokes flow](../../../../../../uniqueness-of-stokes-flow.md) therefore give the same disturbance. The pure strain produces no resultant force or couple, by its symmetric degree-two angular structure.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
