<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

Let $A=Dy(x)$ be the [Jacobian matrix](../../../../../jacobian-matrix.md) and $K(y)=H(x(y))$. The [chain rule](../../../../../chain-rule.md) gives $\nabla_xH=A^T\nabla_yK$. Therefore the [Hamilton equations](../../../../../hamilton-s-equations.md) transform to $\dot y=AJ A^T\nabla_yK$, with $J=\begin{pmatrix}0&-I\\I&0\end{pmatrix}$. They have the required canonical form for every [Hamiltonian](../../../../../hamiltonian.md) exactly when

$$
\boxed{AJA^T=J.}
$$

Necessity follows by choosing Hamiltonians whose gradients take arbitrary values at a point; sufficiency follows from the displayed transformed equation. This is the [symplectic matrix](../../../../../symplectic-matrix.md) condition for a [canonical transformation](../../../../../canonical-transformation.md), and it also forces $A$ to be invertible.

For the given transformation, $A=\begin{pmatrix}1&2\\-1/4&1/2\end{pmatrix}$ has [determinant](../../../../../determinant.md) one. For any $2\times2$ matrix, $AJA^T=(\det A)J$, so the proposed transformation **is canonical**.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
