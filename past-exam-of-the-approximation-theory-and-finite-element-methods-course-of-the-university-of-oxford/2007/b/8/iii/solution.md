<h1 id="b/8/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Define the [mass matrix](../../../../../mass-matrix.md) $M_{ij}=\int_0^1\phi_j\phi_i$ and [stiffness matrix](../../../../../stiffness-matrix.md) $K_{ij}=\int_0^1\phi_j'\phi_i'$ for $1\leq i,j\leq N$. With coefficient vectors $U^m$, the step system is

$$
\boxed{\mathsf A U^{m+1}=M U^m,\qquad\mathsf A=M+\Delta t(K+M).}
$$

The matrices are symmetric, and $V^T\mathsf AV=\|v_h\|_2^2+\Delta t(\|v_h'\|_2^2+\|v_h\|_2^2)>0$ for nonzero $V$, proving positive definiteness.

For $h=1/2$, the first [basis](../../../../../basis.md) function is the full tent at $1/2$, and the last is the half tent ending at $1$. Integration gives

$$
M=\begin{pmatrix}1/3&1/12\\1/12&1/6\end{pmatrix},\qquad
K=\begin{pmatrix}4&-2\\-2&2\end{pmatrix}.
$$

Since $\Delta t=2/2=1$, the requested [matrix](../../../../../matrix.md) in this normalization is

$$
\boxed{\mathsf A=2M+K=\begin{pmatrix}14/3&-11/6\\-11/6&7/3\end{pmatrix}.}
$$

Here the [matrix](../../../../../matrix.md) symbol $M$ is distinct from the printed integer number of time steps.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
