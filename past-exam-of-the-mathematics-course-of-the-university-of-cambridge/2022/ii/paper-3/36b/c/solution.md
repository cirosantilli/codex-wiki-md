<h1 id="36b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [electric dipole moment](../../../../../../electric-dipole-moment.md) of a localized charge density is

$$
\mathbf p(t)=\int_{\mathbb R^3}\mathbf x\,\rho(\mathbf x,t)\,d^3x.
$$

Differentiate and use the [continuity equation](../../../../../../continuity-equation.md) $\dot\rho+\nabla\cdot\mathbf J=0$:

$$
\dot p_i
=-\int x_i\partial_jJ_j\,d^3x
=\int J_i\,d^3x
-\int_{\partial\mathbb R^3}x_iJ_jn_j\,dS.
$$

Localization makes the boundary integral vanish. Component by component,

$$
\boxed{\dot{\mathbf p}(t)=\int_{\mathbb R^3}\mathbf J(\mathbf x,t)\,d^3x}.
$$

This is the [time derivative of the electric dipole moment](../../../../../../time-derivative-of-the-electric-dipole-moment.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [36B](../../36b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
