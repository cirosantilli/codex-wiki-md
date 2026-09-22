# Sparse Gaussian elimination

↑ **Parent:** [Gaussian elimination](gaussian-elimination.md)

[Sparse Gaussian elimination](sparse-gaussian-elimination.md) solves a [linear system](system-of-linear-equations.md) by [Gaussian elimination](gaussian-elimination.md) while exploiting its [sparse matrix](sparse-matrix.md) structure to avoid storing zeros and performing unnecessary [arithmetic operations](arithmetic-operation.md). The catch is that zeros in the input need not remain zero: eliminating a shared unknown can couple two equations that previously had no direct coupling. These new positions are [fill-in](fill-in.md), and their number can depend strongly on the order of elimination.

For a real [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md), the usual direct method is a [Cholesky decomposition](cholesky-decomposition.md). Choose an ordering, use [symbolic factorization](symbolic-factorization.md) to allocate the predicted factor entries, compute their values, then solve two [triangular systems](triangular-system.md). [Compressed sparse storage](compressed-sparse-storage.md) makes the reduced storage useful. General [LU decomposition](lu-decomposition.md) may also need numerical [partial pivoting](columnwise-partial-pivoting.md), so an ordering chosen for sparsity can change during factorization.[Applications of Parallel Computers, CS267, Spring 1996; CS267, Lecture 27, 23 April 1996, Cholesky versus LU Decomposition: distinction between numerical pivot selection and advance ordering, and phases 1–4; Sparse Matrix Storage Schemes](applications-of-parallel-computers-cs267-spring-1996/lecture-27-sparse-gaussian-elimination.md)

For a fixed ordering, let $P$ be the [permutation matrix](permutation-matrix.md) that puts the unknowns in that order. Permute both rows and columns:

$$
B=PAP^T=CC^T,\qquad Cy=Pb,\qquad C^Tz=y,\qquad x=P^Tz.
$$

Here $C$ is the [lower triangular matrix](lower-triangular-matrix.md) in the [Cholesky decomposition](cholesky-decomposition.md) of $B$; $z=Px$. [Forward substitution](forward-substitution.md) and [back substitution](back-substitution.md) give the original solution. The simultaneous permutation preserves the [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) property because $v^TBv=(P^Tv)^TA(P^Tv)>0$ for every nonzero [vector](vector.md) $v$. A row permutation alone generally loses the [symmetric matrix](symmetric-matrix.md) structure.

The local mechanism is a [Schur complement](schur-complement.md). If the active [pivot element](pivot-element.md) is $a_{kk}$, then for remaining indices $i,j$,

$$
a_{ij}^{\mathrm{new}}=a_{ij}-\frac{a_{ik}a_{kj}}{a_{kk}}.
$$

Even when $a_{ij}=0$, two nonzero couplings through $k$ make the second term nonzero. Thus the [elimination graph](elimination-graph.md) removes $k$ and joins its remaining neighbors into a [clique](clique-graph-theory.md). The [fill-path criterion for symmetric elimination](fill-path-criterion-for-symmetric-elimination.md) extends this local rule across several steps. The [elimination tree](elimination-tree.md) organizes the resulting dependencies; the [minimum degree algorithm](minimum-degree-algorithm.md) and [nested dissection](nested-dissection.md) choose orderings to control them.

This connection between [graphs](graph-split.md) and [linear systems](system-of-linear-equations.md) was already explicit in [Donald J. Rose](donald-j-rose.md), [R. Endre Tarjan](robert-tarjan.md) and [George S. Lueker](george-s-lueker.md)'s 1976 study of [fill-in](fill-in.md) and [perfect elimination orderings](perfect-elimination-ordering.md).[Abstract: symmetric positive-definite systems, fill calculation for a prescribed ordering, and algorithms for special orderings; publication information, June 1976](algorithmic-aspects-of-vertex-elimination-on-graphs-by-donald-j-rose-and-others.md)

**Table of contents**

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

## ↑ Ancestors (7)

1. [Gaussian elimination](gaussian-elimination.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Gaussian elimination](gaussian-elimination.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/6/solution.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
