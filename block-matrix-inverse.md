# Block matrix inverse

↑ **Parent:** [Matrix inverse](matrix-inverse-split.md)

A [block matrix inverse](block-matrix-inverse.md) expresses the [matrix inverse](matrix-inverse-split.md) in terms of smaller [matrices](matrix.md). Partition a [square matrix](square-matrix.md) over a [field](field.md) as

$$
M=\begin{pmatrix}A&B\\C&D\end{pmatrix},\qquad
A\in\mathbb F^{p\times p},\quad D\in\mathbb F^{q\times q}.
$$

If $A$ is an [invertible matrix](invertible-matrix.md), define its [Schur complement](schur-complement.md) $S=D-CA^{-1}B$. Then $M$ is an [invertible matrix](invertible-matrix.md) exactly when $S$ is an [invertible matrix](invertible-matrix.md), and

$$
\boxed{
M^{-1}=\begin{pmatrix}
A^{-1}+A^{-1}BS^{-1}CA^{-1}&-A^{-1}BS^{-1}\\
-S^{-1}CA^{-1}&S^{-1}
\end{pmatrix}.
}
$$

The order of the [matrix products](matrix-product.md) matters. In particular, the lower-right block is $S^{-1}$, rather than generally $D^{-1}$: the coupling through $B$ and $C$ changes the response.[Appendix A.5.5, printed p. 650: inverse of a symmetric block matrix; §C.4.1, printed p. 673: elimination for general blocks](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

For an original example, take

$$
M=\begin{pmatrix}2&0&1\\0&3&2\\1&2&5\end{pmatrix},\quad
A=\begin{pmatrix}2&0\\0&3\end{pmatrix},\quad
B=C^T=\begin{pmatrix}1\\2\end{pmatrix},\quad D=5.
$$

The [Schur complement](schur-complement.md) is $S=5-1/2-4/3=19/6$. Substitution gives the concise answer

$$
\boxed{M^{-1}=\frac1{19}\begin{pmatrix}11&2&-3\\2&9&-4\\-3&-4&6\end{pmatrix}}.
$$

Multiplying in either order gives the [identity matrix](identity-matrix.md); the lower-right entry is $6/19$, whereas $D^{-1}=1/5$. The difference records the feedback through the two eliminated variables.

<a id="image-a-block-matrix-inverse-computed-from-the-smaller-schur-complement"></a>
![](block-matrix-schur-inverse-example.png)

**[Figure 2](#image-a-block-matrix-inverse-computed-from-the-smaller-schur-complement). A block matrix inverse computed from the smaller Schur complement**. Original exact example. Colours mark the two-by-two block $A$, the coupling blocks $B,C$, and the scalar block $D$. The same partition is retained in the [matrix inverse](matrix-inverse-split.md); its blocks are not the entrywise inverses of the original blocks.

Often the desired output is a solution of a [linear system](system-of-linear-equations.md), rather than every entry of a [matrix inverse](matrix-inverse-split.md). [Block elimination](block-elimination.md) solves with $A$ and then with $S$, recovering the eliminated variables by [back substitution](back-substitution.md). Reusing an [LU decomposition](lu-decomposition.md) of $A$ avoids explicitly forming $A^{-1}$. A favourable [block diagonal matrix](block-diagonal-matrix.md) or [tridiagonal matrix](tridiagonal-matrix.md) block can make this useful; merely partitioning an unstructured dense [matrix](matrix.md) does not guarantee a faster solve.[§C.4.1, printed pp. 672–675: Algorithm C.4, factor-solve interpretation and dense complexity comparison](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

**Table of contents**

- [Block elimination](block-elimination.md)
- [Choosing a different block pivot](choosing-a-different-block-pivot.md)

## ↑ Ancestors (6)

1. [Matrix inverse](matrix-inverse-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Block elimination](block-elimination.md)
- [Block matrix inverse](block-matrix-inverse.md)
- [Choosing a different block pivot](choosing-a-different-block-pivot.md)
- [Leave-one-out residual identity for a linear smoother](leave-one-out-residual-identity-for-a-linear-smoother.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205/5/b/solution.md)
- [Schur complement](schur-complement.md)
- [Schur complement determinant identity](schur-complement-determinant-identity.md)
