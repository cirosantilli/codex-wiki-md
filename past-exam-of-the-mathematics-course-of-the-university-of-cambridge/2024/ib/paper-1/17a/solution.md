<h1 id="17a/solution">Solution</h1>

↑ **Parent:** [17A](../17a.md)

A [Givens rotation](../../../../../givens-rotation.md) $\Omega^{[p,q]}$ is the identity except in rows and columns $p,q$, where it has the block

$$
\begin{pmatrix}c&s\\-s&c\end{pmatrix},
\qquad c=\cos\theta,
\quad s=\sin\theta.
$$

For $a=A_{pj}$ and $b=A_{qj}$, choose

$$
c=\frac{a}{\sqrt{a^2+b^2}},
\qquad
s=\frac{b}{\sqrt{a^2+b^2}}
$$

when $(a,b)\ne(0,0)$. Then

$$
(\Omega^{[p,q]}A)_{qj}=-sa+cb=0.
$$

If both entries vanish, any angle works.

For the given [matrix](../../../../../matrix.md), first use

$$
\Omega^{[1,3]}=
\begin{pmatrix}
1/\sqrt2&0&1/\sqrt2\\
0&1&0\\
-1/\sqrt2&0&1/\sqrt2
\end{pmatrix}.
$$

It gives

$$
\Omega^{[1,3]}A=
\begin{pmatrix}
2&1&1\\
0&\sqrt3&0\\
0&1&\sqrt3
\end{pmatrix}.
$$

Then use

$$
\Omega^{[2,3]}=
\begin{pmatrix}
1&0&0\\
0&\sqrt3/2&1/2\\
0&-1/2&\sqrt3/2
\end{pmatrix}.
$$

Thus $R=\Omega^{[2,3]}\Omega^{[1,3]}A$ is

$$
R=
\begin{pmatrix}
2&1&1\\
0&2&\sqrt3/2\\
0&0&3/2
\end{pmatrix}.
$$

All leading row entries are positive. The resulting [QR decomposition by Givens rotations](../../../../../qr-decomposition-by-givens-rotations.md) is

$$
\boxed{A=QR},
$$

where

$$
\boxed{
Q=(\Omega^{[2,3]}\Omega^{[1,3]})^T
=\begin{pmatrix}
\sqrt2/2&-\sqrt2/4&-\sqrt6/4\\
0&\sqrt3/2&-1/2\\
\sqrt2/2&\sqrt2/4&\sqrt6/4
\end{pmatrix}}
$$

and $R$ is the [matrix](../../../../../matrix.md) above. Since it is a product of transposed rotations, $Q$ is orthogonal.

## ↑ Ancestors (10)

1. [17A](../17a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
