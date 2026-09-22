<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

For a full-column-rank [matrix](../../../../../matrix.md), a thin [QR decomposition](../../../../../qr-decomposition.md) has $A=Q_1R$, where $Q_1^TQ_1=I_n$ and $R$ is nonsingular upper triangular. Extend $Q_1$ to an orthogonal [matrix](../../../../../matrix.md) $Q=(Q_1,Q_2)$. Orthogonality gives

$$
\|Ax-b\|^2=\|Rx-Q_1^Tb\|^2+\|Q_2^Tb\|^2.
$$

Thus the unique least-squares solution satisfies $Rx^*=Q_1^Tb$, with residual norm $\|Q_2^Tb\|$. In a rank-deficient problem $R$ is singular and uniqueness needs separate treatment.

A [Givens rotation](../../../../../givens-rotation.md) is the identity except for the rows/columns $p,q$, whose block is $\left(\begin{smallmatrix}c&s\\-s&c\end{smallmatrix}\right)$ with $c^2+s^2=1$. Its transpose times itself has that block equal to the identity, so it is orthogonal. Choose $c=4/5,s=3/5$ in rows two and three. Then

$$
GA=\begin{pmatrix}2&1&1\\0&5&2\\0&0&1\\0&0&0\end{pmatrix},\qquad
Gb=\begin{pmatrix}2\\3\\-1\\2\end{pmatrix}.
$$

Back substitution in the first three rows gives

$$
\boxed{x^*=(1,1,-1)^T,\qquad \|Ax^*-b\|=2.}
$$

The fourth row of the rotated residual is the unavoidable value $-2$, while the other three rows vanish. Thus this rotation also directly exhibits the least-squares optimality.

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
