# Covector transformation under a change of basis

↑ **Parent:** [Covector](covector.md)

Let the columns of an [invertible matrix](invertible-matrix.md) $B$ be a new [basis](basis.md) expressed in the old [basis](basis.md). The same [vector](vector.md) has old [coordinate vector](coordinate-vector.md) $x$ and new [coordinate vector](coordinate-vector.md) $x'=B^{-1}x$. If a [covector](covector.md) has old row $\ell$, its new row is $\ell'=\ell B$, since

$$
\ell'x'=\ell B B^{-1}x=\ell x.
$$

Thus the scalar [dual pairing](dual-pairing.md) stays unchanged. If [covector](covector.md) coefficients are stored as a column $c=\ell^T$, their new column is $c'=B^Tc$; this is the inverse transpose of the transformation $x\mapsto B^{-1}x$ on [vector](vector.md) coordinates. These conventions express the [covariance and contravariance of vectors](covariance-and-contravariance-of-vectors.md). [Sergei Treil, Linear Algebra Done Wrong, §8.1.1: coordinate changes in the dual space](https://www.math.brown.edu/streil/papers/LADW/HTML_2026_04-30/Ch8.html).

For the [basis](basis.md) $b_1=(1,0)$, $b_2=(1,1)$,

$$
B=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad
x=\begin{pmatrix}3\\1\end{pmatrix},\qquad
x'=\begin{pmatrix}2\\1\end{pmatrix}.
$$

The [linear functional](linear-functional.md) $\varphi(x,y)=2x-y$ has rows $\ell=\begin{pmatrix}2&-1\end{pmatrix}$ and $\ell'=\begin{pmatrix}2&1\end{pmatrix}$. Both calculations give five: $2\cdot3-1\cdot1=2\cdot2+1\cdot1$. Changing the [basis](basis.md) changes the descriptions, not the measured value.

## ↑ Ancestors (7)

1. [Covector](covector.md)
2. [Dual space](dual-space-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Dual space](dual-space-split.md)
