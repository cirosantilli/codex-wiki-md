<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

View $X$ as the matrix of a [linear map](../../../../../linear-map.md) $T:F^m\to F^n$ of [matrix rank](../../../../../matrix-rank.md) $r$. Choose vectors $u_1,\ldots,u_r$ whose images form a [basis](../../../../../basis.md) of $\operatorname{im}T$, extend them by a basis of $\ker T$ to a basis of $F^m$, and extend $Tu_1,\ldots,Tu_r$ to a basis of $F^n$. In these two bases the matrix of $T$ is the [rank normal form](../../../../../rank-normal-form.md)

$$
\begin{pmatrix}I_r&0\\0&0\end{pmatrix}.
$$

The two changes of basis give invertible $P,Q$ with the displayed matrix equal to $Q^{-1}XP$.

For the [block upper triangular matrix](../../../../../block-upper-triangular-matrix.md) $A=\begin{pmatrix}B&D\\0&C\end{pmatrix}$, every nonzero term in the [Leibniz formula for determinants](../../../../../leibniz-formula-for-determinants.md) sends the rows belonging to $C$ into the columns belonging to $C$; bijectivity then sends the remaining rows into the $B$ columns. The permutation sum consequently factors into the determinant sums for $B$ and $C$, proving

$$
\boxed{\det A=\det B\det C.}
$$

Finally suppose $L(X)=0$, so $AX=XB$: the map $X:\mathbb C^m\to\mathbb C^n$ is an [intertwining operator](../../../../../intertwining-operator.md). If $v$ lies in the [generalized eigenspace](../../../../../generalized-eigenspace.md) of $B$ for $\lambda$, then for some $k$,

$$
(A-\lambda I)^kXv=X(B-\lambda I)^kv=0.
$$

Because $A$ and $B$ have no common [eigenvalue](../../../../../eigenvalue.md), $A-\lambda I$ is invertible, hence $Xv=0$. The generalized eigenspaces of $B$ span $\mathbb C^m$, so $X=0$. Thus **the [Sylvester equation](../../../../../sylvester-equation.md) operator $L$ is injective.**

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
