# Block elimination

↑ **Parent:** [Block matrix inverse](block-matrix-inverse.md)

Write a [linear system](system-of-linear-equations.md) as $Ax+By=f$ and $Cx+Dy=g$, with $A$ an [invertible matrix](invertible-matrix.md). Solving the first equation for $x$ and substituting in the second gives

$$
x=A^{-1}(f-By),\qquad
(D-CA^{-1}B)y=g-CA^{-1}f.
$$

Thus the [Schur complement](schur-complement.md) is the coefficient [matrix](matrix.md) remaining after the $x$ variables have been eliminated. When it is an [invertible matrix](invertible-matrix.md), solve the reduced [linear system](system-of-linear-equations.md) for $y$ and recover $x$. In computation, expressions such as $A^{-1}B$ mean solving with each column of $B$, using the same [LU decomposition](lu-decomposition.md) or [Cholesky decomposition](cholesky-decomposition.md) when applicable.

For the example under [block matrix inverse](block-matrix-inverse.md) and right-hand side $(3,1,4)^T$, take $f=(3,1)^T$ and $g=4$. Since $CA^{-1}f=13/6$, the reduced equation is $(19/6)y=11/6$. [Back substitution](back-substitution.md) gives

$$
\boxed{(x_1,x_2,y)=(23,-1,11)/19}.
$$

The original equations return $3$, $1$ and $4$, respectively. The reduction retained the influence of $x_1,x_2$ on $y$ through the correction $CA^{-1}B$.

A short proof outline also explains whether $M$ is an [invertible matrix](invertible-matrix.md): the exact [matrix factorization](matrix-decomposition.md)

$$
M=\begin{pmatrix}I&0\\CA^{-1}&I\end{pmatrix}
\begin{pmatrix}A&0\\0&S\end{pmatrix}
\begin{pmatrix}I&A^{-1}B\\0&I\end{pmatrix}
$$

has [invertible matrices](invertible-matrix.md) on the outside. Therefore $M$ is an [invertible matrix](invertible-matrix.md) precisely when the central [block diagonal matrix](block-diagonal-matrix.md) is one. Reversing the factors gives the [block matrix inverse](block-matrix-inverse.md), while taking [determinants](determinant.md) gives the [Schur complement determinant identity](schur-complement-determinant-identity.md).

## ↑ Ancestors (7)

1. [Block matrix inverse](block-matrix-inverse.md)
2. [Matrix inverse](matrix-inverse-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Block matrix inverse](block-matrix-inverse.md)
- [Matrix decomposition](matrix-decomposition.md)
- [Schur complement](schur-complement.md)
- [Schur complement determinant identity](schur-complement-determinant-identity.md)
