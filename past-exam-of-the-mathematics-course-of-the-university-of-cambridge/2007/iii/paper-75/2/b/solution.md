<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) implies

$$
\nabla_\perp\cdot\delta\mathbf B_\perp=-\partial_z\delta B_\parallel.
$$

With $\delta B/B_0=O(\epsilon)$ and $\partial_z=O(\epsilon\nabla_\perp)$, the right-hand side is $O(\epsilon^2k_\perp B_0)$. Thus the leading, order-$\epsilon$ perpendicular field is [divergence-free](../../../../../../solenoidal-vector-field.md). On a simply connected perpendicular patch, or for the nonzero perpendicular [Fourier modes](../../../../../../fourier-mode.md) of a periodic domain, it has a [stream function](../../../../../../stream-function.md). Choose its normalization by

$$
\delta B_x=-\frac{B_0}{v_A}\partial_y\Psi,\qquad\delta B_y=\frac{B_0}{v_A}\partial_x\Psi.
$$

Consequently the leading [reduced electron magnetohydrodynamics](../../../../../../reduced-electron-magnetohydrodynamics.md) representation is

$$
\boxed{\frac{\delta\mathbf B}{B_0}=\frac1{v_A}\hat{\mathbf z}\times\nabla_\perp\Psi+\hat{\mathbf z}\frac{\delta B_\parallel}{B_0}+O(\epsilon^2).}
$$

The error denotes an order-$\epsilon^2$ field relative to $B_0$. The parallel perturbation is an independent scalar and is not removed by leading perpendicular solenoidality.

For clarity, the representation is asymptotic rather than an exact decomposition of an arbitrary three-dimensional [solenoidal](../../../../../../solenoidal-vector-field.md) field. If $\delta B_\parallel$ depends on $z$, exact solenoidality can be restored by adding $\nabla_\perp\chi$ to $\delta\mathbf B_\perp$, where $\nabla_\perp^2\chi=-\partial_z\delta B_\parallel$. Its amplitude is $O(\epsilon^2B_0)$, so it lies beyond the retained field order. A perpendicular harmonic component can be absorbed into the guide field or fixed separately by [boundary conditions](../../../../../../boundary-condition.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
