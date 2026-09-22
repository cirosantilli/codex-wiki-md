<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A matrix is [non-normal](../../../../../../non-normal-matrix.md) when it does not commute with its [adjoint matrix](../../../../../../conjugate-transpose.md):

$$
LL^\dagger\ne L^\dagger L.
$$

Nonorthogonal decaying eigenmodes can interfere constructively and produce [transient growth](../../../../../../transient-growth.md). For example,

$$
L=\begin{pmatrix}-1&10\\0&-2\end{pmatrix}
$$

has two negative [eigenvalues](../../../../../../eigenvalue.md) but is non-normal. Starting from $x(0)=(0,1)^T$ gives

$$
x(t)=\begin{pmatrix}10(e^{-t}-e^{-2t})\\e^{-2t}\end{pmatrix}.
$$

At $t=\log2$, its squared [Euclidean norm](../../../../../../euclidean-norm.md) is $2.5^2+0.25^2>1=|x(0)|^2$. The energy grows transiently even though both eigenmodes eventually decay.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
