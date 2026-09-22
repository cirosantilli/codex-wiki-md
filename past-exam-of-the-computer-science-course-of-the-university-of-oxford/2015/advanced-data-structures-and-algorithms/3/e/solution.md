<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $G=(L\cup R,E)$ be the given [bipartite graph](../../../../../bipartite-graph-split.md). A [matching in a graph](../../../../../matching-graph-theory-split.md) selects [edges](../../../../../edge-of-a-graph.md) with no shared endpoint. For each [edge](../../../../../edge-of-a-graph.md) $e$, introduce an indicator $x_e$ for selection. The [integer program](../../../../../integer-programming.md) for a [maximum cardinality matching](../../../../../maximum-cardinality-matching.md) is

$$
\boxed{
\begin{aligned}
\max\quad&\sum_{e\in E}x_e\\
\text{subject to}\quad&\sum_{e\ni v}x_e\leq1&& (v\in L\cup R),\\
&x_e\in\{0,1\}&& (e\in E).
\end{aligned}}
$$

Its [linear programming relaxation](../../../../../linear-programming-relaxation.md) is

$$
P=\left\{x\in\mathbb R^E:x_e\geq0\ (e\in E),\quad\sum_{e\ni v}x_e\leq1\ (v\in L\cup R)\right\},
$$

with the same [objective function](../../../../../objective-function.md). Explicit upper bounds $x_e\leq1$ may be included, but they already follow from a constraint at either endpoint.

We prove that every [extreme point](../../../../../extreme-point.md) of $P$ is integral by showing that any [feasible point](../../../../../feasible-point.md) with a fractional coordinate admits a two-sided perturbation. Given such an $x$, form the [fractional support graph](../../../../../fractional-support-graph-of-a-matching-relaxation.md) $H$ with exactly those [edges](../../../../../edge-of-a-graph.md) for which $0<x_e<1$. This is a nonempty [bipartite graph](../../../../../bipartite-graph-split.md). A [vertex](../../../../../vertex-graph-theory.md) incident to one of these [edges](../../../../../edge-of-a-graph.md) cannot also meet an [edge](../../../../../edge-of-a-graph.md) with value $1$, because its incident sum would exceed $1$.

First suppose $H$ contains a [graph cycle](../../../../../cycle-in-a-graph.md). Choose a simple one, $e_1,\ldots,e_q$. Its length $q$ is even since $H$ is a [bipartite graph](../../../../../bipartite-graph-split.md). Define a nonzero [vector](../../../../../vector.md) $h$ by alternating $+1,-1$ along the [graph cycle](../../../../../cycle-in-a-graph.md) and putting $0$ on other [edges](../../../../../edge-of-a-graph.md). At each [vertex](../../../../../vertex-graph-theory.md) on the [graph cycle](../../../../../cycle-in-a-graph.md), the two changed coordinates have opposite signs, so its incident sum is unchanged. Choose

$$
0<\varepsilon<\min_{e\text{ on the cycle}}\{x_e,1-x_e\}.
$$

Then $x^+=x+\varepsilon h$ and $x^-=x-\varepsilon h$ are distinct [feasible points](../../../../../feasible-point.md): no coordinate leaves $[0,1]$ and all incident sums are unchanged. Since $x=(x^++x^-)/2$, it is not an [extreme point](../../../../../extreme-point.md).

Otherwise $H$ is a [forest](../../../../../forest.md). Choose a [connected component of a graph](../../../../../component-graph-theory.md) containing an [edge](../../../../../edge-of-a-graph.md), and a simple [graph path](../../../../../path-in-a-graph.md) in it between two [tree leaves](../../../../../leaf-of-a-tree.md). Alternate $+1,-1$ along the [graph path](../../../../../path-in-a-graph.md) to define $h$. Every internal [vertex](../../../../../vertex-graph-theory.md) of the [graph path](../../../../../path-in-a-graph.md) still has unchanged incident sum, including any additional [edges](../../../../../edge-of-a-graph.md) branching from it. At either endpoint, exactly one incident [edge](../../../../../edge-of-a-graph.md) has fractional value; all other incident coordinates are $0$, since a coordinate $1$ is impossible there. Thus each endpoint has strictly positive slack $1-\sum_{e\ni v}x_e$ in its degree constraint. Choose $\varepsilon>0$ smaller than these two slacks and smaller than every $x_e$ and $1-x_e$ along the [graph path](../../../../../path-in-a-graph.md). Both $x+\varepsilon h$ and $x-\varepsilon h$ remain feasible: the endpoint sums can increase or decrease by $\varepsilon$, and the internal sums do not change. Again $x$ is the midpoint of distinct [feasible points](../../../../../feasible-point.md), contradicting extremality.

Both cases exclude fractional coordinates at an [extreme point](../../../../../extreme-point.md). Therefore

$$
\boxed{\text{every extreme point of }P\text{ has }x_e\in\{0,1\}\text{ and represents a matching}.}
$$

The nonempty bounded [linear polyhedron](../../../../../linear-polyhedron.md) $P$ has an optimal [extreme point](../../../../../extreme-point.md) for the stated [linear function](../../../../../linear-function.md), so the relaxation yields a [maximum cardinality matching](../../../../../maximum-cardinality-matching.md). This is stronger than the existence of one integral optimum: it proves integrality of every [extreme point](../../../../../extreme-point.md). It does not claim that every optimal [feasible point](../../../../../feasible-point.md) is integral; convex mixtures of distinct optimal [matchings in a graph](../../../../../matching-graph-theory-split.md) can be fractional.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
