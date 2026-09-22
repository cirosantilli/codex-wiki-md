# Fill-in

↑ **Parent:** [Sparse Gaussian elimination](sparse-gaussian-elimination.md)

[Fill-in](fill-in.md) consists of new nonzero positions created by [Gaussian elimination](gaussian-elimination.md), absent from the original [sparse matrix](sparse-matrix.md) in the same ordering. For a [Cholesky decomposition](cholesky-decomposition.md) $PAP^T=CC^T$, compare $C$ with the lower triangle of $PAP^T$, not with the unpermuted input. Each new undirected [edge](edge-of-a-graph.md) of the [elimination graph](elimination-graph.md) contributes one structural position in $C$. The [sparse elimination of a four-leaf star](sparse-elimination-of-a-four-leaf-star.md) gives six such positions when the center is eliminated first, and none when the leaves are eliminated first.

[Symbolic factorization](symbolic-factorization.md) predicts possible nonzeros from the pattern alone. An initially zero $a_{ij}$ becomes nonzero in a single scalar step if both $a_{ik}$ and $a_{kj}$ are nonzero; however, at later steps several contributions can cancel. For an exact example, let

$$
H=\begin{pmatrix}2&1&1&0\\1&2&0&1\\1&0&3&-1/3\\0&1&-1/3&3\end{pmatrix}.
$$

Eliminate indices $1,2$ in that order. The first [Schur complement](schur-complement.md), in order $(2,3,4)$, is

$$
\begin{pmatrix}3/2&-1/2&1\\-1/2&5/2&-1/3\\1&-1/3&3\end{pmatrix}.
$$

The second [pivot element](pivot-element.md) updates the $(3,4)$ entry to $-1/3-(-1/2)(1)/(3/2)=0$. The remaining block is $\operatorname{diag}(7/3,7/3)$, so all four [pivot elements](pivot-element.md) are positive and $H$ is a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md). The [elimination graph](elimination-graph.md) retains the structural [edge](edge-of-a-graph.md) $3-4$, but this exact choice of coefficients makes the numerical entry vanish. A small change to $H_{34}=H_{43}$ generally removes the cancellation.

Such an exact zero is different from discarding a small value computed with [floating-point arithmetic](floating-point-arithmetic-split.md). The [symbolic factorization](symbolic-factorization.md) deliberately reserves space for possible entries without depending on special numerical identities. A [perfect elimination ordering](perfect-elimination-ordering.md) creates no structural [fill-in](fill-in.md) at all; an ordering with cancellations need not have that property.

## ↑ Ancestors (8)

1. [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
2. [Gaussian elimination](gaussian-elimination.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Compressed sparse storage](compressed-sparse-storage.md)
- [Fill-in](fill-in.md)
- [Jacobi method](jacobi-method.md)
- [Leaf elimination of a tree-pattern positive-definite matrix](leaf-elimination-of-a-tree-pattern-positive-definite-matrix.md)
- [Minimum degree algorithm](minimum-degree-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/6/solution.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
- [Sparse elimination of a four-leaf star](sparse-elimination-of-a-four-leaf-star.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
- [Tridiagonal elimination recurrences](tridiagonal-elimination-recurrences.md)
- [Zero-pivot failure of tridiagonal elimination](zero-pivot-failure-of-tridiagonal-elimination.md)
