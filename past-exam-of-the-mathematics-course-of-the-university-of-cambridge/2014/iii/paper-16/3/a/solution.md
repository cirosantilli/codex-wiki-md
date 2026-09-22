<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Moser's trick](../../../../../../moser-s-trick.md) turns variation of [symplectic forms](../../../../../../symplectic-form.md) into an equation for a time-dependent [vector field](../../../../../../vector-field.md). Let $\omega_t$, $0\leq t\leq1$, be a smooth path of [symplectic forms](../../../../../../symplectic-form.md) on a compact manifold without boundary, with a constant [de Rham cohomology](../../../../../../de-rham-cohomology.md) class. Choose a smooth family of one-forms $\alpha_t$ such that $\dot\omega_t=d\alpha_t$. Such a smooth choice can be made using a fixed auxiliary metric; the essential requirement is this exactness throughout the path.

Nondegeneracy uniquely determines $X_t$ by

$$
\iota_{X_t}\omega_t=-\alpha_t.
$$

Let $f_t$ be its flow, with $f_0=\mathrm{id}$. Compactness ensures existence over the whole parameter interval. By [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md),

$$
\frac d{dt}f_t^*\omega_t
=f_t^*(\dot\omega_t+\mathcal L_{X_t}\omega_t)
=f_t^*(d\alpha_t+d\iota_{X_t}\omega_t)=0.
$$

Thus

$$
\boxed{f_t^*\omega_t=\omega_0.}
$$

The path is made constant by a [diffeomorphism](../../../../../../diffeomorphism.md) moving with $X_t$. Every interpolating form must be nondegenerate; equal endpoint cohomology alone does not ensure that every linearly interpolated form is a [symplectic form](../../../../../../symplectic-form.md). On a noncompact manifold one instead needs completeness of this flow, or restricts to a sufficiently small neighborhood, as in the local argument below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
