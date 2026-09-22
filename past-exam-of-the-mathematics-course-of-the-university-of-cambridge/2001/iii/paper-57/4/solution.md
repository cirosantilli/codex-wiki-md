<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the undirected [graph](../../../../../graph-split.md) of the symmetric off-diagonal sparsity pattern. Reading the original matrix gives the edges

$$
\{1,3\},\ \{1,4\},\ \{1,7\},\ \{2,8\},\ \{4,5\},\ \{5,8\},\ \{6,7\},\ \{7,9\}.
$$

This connected nine-vertex, eight-edge graph is a [tree](../../../../../tree-graph-theory.md). A leaf-removal [perfect elimination ordering](../../../../../perfect-elimination-ordering.md) is

$$
\boxed{3,\ 2,\ 6,\ 9,\ 8,\ 5,\ 4,\ 7,\ 1.}
$$

The corresponding lists of remaining neighbors are, in order, $\{1\},\{8\},\{7\},\{7\},\{5\},\{4\},\{1\},\{1\},\varnothing$. Thus simultaneous row and column permutation to this ordering allows [Gaussian elimination](../../../../../gaussian-elimination.md) without [fill-in](../../../../../fill-in.md).

Here are the precise facts that justify the procedure. First, eliminating index $i$ makes the remaining entries

$$
a_{jk}^{\rm new}=a_{jk}-\frac{a_{ji}a_{ik}}{a_{ii}}.
$$

Only pairs of remaining neighbors of $i$ can acquire a new nonzero entry. Consequently a vertex whose remaining neighbors form a clique can be eliminated without structural fill. Such a vertex is simplicial. An ordering in which each successive vertex is simplicial is a [perfect elimination ordering](../../../../../perfect-elimination-ordering.md). The graph characterization says that a graph admits such an ordering if and only if it is a [chordal graph](../../../../../chordal-graph.md), meaning every cycle of length at least four has a chord. A tree has no cycles; more concretely, every nontrivial finite tree has a leaf, and removing a leaf leaves a forest. These statements explain why successive leaf removal works here without having to find a general-purpose chordal ordering.

Second, for a symmetric [positive-definite matrix](../../../../../positive-definite-matrix.md), every diagonal pivot and every successive [Schur complement](../../../../../schur-complement.md) is positive definite. For example, if the first pivot is $a_{ii}$ and its coupling column is $b$, then for any nonzero remaining vector $x$,

$$
x^T\left(C-\frac{bb^T}{a_{ii}}\right)x
=\begin{pmatrix}-b^Tx/a_{ii}\\x\end{pmatrix}^{\!T}
\begin{pmatrix}a_{ii}&b^T\\b&C\end{pmatrix}
\begin{pmatrix}-b^Tx/a_{ii}\\x\end{pmatrix}>0.
$$

Thus no zero pivot requires abandoning the proposed ordering. Since each eliminated vertex here has at most one remaining neighbor, its Schur update changes only a diagonal entry. This proves the claimed fill-free [LDL decomposition](../../../../../ldl-decomposition.md) or [Cholesky decomposition](../../../../../cholesky-decomposition.md) for every positive-definite matrix with the given pattern, including cases with additional accidental zeros. It is [leaf elimination of a tree-pattern positive-definite matrix](../../../../../leaf-elimination-of-a-tree-pattern-positive-definite-matrix.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
