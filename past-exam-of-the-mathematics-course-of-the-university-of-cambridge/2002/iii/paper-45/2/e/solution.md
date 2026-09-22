<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the [Zeldovich approximation](../../../../../../zeldovich-approximation.md), form the [Jacobian matrix](../../../../../../jacobian-matrix.md) of the Lagrangian map:

$$
\frac{\partial x_i}{\partial q_j}=\delta_{ij}-b\,\partial_i\partial_j\psi_{\rm in}.
$$

Let $\lambda_1\geq\lambda_2\geq\lambda_3$ be the eigenvalues of this potential [Hessian matrix](../../../../../../hessian-matrix.md), with the convention that positive $\lambda$ means compression. Before [shell crossing](../../../../../../shell-crossing.md), conservation of the mass in a Lagrangian volume gives

$$
\boxed{1+\delta=\frac1{\det(\partial\mathbf x/\partial\mathbf q)}
=\frac1{(1-b\lambda_1)(1-b\lambda_2)(1-b\lambda_3)}.}
$$

If $\lambda_1>0$ and is distinct from the other eigenvalues, the first singularity occurs at $b=1/\lambda_1$. One principal length collapses while the other two remain nonzero. The resulting [cosmological caustic](../../../../../../cosmological-caustic.md) is locally a sheet, conventionally a pancake, rather than a simultaneous spherical point collapse. Degenerate equal eigenvalues can instead give line- or pointlike special cases.

The predicted density divergence signals failure of the single-stream description. If the straight Lagrangian displacements are simply continued, particles cross the sheet and keep moving along their original displacement directions. They are not slowed and trapped by the evolved self-gravitating multistream structure. The streams therefore separate again, producing excessively broad pancakes at late times. In an [N-body simulation](../../../../../../n-body-simulation.md), the changing gravitational field pulls crossing streams back, produces repeated crossings and binds matter into more compact structures. This is the limitation described by [Zeldovich pancake thickness after shell crossing](../../../../../../zeldovich-pancake-thickness-after-shell-crossing.md). The initial-displacement extrapolation is useful through the onset of collapse, but does not supply the self-consistent post-crossing gravitational dynamics or virialization. After crossing, the physical density would require summing inverse absolute Jacobians over all streams, not using one negative determinant as a density.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
