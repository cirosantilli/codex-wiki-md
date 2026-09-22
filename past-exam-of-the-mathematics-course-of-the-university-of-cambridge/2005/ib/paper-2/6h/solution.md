<h1 id="6h/solution">Solution</h1>

↑ **Parent:** [6H](../6h.md)

In SI units, the sourced [Maxwell equations](../../../../../maxwell-equations.md) are

$$
\nabla\cdot\mathbf E=\rho/\epsilon_0,\qquad\nabla\cdot\mathbf B=0,
\qquad\nabla\times\mathbf E=-\partial_t\mathbf B,
\qquad\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E.
$$

Take the [divergence](../../../../../divergence.md) of the last equation. The [divergence](../../../../../divergence.md) of a [curl](../../../../../curl.md) vanishes; using the first equation gives the necessary local conservation law

$$
\boxed{\partial_t\rho+\nabla\cdot\mathbf J=0.}
$$

For sources supported in a fixed region, integrate over a containing surface where the current vanishes. The [divergence](../../../../../divergence.md) theorem gives

$$
\frac{d}{dt}\int_V\rho\,d^3x=-\int_{\partial V}\mathbf J\cdot\mathbf n\,dS=0.
$$

Thus the total charge is constant. For each component of the [electric dipole moment](../../../../../electric-dipole-moment.md), integration by parts gives

$$
\frac{d}{dt}\int_Vx_i\rho\,d^3x
=-\int_Vx_i\partial_jJ_j\,d^3x
=-\int_{\partial V}x_i\mathbf J\cdot\mathbf n\,dS+\int_VJ_i\,d^3x.
$$

The surface term again vanishes, so

$$
\boxed{\frac{d}{dt}\int_V\mathbf x\rho\,d^3x=\int_V\mathbf J\,d^3x.}
$$

Smooth [compact](../../../../../compact-space.md) support suffices for these manipulations; equivalently one may integrate the [charge continuity equation](../../../../../charge-continuity-equation.md) over all space and use the fixed support to identify the [integrals](../../../../../integral.md) with those over $V$.

## ↑ Ancestors (10)

1. [6H](../6h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
