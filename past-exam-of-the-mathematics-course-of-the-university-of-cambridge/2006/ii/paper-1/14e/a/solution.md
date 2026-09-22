<h1 id="14e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Linearizing about the orbit gives $\dot\eta=A(t)\eta$, where $A(t)=Df(X(t))$. The [fundamental matrix](../../../../../../fundamental-matrix-of-a-linear-differential-equation.md) therefore satisfies

$$
\boxed{\dot\Phi(t)=A(t)\Phi(t),\qquad\Phi(0)=I.}
$$

The [Floquet multipliers](../../../../../../floquet-multiplier.md) are the [eigenvalues](../../../../../../eigenvalue.md) of the [monodromy matrix](../../../../../../monodromy-matrix.md) $\Phi(T)$. Differentiating the orbit equation shows that its tangent $\dot X(t)$ solves the [variational equation](../../../../../../variational-equation.md). Since $\dot X(T)=\dot X(0)\ne0$, one multiplier is one.

For an invertible [fundamental matrix](../../../../../../fundamental-matrix-of-a-linear-differential-equation.md), differentiating the [determinant](../../../../../../determinant.md) gives $(\det\Phi)'=\operatorname{tr}(\Phi^{-1}\dot\Phi)\det\Phi=\operatorname{tr}A\det\Phi$. [Integration](../../../../../../integral.md) from the identity yields $\det\Phi(T)=\exp(\int_0^T\operatorname{tr}A(t)dt)$. The [determinant](../../../../../../determinant.md) is the product of the two multipliers, so the other is

$$
\boxed{\mu=\exp\left(\int_0^T\nabla\cdot f(X(t))\,dt\right).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
