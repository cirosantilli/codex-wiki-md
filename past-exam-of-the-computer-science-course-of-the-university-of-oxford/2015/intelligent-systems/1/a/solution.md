<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V$ be the [set](../../../../../set-split.md) of [Boolean variables](../../../../../boolean-variable.md) occurring in $T$ or the initial query $Q$, and put $N=|V|$. Represent a current query by a [subset](../../../../../subset.md) $R\subseteq\{\neg p:p\in V\}$: the [Boolean literals](../../../../../boolean-literal.md) in this [set](../../../../../set-split.md) are the outstanding obligations. The initial state is $R=Q$, and the [goal test](../../../../../goal-test.md) is $R=\varnothing$.

An action chooses a [Horn clause](../../../../../horn-clause.md) $C\in T$ with positive [Boolean literal](../../../../../boolean-literal.md) $p$, provided $\neg p\in R$. Its [search transition model](../../../../../search-transition-model.md) is precisely the given [resolution inference rule](../../../../../resolution-inference-rule.md):

$$
R\longmapsto R'=(C\cup R)\setminus\{p,\neg p\}.
$$

Thus it removes the obligation $\neg p$ and inserts all negative [Boolean literals](../../../../../boolean-literal.md) of $C$. Repeated [Boolean literals](../../../../../boolean-literal.md) merge because queries are [sets](../../../../../set-split.md). A [Horn clause](../../../../../horn-clause.md) without a positive [Boolean literal](../../../../../boolean-literal.md) supplies no action under the rule specified in this paper; it must not be treated as an additional way of finishing the query.

Give every action unit cost. A [graph path](../../../../../path-in-a-graph.md) with $\ell$ actions gives a proof containing $\ell+1$ queries, so minimizing either quantity gives the same shortest proof. [Uniform-cost search](../../../../../uniform-cost-search.md) orders the [search frontier](../../../../../search-frontier.md) by the number of actions already taken and applies the [goal test](../../../../../goal-test.md) when removing a [search node](../../../../../search-node.md) for expansion. Recording parent actions reconstructs the proof.

There are at most two choices, present or absent, for each of the $N$ negative [Boolean literals](../../../../../boolean-literal.md). Therefore

$$
\boxed{c(R,C,R')=1,\qquad |\mathcal S|\le 2^N.}
$$

This bounds the [state space](../../../../../state-space.md), including the empty query, rather than the possibly infinite [search tree](../../../../../search-tree.md) of action histories.[Printed p. 2, corrected Question 1, definitions and part (a)](../../../../../intelligent-systems-examination-paper-by-the-university-of-oxford-2015.md)

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
