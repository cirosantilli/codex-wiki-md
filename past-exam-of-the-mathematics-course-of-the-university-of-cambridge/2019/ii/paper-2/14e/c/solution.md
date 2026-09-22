<h1 id="14e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the [gauge transformation](../../../../../../gauge-transformation.md),

$$
\widetilde{\mathbf B}=\nabla\times(\mathbf A+\nabla f)=\mathbf B
$$

because the [curl](../../../../../../curl.md) of a [gradient](../../../../../../gradient.md) vanishes, and

$$
\widetilde{\mathbf E}
=-\nabla(\phi-\partial_tf)-\partial_t(\mathbf A+\nabla f)
=\mathbf E.
$$

The transformed [Lagrangian](../../../../../../lagrangian.md) is

$$
\widetilde L=L+q(\partial_tf+\dot{\mathbf r}\cdot\nabla f)
=L+\frac d{dt}(qf).
$$

A total time derivative changes the action only by endpoint terms, whose variation vanishes for fixed endpoints, so the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) are unchanged.

The new momentum is

$$
\widetilde{\mathbf p}=m\dot{\mathbf r}+q\widetilde{\mathbf A}
=\mathbf p+q\nabla f.
$$

Use the [type-two generating function for a canonical transformation](../../../../../../type-two-generating-function-for-a-canonical-transformation.md)

$$
F_2(\mathbf r,\widetilde{\mathbf p},t)
=\mathbf r\cdot\widetilde{\mathbf p}-qf(\mathbf r,t).
$$

It gives $\mathbf p=\partial F_2/\partial\mathbf r=\widetilde{\mathbf p}-q\nabla f$, $\widetilde{\mathbf r}=\partial F_2/\partial\widetilde{\mathbf p}=\mathbf r$, and

$$
\widetilde H=H+\partial_tF_2=H-q\partial_tf.
$$

This equals $|\widetilde{\mathbf p}-q\widetilde{\mathbf A}|^2/(2m)+q\widetilde\phi$, so the gauge change is a time-dependent [canonical transformation](../../../../../../canonical-transformation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14E](../../14e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
