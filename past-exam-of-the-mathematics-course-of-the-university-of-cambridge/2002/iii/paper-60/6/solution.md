<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

[Sparse Gaussian elimination](../../../../../sparse-gaussian-elimination.md) seeks a direct solution while preserving the advantage of a small number of nonzeros. The main issue is that eliminating unknowns creates new interactions between the remaining unknowns. For a symmetric positive-definite system, simultaneous row and column permutation merely changes the elimination order, and [Cholesky decomposition](../../../../../cholesky-decomposition.md) or [LDL decomposition](../../../../../ldl-decomposition.md) can proceed without pivoting. Partition one elimination step as

$$
A=\begin{pmatrix}a&b^T\\b&C\end{pmatrix},\qquad
A=\begin{pmatrix}1&0\\b/a&I\end{pmatrix}
\begin{pmatrix}a&0\\0&C-bb^T/a\end{pmatrix}
\begin{pmatrix}1&b^T/a\\0&I\end{pmatrix}.
$$

The remaining system has the [Schur complement](../../../../../schur-complement.md) $C-bb^T/a$. It is positive-definite because, for any nonzero $z$, minimizing the positive quadratic form of $A$ over the first coordinate gives $z^T(C-bb^T/a)z>0$. This both justifies the next positive pivot and identifies exactly where fill can appear.

The [matrix graph](../../../../../matrix-graph.md) of a symmetric sparsity pattern has one vertex per unknown and an edge $i-j$ when $a_{ij}$ is structurally nonzero. At pivot $k$, the update

$$
a_{ij}\longleftarrow a_{ij}-a_{ik}a_{kj}/a_{kk}
$$

can change an entry only when both $i$ and $j$ are current neighbors of $k$. Thus the [elimination graph](../../../../../elimination-graph.md) operation removes $k$ and makes its remaining neighbors a [clique](../../../../../clique-graph-theory.md). Edges absent before this update are [fill-in](../../../../../fill-in.md). The [graph](../../../../../graph-split.md) describes structural or generic nonzeros: special cancellations in the numerical values can reduce the actual fill, but cannot justify omitting possible entries in advance.

A useful global description is the [fill-path criterion for symmetric elimination](../../../../../fill-path-criterion-for-symmetric-elimination.md). After a set $E$ has been eliminated, remaining vertices $i,j$ are adjacent generically exactly when their original [graph](../../../../../graph-split.md) contains a path from $i$ to $j$ with all internal vertices in $E$. The assertion starts with the original edges when $E$ is empty. Eliminating the next vertex concatenates two earlier such paths through it; conversely, split any allowed path at the newly eliminated vertex to recover the two earlier connections. This induction explains why sparse long-range couplings may eventually become dense.

The order is decisive. For a star with four leaves, eliminating a leaf only changes the diagonal of its sole neighbor and creates no fill. Repeated leaf elimination preserves this property. Eliminating the central vertex first instead connects all four leaves, creating six edges and a dense four-variable trailing system. This occurs, for example, in a positive-definite star [matrix](../../../../../matrix.md) with central diagonal $5$, leaf diagonals $2$ and edge entries $-1$; no cancellation removes the new leaf couplings.

<a id="6/image-the-same-sparse-star-graph-creates-no-fill-with-leaf-elimination-and-six-fill-edges-with-central-elimination"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60-elimination.png)

**[Figure 1](#6/image-the-same-sparse-star-graph-creates-no-fill-with-leaf-elimination-and-six-fill-edges-with-central-elimination). The same sparse star graph creates no fill with leaf elimination and six fill edges with central elimination**.

For an arbitrary [graph](../../../../../graph-split.md), an ordering creates no fill precisely when each pivot's later neighbors are already a [clique](../../../../../clique-graph-theory.md), namely a [perfect elimination ordering](../../../../../perfect-elimination-ordering.md). Such an ordering exists exactly for a [chordal graph](../../../../../chordal-graph.md). A chordless cycle of length at least four illustrates the obstruction: its first removed vertex connects its two previously nonadjacent neighbors. Eliminating in a chosen order adds chords until the completed [graph](../../../../../graph-split.md) is chordal. Thus sparsity of the original [matrix](../../../../../matrix.md) alone does not guarantee sparse factors; the [graph](../../../../../graph-split.md) and its ordering matter together.

If pivot $j$ has $d_j$ later neighbors, its column contains $d_j+1$ factor entries and its symmetric outer-product update costs $O(d_j^2)$ arithmetic. The total storage is governed by $\sum_j(d_j+1)$ and the work by $\sum_j(d_j+1)^2$. A band ordering with [matrix bandwidth](../../../../../matrix-bandwidth.md) $b$ gives the familiar $O(Nb)$ storage and $O(Nb^2)$ work, but a narrow profile or [graph](../../../../../graph-split.md) separator can do better than a single global band. The [minimum degree algorithm](../../../../../minimum-degree-algorithm.md) greedily chooses a current low-degree pivot; it often keeps immediate updates small, but it must account for previously created fill and need not minimize total fill.

[Nested dissection](../../../../../nested-dissection.md) instead finds a small [vertex separator](../../../../../vertex-separator.md), recursively eliminates disconnected subdomains, and leaves separator variables until last. For a regular two-dimensional grid with $N$ unknowns, a separator has $O(\sqrt N)$ vertices. Its dense final work is $O(N^{3/2})$, and recursive balanced separation gives

$$
W(N)\leq2W(N/2)+CN^{3/2}=O(N^{3/2}).
$$

At each level the summed separator-square storage is $O(N)$, giving $O(N\log N)$ factor storage over the logarithmic number of levels. These estimates assume the usual geometric separator structure; they are not guarantees for every sparse [graph](../../../../../graph-split.md). Independent subdomains also expose parallel work.

In a practical solver a [symbolic factorization](../../../../../symbolic-factorization.md) phase uses the pattern and ordering to allocate factor storage and schedule updates. For the lower-triangular factor, the [elimination tree](../../../../../elimination-tree.md) takes the parent of column $j$ to be its first later row index containing a structural nonzero. Descendant updates flow towards those later pivots, making the tree useful for dependency scheduling and the organization of the factorization. [Compressed sparse storage](../../../../../compressed-sparse-storage.md) records only entries and indices; the numerical phase then computes the values, followed by forward and backward substitution. The factors can be reused for many right-hand sides.

Finally, structural efficiency must be balanced with [numerical stability](../../../../../stability-of-a-numerical-method.md). For a nonsymmetric system the pattern can be represented by a directed or bipartite [graph](../../../../../graph-split.md), and elimination creates edges from incoming to outgoing neighbors. Separate row and column permutations are possible. A fill-reducing column ordering does not ensure a safe pivot: scaling and [partial pivoting](../../../../../columnwise-partial-pivoting.md) may be needed to prevent division by a tiny number and large growth. Such row interchanges can change the predicted fill. Positive-definite symmetric problems avoid this conflict; general sparse solvers must manage it explicitly. **Graph-based ordering controls factor sparsity, while pivoting controls numerical safety; an effective sparse factorization needs both.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
