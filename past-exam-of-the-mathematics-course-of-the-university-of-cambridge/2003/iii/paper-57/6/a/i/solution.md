<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Identify $\mathbb R^3$ with the traceless [Hermitian matrices](../../../../../../../hermitian-operator.md) $X=x\cdot\sigma$, where $\sigma_i$ are the [Pauli matrices](../../../../../../../pauli-matrices.md). Then $\det X=-|x|^2$. For $U\in SU(2)$ the action $X\mapsto UXU^\dagger$ preserves trace, Hermiticity and determinant, so gives an orthogonal transformation of $\mathbb R^3$. Since $SU(2)$ is connected, the determinant of this transformation is $+1$.

An element in the kernel commutes with every $\sigma_i$, hence is scalar. Unitarity and determinant one restrict it to $\pm I$. Every three-dimensional rotation is a rotation through some angle $\theta$ around a unit axis $n$. It is obtained by

$$
U=\exp(-i\theta\,n\cdot\sigma/2)=\cos(\theta/2)I-i\sin(\theta/2)n\cdot\sigma.
$$

Indeed multiplication with $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$ gives the [Rodrigues rotation formula](../../../../../../../rodrigues-rotation-formula.md) for $UXU^\dagger$. This proves surjectivity, not just equality of Lie-algebra dimensions. Therefore

$$
\boxed{SU(2)/\{\pm I\}\cong SO(3).}
$$

A full $2\pi$ rotation lifts from $I$ to $-I$, explaining the double cover and the [Spin group](../../../../../../../spin-group.md) interpretation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
