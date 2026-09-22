<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [extreme point](../../../../../../extreme-point.md) of a [convex set](../../../../../../convex-set.md) cannot be written as a nontrivial convex combination of two distinct members. If a [permutation matrix](../../../../../../permutation-matrix.md) $P=\theta B+(1-\theta)C$ with $0<\theta<1$ and $B,C$ doubly stochastic, each zero entry of $P$ forces the corresponding entries of $B,C$ to be zero by nonnegativity. The unique possible nonzero entry in each row must then be one by the row sum. Thus $B=C=P$, proving that every [permutation matrix](../../../../../../permutation-matrix.md) is extreme.

Conversely, let $A$ be a [doubly stochastic matrix](../../../../../../doubly-stochastic-matrix.md) that is not a [permutation matrix](../../../../../../permutation-matrix.md). At least one entry lies strictly between zero and one. Form a [bipartite graph](../../../../../../bipartite-graph.md) whose two vertex classes are rows and columns, with edges precisely at these fractional entries. Every incident row has at least two fractional entries: a single fractional entry, with all other entries zero or one, could not give row sum one. The same holds for columns.

A finite nonempty graph whose incident vertices all have degree at least two contains a cycle. In a [bipartite graph](../../../../../../bipartite-graph.md) that cycle has even length. Assign alternating signs $+1,-1$ to its entries, giving a nonzero matrix $D$ with every row and column sum zero. Choose $\varepsilon>0$ smaller than the distance of each cycle entry from both zero and one. Then $A+\varepsilon D$ and $A-\varepsilon D$ remain [doubly stochastic matrices](../../../../../../doubly-stochastic-matrix.md), are distinct, and satisfy

$$
A=\tfrac12(A+\varepsilon D)+\tfrac12(A-\varepsilon D).
$$

So $A$ is not extreme. Therefore

$$
\boxed{\operatorname{Ext}(\mathcal C)=\{\text{permutation matrices}\}.}
$$

This [alternating-cycle perturbation of a doubly stochastic matrix](../../../../../../alternating-cycle-perturbation-of-a-doubly-stochastic-matrix.md) proves the extreme-point part of the [Birkhoff-von Neumann theorem](../../../../../../birkhoff-von-neumann-theorem.md) directly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
