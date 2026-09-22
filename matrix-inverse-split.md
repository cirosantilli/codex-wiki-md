# Matrix inverse

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_inverse)

For an $n$-by-$n$ [square matrix](square-matrix.md) $A$ over a [field](field.md), its matrix inverse is an $n$-by-$n$ [matrix](matrix.md) $A^{-1}$ satisfying both identities

$$
AA^{-1}=A^{-1}A=I_n,
$$

where $I_n$ is the [identity matrix](identity-matrix.md). It exists exactly when $A$ is an [invertible matrix](invertible-matrix.md), equivalently when its [matrix rank](matrix-rank.md) is $n$ or its [determinant](determinant.md) is nonzero. It reverses the [linear map](linear-map.md): applying $A$ and then $A^{-1}$ recovers the input, while applying $A^{-1}$ and then $A$ recovers the output.[Strang, MIT 18.06 Lecture 3: the two inverse identities](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/resources/lecture-3-multiplication-and-inverse-matrices/)

The [matrix inverse](matrix-inverse-split.md) is unique. If $B$ and $C$ both satisfy the identities, then $B=B(AC)=(BA)C=C$. Although the definition is two-sided, for finite [square matrices](square-matrix.md) either identity alone suffices: $BA=I$ forces a [trivial kernel](trivial-kernel.md), whereas $AB=I$ forces [surjectivity](surjective-function.md); either makes $A$ an [invertible matrix](invertible-matrix.md) by the [rank-nullity theorem](rank-nullity-theorem.md). Rectangular [matrices](matrix.md) may have only one of these properties.

For a concrete example, take

$$
A=\begin{pmatrix}2&1\\1&1\end{pmatrix},\qquad
\det A=2\cdot1-1\cdot1=1,\qquad
A^{-1}=\begin{pmatrix}1&-1\\-1&2\end{pmatrix}.
$$

Direct [matrix multiplication](matrix-multiplication.md) gives

$$
AA^{-1}=\begin{pmatrix}2-1&-2+2\\1-1&-1+2\end{pmatrix}=I_2,
\qquad
A^{-1}A=\begin{pmatrix}2-1&1-1\\-2+2&-1+2\end{pmatrix}=I_2.
$$

Consequently the [vector](vector.md) $v=(1,2)^T$ follows a reversible journey:

$$
\begin{pmatrix}1\\2\end{pmatrix}
\xrightarrow{\ A\ }\begin{pmatrix}4\\3\end{pmatrix}
\xrightarrow{\ A^{-1}\ }\begin{pmatrix}4-3\\-4+6\end{pmatrix}
=\begin{pmatrix}1\\2\end{pmatrix}.
$$

The columns $(2,1)^T$ and $(1,1)^T$ are the images of the [standard basis](standard-basis.md) vectors. They turn the unit square into a [parallelogram](parallelogram.md); the [matrix inverse](matrix-inverse-split.md) restores both the square and its surrounding grid. Since $\det A=1$, this example changes shape while preserving [area](surface-area.md), illustrating that invertibility does not require preserving lengths or angles.

<a id="image-a-matrix-inverse-restores-a-grid-and-a-vector-a-singular-matrix-merges-distinct-inputs"></a>
![](matrix-inverse-undoing-a-map.png)

**[Figure 1](#image-a-matrix-inverse-restores-a-grid-and-a-vector-a-singular-matrix-merges-distinct-inputs). A matrix inverse restores a grid and a vector; a singular matrix merges distinct inputs**.

For comparison, the [singular matrix](singular-matrix.md)

$$
S=\begin{pmatrix}1&1\\0&0\end{pmatrix},\qquad
S\begin{pmatrix}1\\0\end{pmatrix}
=S\begin{pmatrix}0\\1\end{pmatrix}
=\begin{pmatrix}1\\0\end{pmatrix}
$$

cannot have a [matrix inverse](matrix-inverse-split.md): the output $(1,0)^T$ cannot specify which of the two inputs occurred. Their difference $(1,-1)^T$ belongs to its [kernel](kernel-of-a-linear-map-split.md). Indeed $S(x,y)^T=(x+y,0)^T$ collapses the [plane](plane.md) to a [line](straight-line.md), its [matrix rank](matrix-rank.md) is one, and its [determinant](determinant.md) is zero. No subsequent [function](function-split.md) of the output alone can reconstruct every input.

An important use of the [matrix inverse](matrix-inverse-split.md) is describing the unique solution of a [linear system](system-of-linear-equations.md):

$$
Ax=b\iff x=A^{-1}b.
$$

For $b=(4,3)^T$, the preceding computation solves $2x_1+x_2=4$ and $x_1+x_2=3$, giving $x=(1,2)^T$. In computation, usually solve the [linear system](system-of-linear-equations.md) using [Gaussian elimination](gaussian-elimination.md) and a factorization such as an [LU decomposition](lu-decomposition.md), rather than forming every entry of the [matrix inverse](matrix-inverse-split.md). The inverse formula specifies the answer; a factorization provides a reusable way to compute it for each right-hand side.[MIT 18.06, Spring 2017 final solutions, problem 5(b): solve with triangular factors rather than computing inverses](https://www.mit.edu/~18.06/Spring17/final-sol.pdf)

Here the [LU decomposition](lu-decomposition.md) is especially simple:

$$
A=LU,\qquad
L=\begin{pmatrix}1&0\\\tfrac12&1\end{pmatrix},\qquad
U=\begin{pmatrix}2&1\\0&\tfrac12\end{pmatrix}.
$$

Solve $Ly=b$ by [forward substitution in a triangular system](forward-substitution-in-a-triangular-system.md): $y_1=4$ and $y_2=3-\tfrac12\cdot4=1$. Then solve $Ux=y$ by [backward substitution in a triangular system](backward-substitution-in-a-triangular-system.md): $x_2=2$ and $x_1=(4-2)/2=1$. The same factors work when $b$ changes. If the whole [matrix inverse](matrix-inverse-split.md) is actually needed, its $j$th column is the solution of $Ax=e_j$, where $e_j$ is the $j$th [standard basis](standard-basis.md) vector.

Reversing several operations means undoing the last one first. For [invertible matrices](invertible-matrix.md) of the same size,

$$
(AB)^{-1}=B^{-1}A^{-1},
$$

because $(AB)(B^{-1}A^{-1})=A(BB^{-1})A^{-1}=I$, and the product in the other order is also $I$. This is why a [change-of-basis matrix](change-of-basis-matrix.md) uses its [matrix inverse](matrix-inverse-split.md) to reverse the direction of coordinate conversion.

**Table of contents**

- [Matrix inversion](matrix-inversion.md)
- [Woodbury matrix identity](woodbury-matrix-identity.md)
- [Matrix inversion is not additive](matrix-inversion-is-not-additive.md)
- [Matrix commutation with an inverse](matrix-commutation-with-an-inverse.md)
- [Block matrix inverse](block-matrix-inverse.md)
  - [Block elimination](block-elimination.md)
  - [Choosing a different block pivot](choosing-a-different-block-pivot.md)
- [Sherman–Morrison formula](sherman-morrison-formula.md)
  - [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)
    - [Solvability of an affine rank-one vector equation](solvability-of-an-affine-rank-one-vector-equation.md)
- [Moore-Penrose inverse](moore-penrose-inverse.md)
  - [Overdetermined least-squares example](overdetermined-least-squares-example.md)
  - [Underdetermined minimum-norm example](underdetermined-minimum-norm-example.md)
  - [Small singular values in the Moore-Penrose inverse](small-singular-values-in-the-moore-penrose-inverse.md)
  - [Moore--Penrose inverse of a Hilbert-space operator](moore-penrose-inverse-of-a-hilbert-space-operator.md)
  - [Penrose equations](penrose-equations.md)
  - [Reverse-order law for the Moore--Penrose inverse](reverse-order-law-for-the-moore-penrose-inverse.md)
- [Push-through identity](push-through-identity.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (75)

- [Block matrix inverse](block-matrix-inverse.md)
- [Cartesian basis](cartesian-basis.md)
- [Cartesian basis under rotation](cartesian-basis-under-rotation.md)
- [Change-of-basis matrix](change-of-basis-matrix.md)
- [Cholesky decomposition](cholesky-decomposition.md)
- [Derivative of a local inverse map](derivative-of-a-local-inverse-map.md)
- [Dual lattice](dual-lattice.md)
- [Fundamental matrix of a finite absorbing Markov chain](fundamental-matrix-of-a-finite-absorbing-markov-chain.md)
- [Gauss-Seidel method](gauss-seidel-method.md)
- [Group representation](group-representation.md)
- [Implicit function theorem](implicit-function-theorem.md)
- [Inverse infinity-norm bound from diagonal dominance](inverse-infinity-norm-bound-from-diagonal-dominance.md)
- [Invertible matrix](invertible-matrix.md)
- [LU decomposition](lu-decomposition.md)
- [Matrix commutation with an inverse](matrix-commutation-with-an-inverse.md)
- [Matrix determinant lemma](matrix-determinant-lemma.md)
- [Matrix geometric series](matrix-geometric-series.md)
- [Matrix inverse](matrix-inverse-split.md)
- [Matrix inverse from a decaying matrix exponential](matrix-inverse-from-a-decaying-matrix-exponential.md)
- [Matrix preconditioner](matrix-preconditioner.md)
- [Matrix splitting](matrix-splitting.md)
- [Moore-Penrose inverse](moore-penrose-inverse.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/1a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/6c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/7b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/6a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/6d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-40/1/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/2a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/2b/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/38c/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-342/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/5/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/5/c/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/2/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-b/7/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/13/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/11/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/12/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/12/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/14/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/18/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/18/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/18/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-2/10/a/solution.md)
- [Powers of the identity plus a square-zero matrix](powers-of-the-identity-plus-a-square-zero-matrix.md)
- [Quantum Hall conductivity tensor inversion](quantum-hall-conductivity-tensor-inversion.md)
- [Rank-one matrix update](rank-one-matrix-update.md)
- [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)
- [Resistivity tensor](resistivity-tensor.md)
- [Rotation matrix](rotation-matrix.md)
- [Schur complement](schur-complement.md)
- [Sheet resistivity](sheet-resistivity.md)
- [Sherman–Morrison formula](sherman-morrison-formula.md)
- [Singular matrix](singular-matrix.md)
- [Singular value](singular-value.md)
- [Symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md)
- [Trace and local volume change](trace-and-local-volume-change.md)
- [Triangular solves for LU decomposition](triangular-solves-for-lu-decomposition.md)
- [Variation of inverse metric](variation-of-inverse-metric.md)
