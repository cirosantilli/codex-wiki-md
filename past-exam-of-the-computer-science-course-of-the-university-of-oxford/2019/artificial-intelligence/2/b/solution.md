<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the knight-variable representation and build a placement one knight at a time. The initial state is the empty placement. An action places the next knight on an empty square attacking no previously placed knight; the [search transition model](../../../../../search-transition-model.md) appends that square. The [goal test](../../../../../goal-test.md) is that $k$ knights have been placed. Each action adds exactly one, so any solution has depth **$k$**.

Put $N=n^2$. At depth $j$, there are at most $N-j$ choices, hence [branching factor](../../../../../branching-factor.md) at most $N$. A coarse [search tree](../../../../../search-tree.md) size bound is $1+N+\cdots+N^k$. Keeping the shrinking choice count gives the sharper bound

$$
\sum_{j=0}^{k}(N)_j,\qquad (N)_j=\frac{N!}{(N-j)!},
$$

where $(N)_j$ is a [falling factorial](../../../../../falling-factorial.md). This counts ordered placements before attack pruning.

For a full expansion down to depth $k$, the number of depth-$k$ leaves is at most **$(N)_k$**, or approximately $n^{2k}$ when $k$ is small relative to $N$. If $I_k$ denotes the number of legal unlabelled $k$-knight placements, the exact number of legal depth-$k$ leaves is $k!I_k$. There can also be earlier dead-end leaves: a legal placement may leave no further nonattacking square. Writing $M_j$ for the number of inclusion-maximal legal $j$-knight placements, the fully explored pruned tree has

$$
k!I_k+\sum_{j=0}^{k-1}j!M_j
$$

leaves. Its leaf count is still at most the unpruned $(N)_k$, since each early leaf replaces a disjoint nonempty subtree of the unpruned tree. [Breadth-first search](../../../../../breadth-first-search.md) that stops at its first goal can construct less of the last layer; if no solution exists, it exhausts the reachable partial placements.

Identifying different insertion orders changes the representation. With a state that is an unlabelled [set](../../../../../set-split.md) of occupied squares and repeated-state elimination, the corresponding depth-$k$ state bound is $\binom Nk$, with $I_k$ legal goal states. The factorial and binomial bounds refer to these different representations, not competing counts of the same tree.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
