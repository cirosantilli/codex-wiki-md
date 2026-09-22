<h1 id="37d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [Minkowski spacetime](../../../../../../minkowski-spacetime.md) signature $(-,+,+,+)$ and write $dot x^\mu=dx^\mu/d\lambda$. The reparametrization-invariant [relativistic charged-particle action](../../../../../../relativistic-charged-particle-action.md) is

$$
\boxed{
S[x]=-mc\int_{\lambda_i}^{\lambda_f}
\sqrt{-\eta_{\mu\nu}\dot x^\mu\dot x^\nu}\,d\lambda
+q\int_{\lambda_i}^{\lambda_f}A_\mu(x)\dot x^\mu\,d\lambda.
}
$$

The first term is $-mc^2\int d\tau$ because

$$
\frac{d\tau}{d\lambda}
=\frac1c\sqrt{-\dot x^2}.
$$

An electromagnetic [gauge transformation](../../../../../../gauge-transformation.md) is

$$
A_\mu\longmapsto A_\mu+\partial_\mu\chi.
$$

It leaves the [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md) unchanged because antisymmetrized second derivatives commute. The action changes only by

$$
\Delta S
=q\int_{\lambda_i}^{\lambda_f}
\partial_\mu\chi\,\dot x^\mu d\lambda
=q\int_{\lambda_i}^{\lambda_f}\frac{d\chi(x(\lambda))}{d\lambda}d\lambda
=\boxed{q\bigl(\chi(x_f)-\chi(x_i)\bigr)}.
$$

This endpoint term has zero variation for fixed endpoints, which is the [gauge invariance of the charged-particle worldline action](../../../../../../gauge-invariance-of-the-charged-particle-worldline-action.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [37D](../../37d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
