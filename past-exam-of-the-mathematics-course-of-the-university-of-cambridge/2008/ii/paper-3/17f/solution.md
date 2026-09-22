<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

The [chromatic polynomial](../../../../../chromatic-polynomial.md) $p_G(t)$ counts proper vertex colorings with $t$ labeled colors at positive integer $t$. For an edge $e$, the [deletion-contraction recurrence for the chromatic polynomial](../../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) is $p_G=p_{G-e}-p_{G/e}$, where parallel edges in the contracted graph are merged. Induction on edges, starting from the edgeless polynomial $t^n$, shows that the coefficients have alternating signs: the contracted graph has one fewer vertex, so subtracting its alternating polynomial reinforces the same signs. The leading coefficient stays one. The coefficient of $t^{n-1}$ decreases by one per added edge, hence it is $-m$. Thus $p_G(t)=\sum_{i=0}^n(-1)^{n-i}a_it^i$, with $a_n=1$, $a_{n-1}=m$ and all $a_i\geq0$.

For a [tree](../../../../../tree-graph-theory.md), choose a root, give it any of $t$ colors, and give every other vertex any of the $t-1$ colors different from its parent. This gives $p_G(t)=t(t-1)^{n-1}$. Conversely, a graph with this polynomial has $m=n-1$. The [chromatic polynomial](../../../../../chromatic-polynomial.md) of a disjoint union is the product of those of its connected components, each divisible by $t$. The given polynomial has a simple zero at zero, forcing a single connected component. A connected graph with $n-1$ edges is a tree. **The converse holds.**

Finally the polynomial determines the number of vertices, the number of edges and the [chromatic number](../../../../../chromatic-number.md). If it equals that of the [Turán graph](../../../../../turan-graph.md) $T_r(n)$, with $1\leq r\leq n$, then $G$ has chromatic number $r$, so has no $K_{r+1}$, and has the maximum possible number of edges for such a graph. The equality case in [Turán's theorem](../../../../../turan-s-theorem.md) makes $G$ isomorphic to $T_r(n)$. This is the [chromatic polynomial determines a Turán graph](../../../../../chromatic-polynomial-determines-a-turan-graph.md) property. If $r>n$, the graph is simply complete and its edge count already determines it.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
