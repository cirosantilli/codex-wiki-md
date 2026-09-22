<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a directed graph, the [uncapacitated minimum-cost flow](../../../../../uncapacitated-minimum-cost-flow.md) problem is

$$
\min_{f\ge0}\sum_{ij}c_{ij}f_{ij},\qquad
\sum_jf_{ij}-\sum_jf_{ji}=b_i\quad\text{at every vertex }i.
$$

Positive $b_i$ is external supply and negative $b_i$ is demand; summing the [flow balances](../../../../../flow-balance.md) requires $\sum_i b_i=0$. There are no finite upper arc capacities. Let $B$ be the [oriented incidence matrix](../../../../../oriented-incidence-matrix.md) with tail $+1$ and head $-1$. For free dual potentials $\pi_i$, the [Lagrangian](../../../../../lagrangian.md) is

$$
\mathcal L(f,\pi)=c^Tf+\pi^T(b-Bf)
=\pi^Tb+\sum_{ij}(c_{ij}-\pi_i+\pi_j)f_{ij}.
$$

Its infimum over nonnegative flows is $\pi^Tb$ exactly when every [network reduced cost](../../../../../network-reduced-cost.md) $r_{ij}=c_{ij}-\pi_i+\pi_j$ is nonnegative; otherwise the infimum is minus infinity. Thus the dual maximizes $\pi^Tb$ subject to these inequalities. For a primal feasible flow and dual feasible potentials,

$$
c^Tf-\pi^Tb=\sum_{ij}r_{ij}f_{ij}\ge0.
$$

This derives [weak duality](../../../../../weak-duality.md) and the [complementary slackness](../../../../../complementary-slackness.md) condition $f_{ij}r_{ij}=0$. A feasible pair satisfying it has equal objectives and certifies optimality.

A [spanning tree](../../../../../spanning-tree.md) gives candidate [network dual potentials](../../../../../network-dual-potential.md) by making all its arcs tight: choose one root potential and propagate $\pi_j=\pi_i-c_{ij}$ along each tree arc, reversing this equation when traversing against the arc. An arbitrary tree does not automatically make the non-tree reduced costs nonnegative; those inequalities must be checked. If a guaranteed feasible construction is needed and there is no negative directed cycle, use [dual network potentials from shortest-path distances](../../../../../dual-network-potentials-from-shortest-path-distances.md): add an auxiliary source reaching every vertex, calculate distances $d_i$, and take $\pi_i=-d_i$. The shortest-path inequality $d_j\le d_i+c_{ij}$ proves [dual feasibility](../../../../../dual-feasibility.md), with tightness on the shortest-path tree.

For the printed dashed tree, set all non-tree flows to zero and solve the balances from the leaves. This gives

$$
\begin{array}{c|rrrrrrrr}
\text{tree arc}&14&43&37&79&15&56&62&68\\\hline
f_{ij}&2&2&2&2&1&1&1&0\\
c_{ij}&1&3&1&3&2&1&1&2
\end{array}
$$

The remaining arcs $46,67,52,28,89$ have zero flow. The total initial cost is $20$. This is a [basic feasible solution](../../../../../basic-feasible-solution.md), though degenerate because the tree flow on $68$ is zero.

Normalize $\pi_1=0$. Tree tightness gives

$$
(\pi_1,\ldots,\pi_9)=(0,-4,-4,-1,-2,-3,-5,-5,-8).
$$

The non-tree reduced costs are

$$
\begin{array}{c|rrrrr}
\text{arc}&46&67&52&28&89\\\hline
r_{ij}&2&0&2&1&-1.
\end{array}
$$

The negative reduced cost on $89$ identifies an improving entering arc for the [network simplex algorithm](../../../../../network-simplex-algorithm.md). Adding it to the tree creates a unique undirected cycle. Sending $\theta$ along $8\to9$ increases the flows on $15,56,68,89$ by $\theta$ and decreases those on $14,43,37,79$ by $\theta$; all other flows are unchanged. This balanced displacement preserves every node equation. Nonnegativity limits $\theta$ to the minimum of the four decreasing flows, namely $2$. Choose arc $14$ to leave among the tied limiting arcs.

After this one pivot the nonzero flows are

$$
\boxed{f_{15}=3,\quad f_{56}=3,\quad f_{62}=1,\quad f_{68}=2,\quad f_{89}=2,}
$$

and every other arc flow is zero. The objective decreases by $\theta r_{89}=-2$, giving cost $18$.

For the new tree, tight potentials normalized at vertex 1 are

$$
(\pi_1,\ldots,\pi_9)=(0,-4,-3,0,-2,-3,-4,-5,-7).
$$

All tree reduced costs are zero. For the non-tree arcs $14,46,67,52,28$ they are $1,1,1,2,1$, respectively, so the potentials are dual feasible. Their dual objective is

$$
\pi^Tb=3\pi_1-\pi_2-2\pi_9=18,
$$

matching the primal cost. [Complementary slackness](../../../../../complementary-slackness.md) therefore proves

$$
\boxed{\text{Minimum flow cost}=18.}
$$

This is the stopping test of the network simplex method: maintain a feasible tree flow, compute tight potentials, enter a negative-reduced-cost non-tree arc, make a maximal feasible cycle adjustment and exchange a limiting tree arc, until all reduced costs are nonnegative. Here exactly one improving step suffices.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
