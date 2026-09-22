<h1 id="6b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since $N_i=N_i^*e^{x_i}$, division of each population equation by $N_i$ gives

$$
\dot x_1=\epsilon_1(e^{x_2}-1),
\qquad
\dot x_2=-\epsilon_2(e^{x_1}-1).
$$

Define the [Hamiltonian function](../../../../../../hamiltonian-function.md)

$$
H(x_1,x_2)
=\epsilon_2(e^{x_1}-x_1-1)
+\epsilon_1(e^{x_2}-x_2-1)
$$

and the [antisymmetric matrix](../../../../../../skew-symmetric-matrix.md)

$$
K=\begin{pmatrix}0&1\\-1&0\end{pmatrix}.
$$

Then

$$
\nabla H
=\begin{pmatrix}\epsilon_2(e^{x_1}-1)\\
\epsilon_1(e^{x_2}-1)\end{pmatrix},
\qquad
\boxed{\dot{\mathbf x}=K\nabla H}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6B](../../6b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
