<h1 id="36a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $\varepsilon_{ij}$ and $\mu_{ij}$ are symmetric and time-independent, the [linear anisotropic dielectric](../../../../../../linear-anisotropic-dielectric.md) relations give

$$
E_i\partial_tD_i
=\varepsilon_{ij}E_i\partial_tE_j
=\frac12\partial_t(\varepsilon_{ij}E_iE_j),
$$

and similarly

$$
H_i\partial_tB_i
=\frac12\partial_t(\mu_{ij}H_iH_j).
$$

Integrate the identity from part (b) over $V$ and apply the [divergence theorem](../../../../../../divergence-theorem.md) to obtain

$$
\boxed{
\frac{\partial}{\partial t}\int_V
\frac12(\varepsilon_{ij}E_iE_j+\mu_{ij}H_iH_j)\,dV
+\int_S(\mathbf E\times\mathbf H)\cdot d\mathbf S
=-\int_V\mathbf E\cdot\mathbf J\,dV}.
$$

When $\mathbf J=0$, this is conservation of electromagnetic energy. The [Poynting theorem in a linear anisotropic medium](../../../../../../poynting-theorem-in-a-linear-anisotropic-medium.md) identifies

$$
\boxed{u=\frac12(\varepsilon_{ij}E_iE_j+\mu_{ij}H_iH_j)}
$$

as the energy density and

$$
\boxed{\mathbf N=\mathbf E\times\mathbf H}
$$

as the energy flux, or [Poynting vector](../../../../../../poynting-vector.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [36A](../../36a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
