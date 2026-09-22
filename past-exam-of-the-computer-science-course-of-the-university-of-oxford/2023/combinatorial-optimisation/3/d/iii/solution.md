<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use [minimum-weight edge cover by matching savings](../../../../../../minimum-weight-edge-cover-by-matching-savings.md). Reject inputs with an [isolated vertex](../../../../../../isolated-vertex.md). For every [vertex](../../../../../../vertex-graph-theory.md) $v$, choose a cheapest incident [edge](../../../../../../edge-of-a-graph.md) $e_v$ and write $c_v=w(e_v)$. Define a baseline and a saving for each [edge](../../../../../../edge-of-a-graph.md) $uv$ by

$$
B=\sum_{v\in V}c_v,\qquad p(uv)=c_u+c_v-w(uv).
$$

Compute a [maximum-weight matching](../../../../../../maximum-weight-matching.md) $M$ using $p$ as its weights, allowing the empty [matching in a graph](../../../../../../matching-graph-theory-split.md) and imposing no maximum-[cardinality](../../../../../../cardinality.md) condition. Negative savings may be ignored. Return

$$
F_M=M\cup\{e_v:v\text{ is an unmatched vertex of }M\}.
$$

This is an [edge cover](../../../../../../edge-cover.md). Since original weights are nonnegative, removing duplicate appearances of an [edge](../../../../../../edge-of-a-graph.md) cannot increase the total, and hence

$$
w(F_M)\leq w(M)+\sum_{v\text{ unmatched}}c_v=B-\sum_{e\in M}p(e).
$$

To prove optimality, take a minimum-weight [edge cover](../../../../../../edge-cover.md) and remove redundant [edges](../../../../../../edge-of-a-graph.md) until it is inclusion-minimal. Nonnegative weights ensure that its weight does not increase, so it remains optimal. As proved in (i), its components are [star graphs](../../../../../../star-graph-theory.md). Choose one [edge](../../../../../../edge-of-a-graph.md) from each [star graph](../../../../../../star-graph-theory.md), forming a [matching in a graph](../../../../../../matching-graph-theory-split.md) $N$.

In a [star graph](../../../../../../star-graph-theory.md) with center $a$, selected leaf $b$, and other leaves $L$, this choice contributes $w(ab)+\sum_{v\in L}c_v$ to $B-p(N)$. Each other leaf $v$ has its [edge](../../../../../../edge-of-a-graph.md) $av$ available, so $c_v\leq w(av)$. Thus this contribution is at most the weight of that [star graph](../../../../../../star-graph-theory.md). Summing over components yields

$$
B-p(N)\leq\operatorname{OPT}.
$$

Since $M$ maximizes saving, $p(M)\geq p(N)$, and consequently

$$
\operatorname{OPT}\leq w(F_M)\leq B-p(M)\leq B-p(N)\leq\operatorname{OPT}.
$$

All inequalities are equalities. Therefore **$F_M$ is a minimum-weight [edge cover](../../../../../../edge-cover.md)**. This proof also handles zero weights and duplicate cheapest-[edge](../../../../../../edge-of-a-graph.md) choices.

Finding all $c_v$ and constructing $F_M$ takes $O(|V|+|E|)$ time. A general-[graph](../../../../../../graph-split.md) [maximum-weight matching](../../../../../../maximum-weight-matching.md) [polynomial-time algorithm](../../../../../../polynomial-time-algorithm.md) supplies the only substantial step; the documented routine runs in $O(|V|^3)$ arithmetic time. Exact rational or integer weights avoid floating-point comparisons affecting optimality.[max\_weight\_matching, maxcardinality=False; Notes: O(number\_of\_nodes \*\* 3), integer arithmetic for integer weights, and floating-point precision caveat](../../../../../../maximum-weight-matching-documentation-by-networkx.md)

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
