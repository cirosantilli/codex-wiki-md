<h1 id="6c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $P=P'=0$, it suffices to map the two edge [vectors](../../../../../../vector.md). Let the columns of the required [matrix](../../../../../../matrix.md) be $u_1,u_2,u_3$. The condition $MQ=Q'$ gives

$$
u_2=\left(-\frac12,0,\frac{\sqrt3}{2}\right)^T.
$$

The condition $MR=R'$ then gives

$$
\frac{\sqrt3}{2}u_1+\frac12u_2=R',
$$

and hence

$$
u_1=\left(\frac{\sqrt3}{2},0,\frac12\right)^T.
$$

These are orthonormal. Taking $u_3=u_1\times u_2=(0,-1,0)^T$ produces the orthogonal [matrix](../../../../../../matrix.md)

$$
\boxed{
M=
\begin{pmatrix}
\sqrt3/2&-1/2&0\\
0&0&-1\\
1/2&\sqrt3/2&0
\end{pmatrix}}.
$$

Its columns are orthonormal, and direct substitution verifies $MP=P'$, $MQ=Q'$, and $MR=R'$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6C](../../6c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
