<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A chain of $r$ diamond-shaped graph stages has $3r+1$ vertices and $4r$ edges, but $2^r$ distinct source-to-target paths: at each stage choose either of two branches. Each path has its own inequality. Therefore **the number of displayed path constraints is not polynomially bounded** in the graph size. Redundancy among some inequalities would not change this count of the given formulation.

The positive integer edge costs imply, for any feasible point,

$$
\|x\|_2\leq\|x\|_1=\sum_e x_e\leq\sum_e c_ex_e\leq k\leq100.
$$

Thus the feasible set lies in the Euclidean ball of radius $100$ centered at zero. That ball lies inside $[-100,100]^m$, so its volume is at most $200^m$. This proves the requested **$O(200^m)$ enclosing-volume bound**, and provides an initial ellipsoid, for example with center zero and shape matrix $10^4I$.

The [ellipsoid method](../../../../../ellipsoid-method.md) needs a [separation oracle](../../../../../separation-oracle.md), rather than an explicit list of every constraint. For a proposed center $z$, first scan the coordinates and the budget inequality. If some $z_e<0$, some $z_e>1$, or $\sum_ec_ez_e>k$, return the corresponding violated inequality as the separating half-space. These tests take $O(m)$ arithmetic operations.

Once those tests pass, assign nonnegative edge length $z_e$ to every edge and solve the [shortest path problem](../../../../../shortest-path-problem.md) from $s$ to $t$. The [Dijkstra algorithm](../../../../../dijkstra-algorithm.md) finds a minimum-length path and stores its predecessors in [polynomial time](../../../../../polynomial-time.md). If its length is less than one, return

$$
\sum_{e\in p}x_e\geq1
$$

for the minimizing path $p$. This inequality contains every feasible point and is violated by $z$. If the shortest length is at least one, every path constraint holds; if no path exists, those constraints are vacuous. In either case $z$ is feasible. This is [path-constraint separation by shortest paths](../../../../../path-constraint-separation-by-shortest-paths.md); checking a single shortest path replaces checking exponentially many paths.

The rational [ellipsoid method](../../../../../ellipsoid-method.md) feasibility theorem now gives polynomial running time in the dimension and coefficient encoding bounds when the oracle runs in [polynomial time](../../../../../polynomial-time.md). Here every path row has coefficients zero or one, and all other coefficients and right sides are bounded integers. Although there are exponentially many rows, their individual encoding lengths are polynomial in $m$. The containing-radius bound and the rational precision bounds are also polynomially describable. For a simple graph $m=O(n^2)$, this gives **a worst-case running time polynomial in $n$**; in general the natural bound is polynomial in the encoded graph size $n+m$.

Use the exact rational feasibility version of the [ellipsoid method](../../../../../ellipsoid-method.md), which handles lower-dimensional polyhedra by rational precision bounds or an appropriate relaxation. Nonemptiness must not be inferred from a positive-volume argument: this feasible set can have empty interior. The allowed algorithmic theorem supplies that detail, while the explicit shortest-path oracle supplies the crucial efficient separation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
