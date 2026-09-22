# Gaussian elimination

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_elimination)

Gaussian elimination applies elementary row operations to reduce a linear system to triangular form. Dense elimination uses $O(n^3)$ arithmetic operations.

[Gaussian elimination](gaussian-elimination.md) solves a [linear system](system-of-linear-equations.md) by removing one unknown from later equations at each step. Write the coefficients and right-hand side together as an [augmented matrix](augmented-matrix.md) $[A\mid b]$. Apply the same [elementary row operations](elementary-row-operation.md) to both parts until the coefficients form a [row echelon form](row-echelon-form.md); for a square [invertible matrix](invertible-matrix.md), this gives an [upper triangular matrix](upper-triangular-matrix.md) system. Then [back substitution](back-substitution.md) recovers the unknowns from the last equation upward. The useful simplification is that each successive equation involves fewer unknowns, while the set of solutions stays the same.

Why do [elementary row operations](elementary-row-operation.md) preserve solutions? Interchanging equations changes only their order. Multiplying an equation by a nonzero [scalar](scalar.md) can be undone by division. Replacing equation $i$ by itself plus $c$ times equation $j$, with $i\ne j$, can be undone by adding $-c$ times the unchanged equation $j$. Equivalently, an [elementary matrix](elementary-matrix.md) $E$ is an [invertible matrix](invertible-matrix.md), so $Ax=b$ if and only if $EAx=Eb$. Applying an operation to $A$ without also applying it to $b$ loses this equivalence.

At step $k$, choose a nonzero [pivot element](pivot-element.md) $a_{kk}$ after any row interchange. For every $i>k$, form the [elimination multiplier](elimination-multiplier.md) $m_i=a_{ik}/a_{kk}$ and perform the [elementary row operation](elementary-row-operation.md) $R_i\leftarrow R_i-m_iR_k$. Its coefficient in column $k$ becomes $a_{ik}-(a_{ik}/a_{kk})a_{kk}=0$ in exact arithmetic. Later operations combine rows that already have zeros in earlier columns, so those zeros survive. If an active column has no nonzero candidate, general [row echelon form](row-echelon-form.md) reduction skips it; a square [invertible matrix](invertible-matrix.md) always has a candidate at each step with suitable row interchanges. [Partial pivoting](columnwise-partial-pivoting.md) also considers [roundoff error](round-off-error.md) when selecting the candidate.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §2.6.1, Definition 2.6.1: select the largest absolute candidate; §2.6.3: permute the right-hand side too](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/2-6-row-pivoting.md)

For a dense $n\times n$ [matrix](matrix.md) with one right-hand side, the classical [algorithm](algorithm-split.md) uses $\tfrac23n^3+O(n^2)$ [arithmetic operations](arithmetic-operation.md) over the [real numbers](real-number.md), counting each [addition](addition.md), [subtraction](subtraction.md), [multiplication](multiplication.md) and [division](division-mathematics.md) as one. At step $k$, the coefficient update has $(n-k)^2$ entries, each costing one [multiplication](multiplication.md) and one [subtraction](subtraction.md); the [elimination multipliers](elimination-multiplier.md), right-hand-side updates and [back substitution](back-substitution.md) contribute lower-order terms. Searching for [partial pivoting](columnwise-partial-pivoting.md) adds $O(n^2)$ comparisons, and storing the dense coefficients uses $O(n^2)$ space. These assumptions exclude the different storage and work patterns of [sparse Gaussian elimination](sparse-gaussian-elimination.md); the exact loop counts appear in [LU factorization and solve costs](lu-factorization-and-solve-costs.md). Here $O$ denotes [Big O notation](big-o-notation.md).

Recording the same steps as an [LU decomposition](lu-decomposition.md) makes [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md) possible. This is useful whenever the coefficients stay fixed while the forcing [vector](vector.md) changes: the expensive elimination is done once. The choice of [pivot element](pivot-element.md) matters even when the [linear system](system-of-linear-equations.md) is well conditioned, as [Tiny-pivot roundoff in Gaussian elimination](tiny-pivot-roundoff-in-gaussian-elimination.md) demonstrates.

**Table of contents**

- [Bareiss algorithm](bareiss-algorithm.md)
- [Gaussian elimination with a row swap](gaussian-elimination-with-a-row-swap.md)
- [Pivot element](pivot-element.md)
- [Elimination multiplier](elimination-multiplier.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
  - [Sparse elimination of a four-leaf star](sparse-elimination-of-a-four-leaf-star.md)
  - [Leaf elimination of a tree-pattern positive-definite matrix](leaf-elimination-of-a-tree-pattern-positive-definite-matrix.md)
  - [Symbolic factorization](symbolic-factorization.md)
  - [Elimination tree](elimination-tree.md)
  - [Nested dissection](nested-dissection.md)
  - [Minimum degree algorithm](minimum-degree-algorithm.md)
  - [Fill-in](fill-in.md)
  - [Matrix graph](matrix-graph.md)
    - [Elimination graph](elimination-graph.md)
      - [Fill-path criterion for symmetric elimination](fill-path-criterion-for-symmetric-elimination.md)
- [Columnwise partial pivoting](columnwise-partial-pivoting.md)
  - [Tiny-pivot roundoff in Gaussian elimination](tiny-pivot-roundoff-in-gaussian-elimination.md)
- [Row echelon form](row-echelon-form.md)
  - [Row-equivalent matrices](row-equivalent-matrices.md)
  - [Row reduction with a parameterized right-hand side](row-reduction-with-a-parameterized-right-hand-side.md)
  - [Reduced row echelon form](reduced-row-echelon-form.md)
    - [Reading solutions from reduced row echelon form](reading-solutions-from-reduced-row-echelon-form.md)
    - [Uniqueness of reduced row echelon form](uniqueness-of-reduced-row-echelon-form.md)
- [Elementary row operation](elementary-row-operation.md)
  - [Elementary matrix](elementary-matrix.md)

## ↑ Ancestors (6)

1. [Numerical linear algebra](numerical-linear-algebra-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (41)

- [Augmented matrix](augmented-matrix.md)
- [Columnwise partial pivoting](columnwise-partial-pivoting.md)
- [Computed three-by-three LU decomposition](computed-three-by-three-lu-decomposition.md)
- [Elementary row operation](elementary-row-operation.md)
- [Elimination graph](elimination-graph.md)
- [Field](field.md)
- [Fill-in](fill-in.md)
- [Fourier diagonalization of a circulant matrix](fourier-diagonalization-of-a-circulant-matrix.md)
- [Gaussian elimination](gaussian-elimination.md)
- [Jacobi method](jacobi-method.md)
- [LU decomposition](lu-decomposition.md)
- [LU factorization and solve costs](lu-factorization-and-solve-costs.md)
- [Matrix inverse](matrix-inverse-split.md)
- [Numerical method](numerical-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-17/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/6d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/2b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-7/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/8c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/5c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/5b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324/4/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-101/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/11/a/i/solution.md)
- [Pivot element](pivot-element.md)
- [Pivoted LU decomposition](pivoted-lu-decomposition.md)
- [Row reduction with a parameterized right-hand side](row-reduction-with-a-parameterized-right-hand-side.md)
- [Simon's algorithm](simon-s-algorithm.md)
- [Sparse elimination of a four-leaf star](sparse-elimination-of-a-four-leaf-star.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
- [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)
- [Unimodular matrix](unimodular-matrix.md)
- [Uniqueness of reduced row echelon form](uniqueness-of-reduced-row-echelon-form.md)
