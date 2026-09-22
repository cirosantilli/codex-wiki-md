<h1 id="1e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For

$$
X=\begin{pmatrix}a&b\\c&d\end{pmatrix},
$$

direct multiplication gives

$$
\phi_A(X)=AX-XA
=\begin{pmatrix}c&d-a\\0&-c\end{pmatrix}.
$$

With respect to the ordered standard basis $(E_{11},E_{12},E_{21},E_{22})$, its matrix is therefore

$$
\boxed{
[\phi_A]=
\begin{pmatrix}
0&0&1&0\\
-1&0&0&1\\
0&0&0&0\\
0&0&-1&0
\end{pmatrix}
}.
$$

This [nilpotent operator](../../../../../../nilpotent-linear-map.md) satisfies $\phi_A^3=0$, while $\phi_A^2\ne0$. Moreover,

$$
\operatorname{rank}\phi_A=2,
\qquad
\operatorname{rank}\phi_A^2=1.
$$

These ranks determine one nilpotent block of size three and one of size one. Hence its [Jordan normal form](../../../../../../jordan-normal-form.md) is

$$
\boxed{J_3(0)\oplus J_1(0)}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1E](../../1e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
