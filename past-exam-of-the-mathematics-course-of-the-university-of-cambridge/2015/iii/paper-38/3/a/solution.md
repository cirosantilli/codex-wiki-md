<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the [oriented incidence matrix](../../../../../../oriented-incidence-matrix.md) convention with $+1$ at an edge's tail and $-1$ at its head. Let $b_i$ be net supply, so $\sum_i b_i=0$. The [uncapacitated minimum-cost flow](../../../../../../uncapacitated-minimum-cost-flow.md) problem on a finite [directed graph](../../../../../../directed-graph.md) is

$$
\min_{f\geq0}\sum_{(i,j)\in E}c_{ij}f_{ij}\quad\text{subject to }\sum_{j:(i,j)\in E}f_{ij}-\sum_{j:(j,i)\in E}f_{ji}=b_i,
$$

or $Bf=b$. Negative $b_i$ denotes net demand. Costs may have either sign; the problem can be infeasible or unbounded.

For vertex [network dual potentials](../../../../../../network-dual-potential.md) $\pi$, the [optimization Lagrangian](../../../../../../optimization-lagrangian.md) is

$$
L(f,\pi)=c^Tf+\pi^T(b-Bf)=\pi^Tb+\sum_{(i,j)\in E}(c_{ij}-\pi_i+\pi_j)f_{ij}.
$$

The infimum over $f\geq0$ is finite exactly when every [network reduced cost](../../../../../../network-reduced-cost.md) $r_{ij}=c_{ij}-\pi_i+\pi_j$ is nonnegative. Thus the [Lagrangian dual problem](../../../../../../lagrangian-dual-problem.md) and [complementary slackness](../../../../../../complementary-slackness.md) are

$$
\boxed{\max_\pi\pi^Tb\quad\text{subject to }r_{ij}\geq0,\qquad f_{ij}r_{ij}=0\text{ for every edge}.}
$$

A feasible flow and feasible [network dual potentials](../../../../../../network-dual-potential.md) satisfying these equalities have equal costs and are optimal by [weak duality](../../../../../../weak-duality.md).

If the underlying [undirected graph](../../../../../../undirected-graph.md) is connected, deleting one redundant balance row makes the [oriented incidence matrix](../../../../../../oriented-incidence-matrix.md) have rank $|V|-1$. A set of $|V|-1$ independent edge columns is exactly a [spanning tree](../../../../../../spanning-tree.md). Set all non-tree flows to zero, solve the tree balances, and check nonnegativity to obtain a [basic feasible solution](../../../../../../basic-feasible-solution.md). Basic tree edges may have zero flow, which is [degeneracy in linear programming](../../../../../../degeneracy-in-linear-programming.md). Requiring $r_{ij}=0$ on tree edges determines [network dual potentials](../../../../../../network-dual-potential.md) up to a common additive constant. If every non-tree [network reduced cost](../../../../../../network-reduced-cost.md) is nonnegative, the tree flow is optimal. This is the basis of the [network simplex algorithm](../../../../../../network-simplex-algorithm.md). If the graph is disconnected, solve the balances separately in each component; each component must have total net supply zero and uses its own [spanning tree](../../../../../../spanning-tree.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
