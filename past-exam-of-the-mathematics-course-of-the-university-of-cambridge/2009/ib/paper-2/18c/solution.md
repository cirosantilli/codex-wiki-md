<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

Choose the [Givens rotation](../../../../../givens-rotation.md) convention in which $\Omega^{[p,q]}$ equals the identity outside rows and columns $p,q$, and has block

$$
\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}
$$

in those coordinates. It is an [orthogonal matrix](../../../../../orthogonal-matrix.md). For any chosen column $j$, write $u=A_{pj}$, $v=A_{qj}$ and $r=\sqrt{u^2+v^2}$. If $r>0$, take $\cos\theta=u/r$, $\sin\theta=v/r$. Then the new entries are $r$ and $-vu/r+uv/r=0$. If both entries vanish, take $\theta=0$. This proves the requested elimination for each chosen $j$; the angle is allowed to depend on $j$, and one angle need not eliminate an entire arbitrary row.

For the given [matrix](../../../../../matrix.md), use $\cos\theta=\sin\theta=1/\sqrt2$ first for $\Omega^{[1,2]}$, obtaining

$$
\Omega^{[1,2]}A=\begin{pmatrix}\sqrt2&7/\sqrt2&3\sqrt2\\0&1/\sqrt2&\sqrt2\\\sqrt2&7/\sqrt2&4\sqrt2\end{pmatrix}.
$$

Use the same cosine and sine for $\Omega^{[1,3]}$. It makes

$$
R=\Omega^{[1,3]}\Omega^{[1,2]}A=\begin{pmatrix}2&7&7\\0&1/\sqrt2&\sqrt2\\0&0&1\end{pmatrix}.
$$

This is already upper triangular, including the zero $(3,2)$ entry, and every leading nonzero row entry is positive. Thus the requested [QR decomposition](../../../../../qr-decomposition.md) is

$$
\boxed{Q=(\Omega^{[1,3]}\Omega^{[1,2]})^T=\begin{pmatrix}1/2&-1/\sqrt2&-1/2\\1/2&1/\sqrt2&-1/2\\1/\sqrt2&0&1/\sqrt2\end{pmatrix},\qquad
R=\begin{pmatrix}2&7&7\\0&1/\sqrt2&\sqrt2\\0&0&1\end{pmatrix}.}
$$

The [orthogonal matrix](../../../../../orthogonal-matrix.md) property follows from the two rotations, and direct multiplication verifies $A=QR$.

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
