<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [vertex cover decision problem](../../../../../vertex-cover-decision-problem.md) takes a finite [simple graph](../../../../../simple-graph.md) $G$ and a [nonnegative integer](../../../../../natural-number.md) $k$, and asks whether there is a [vertex cover](../../../../../vertex-cover.md) of [cardinality](../../../../../cardinality.md) at most $k$. The optimization problem asks for a [minimum vertex cover](../../../../../minimum-vertex-cover.md), with cost equal to its [cardinality](../../../../../cardinality.md).

For the decision problem, if there are no [edges](../../../../../edge-of-a-graph.md), accept; if there is an [edge](../../../../../edge-of-a-graph.md) but $k=0$, reject. Otherwise choose an [edge](../../../../../edge-of-a-graph.md) $uv$ and branch: either include $u$ and recurse on $G-u$ with budget $k-1$, or include $v$ and recurse on $G-v$ with budget $k-1$. Accept if either branch accepts. Every [vertex cover](../../../../../vertex-cover.md) contains at least one endpoint of $uv$, so every possible solution is retained by at least one branch. Conversely, adding the selected endpoint to a [vertex cover](../../../../../vertex-cover.md) returned by the smaller instance covers all original [edges](../../../../../edge-of-a-graph.md). This proves correctness by [induction](../../../../../mathematical-induction.md) on the remaining budget.

The [search tree](../../../../../search-tree.md) has depth at most $k$ and at most $2^k$ leaves. Processing each node in $O(|V|+|E|)$ time gives **$O(2^k(|V|+|E|))$ [running time](../../../../../running-time.md)**, establishing [fixed-parameter tractability](../../../../../fixed-parameter-tractability.md).

For optimization, greedily build a [maximal matching](../../../../../maximal-matching.md) $M$: repeatedly select an [edge](../../../../../edge-of-a-graph.md) and discard every [edge](../../../../../edge-of-a-graph.md) touching either endpoint. Return the [set](../../../../../set-split.md) $C$ of all endpoints of $M$. Any [edge](../../../../../edge-of-a-graph.md) with neither endpoint in $C$ could be added to $M$, contradicting maximality; thus $C$ is a [vertex cover](../../../../../vertex-cover.md). Since the [edges](../../../../../edge-of-a-graph.md) of a [matching in a graph](../../../../../matching-graph-theory-split.md) have pairwise [disjoint](../../../../../disjoint-sets.md) endpoint [sets](../../../../../set-split.md), every [vertex cover](../../../../../vertex-cover.md) must contain at least one different [vertex](../../../../../vertex-graph-theory.md) for each of them. Therefore

$$
\boxed{|C|=2|M|\leq2\tau(G)=2\operatorname{OPT}.}
$$

The greedy construction takes [polynomial time](../../../../../polynomial-time.md), and can be implemented in $O(|V|+|E|)$ with [adjacency lists](../../../../../adjacency-list.md). It needs only a [maximal matching](../../../../../maximal-matching.md), not a [maximum matching](../../../../../maximum-cardinality-matching.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
