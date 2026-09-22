<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Set $c=\cos(2\alpha_1)$ and $s=\sin(2\alpha_1)$. Multiplying the [matrices](../../../../../matrix.md), or using the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md), gives

$$
A_1^\dagger\tau_1A_1=\tau_1,\qquad
A_1^\dagger\tau_2A_1=c\tau_2+s\tau_3,\qquad
A_1^\dagger\tau_3A_1=c\tau_3-s\tau_2.
$$

Collecting the coefficients of $i\tau_j$ in $M'$ yields

$$
\boxed{\begin{pmatrix}x_1'\\x_2'\\x_3'\end{pmatrix}
=\begin{pmatrix}1&0&0\\0&c&-s\\0&s&c\end{pmatrix}
\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}.}
$$

This is the right-handed active [rotation](../../../../../rotation-mathematics.md) by $2\alpha_1$ about the positive $x_1$ axis. Likewise, with $c_j=\cos(2\alpha_j)$ and $s_j=\sin(2\alpha_j)$,

$$
\boxed{A_2:\ (x_1,x_2,x_3)\mapsto(c_2x_1+s_2x_3,\ x_2,\ -s_2x_1+c_2x_3),}
$$



$$
\boxed{A_3:\ (x_1,x_2,x_3)\mapsto(c_3x_1-s_3x_2,\ s_3x_1+c_3x_2,\ x_3).}
$$

Thus the other axes also have [rotation](../../../../../rotation-mathematics.md) angle $2\alpha_j$. The factor of two is essential: replacing $A_j$ by $-A_j$ leaves the [conjugation](../../../../../conjugation.md) unchanged, illustrating the two-to-one relation between [SU(2)](../../../../../su-2-group.md) and three-dimensional [rotations](../../../../../rotation-mathematics.md).

## ↑ Ancestors (13)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
