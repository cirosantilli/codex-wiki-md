<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the [metric travelling salesman problem](../../../../../metric-travelling-salesman-problem.md), a tour is a polynomial-size [complexity certificate](../../../../../certificate-complexity.md): list the vertices in cyclic visiting order. In [polynomial time](../../../../../polynomial-time.md) verify that every vertex occurs exactly once, add the encoded [integer](../../../../../integer.md) edge costs and compare the sum with the threshold. The certificate has $O(n\log n)$ bits, and addition uses a number of bits polynomial in the input length. If validity of the metric input is not treated as a promise, nonnegativity, symmetry and all triangle inequalities can also be checked in [polynomial time](../../../../../polynomial-time.md). Therefore **the decision problem belongs to [NP](../../../../../np-complexity.md)**.

An evaluation algorithm immediately decides a threshold instance by computing the optimum and comparing it with $L$. Conversely, suppose there is a polynomial-time decision algorithm. The optimum is an [integer](../../../../../integer.md) in $[0,nM]$, where $M$ is the largest edge cost; any fixed cyclic ordering gives the upper bound. [Binary search](../../../../../binary-search.md) on this interval using threshold queries finds the exact minimum. It makes $O(\log(nM+1))$ queries, and every queried threshold has polynomial encoding length. Thus the time is polynomial in the bit length, even when $M$ is numerically large. Zero-cost and trivial small instances can be handled directly. Consequently

$$
\boxed{\text{Polynomial-time evaluation exists}\ \Longleftrightarrow\ \text{polynomial-time decision exists}.}
$$

This concerns the optimum value; constructing an optimal tour is the separate optimization task.

For the hardness reduction, start with an undirected graph $G$ on $n\ge3$ vertices and form the complete graph with costs

$$
c_{ij}=\begin{cases}1,&\{i,j\}\in E(G),\\2,&\{i,j\}\notin E(G),\end{cases}\qquad i\ne j.
$$

These costs satisfy the [triangle inequality](../../../../../triangle-inequality.md), since every direct cost is at most two and every two-edge path costs at least two. Set the threshold to $n$. Every tour has exactly $n$ edges, each costing at least one. Hence it has cost at most $n$ precisely when all its edges came from $G$, which is precisely the existence of a [Hamiltonian cycle](../../../../../hamilton-cycle.md) in $G$. The construction and threshold encoding are polynomial-time. Thus the assumed [NP-completeness](../../../../../np-completeness.md) of the Hamiltonian circuit problem gives [NP-hardness](../../../../../np-hardness.md) of metric TSP; together with its [NP](../../../../../np-complexity.md) membership this proves **[NP-completeness](../../../../../np-completeness.md) of metric TSP decision**.

For the approximation, compute a [minimum spanning tree](../../../../../minimum-spanning-tree.md) $T$. Deleting any one edge of an optimal tour leaves a [spanning tree](../../../../../spanning-tree.md), so nonnegative costs imply

$$
c(T)\le\operatorname{OPT}.
$$

Double every tree edge. The resulting connected multigraph has even degrees and hence an [Euler circuit](../../../../../euler-circuit.md), of cost $2c(T)$. Traverse it and skip previously visited vertices, except for the final return to the start. Each skip replaces a path by its direct edge; repeated use of the [triangle inequality](../../../../../triangle-inequality.md) shows that no replacement increases cost. The result is a tour visiting every vertex exactly once and satisfying

$$
\boxed{c(\text{returned tour})\le2c(T)\le2\operatorname{OPT}.}
$$

The Euler traversal and shortcutting take [polynomial time](../../../../../polynomial-time.md), so the assumed polynomial-time MST routine supplies the requested [polynomial-time algorithm](../../../../../polynomial-time-algorithm.md). This is the [double-tree approximation for metric TSP](../../../../../double-tree-approximation-for-metric-tsp.md). In the relative-error convention, $c/\operatorname{OPT}-1\le1$ when the optimum is positive, explaining the printed term “1-approximation”; in the multiplicative convention it is a factor-two approximation. If the optimum is zero, the same bound forces the returned tour to have zero cost as well.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
