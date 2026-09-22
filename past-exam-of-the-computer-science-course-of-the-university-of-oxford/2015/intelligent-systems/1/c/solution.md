<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Termination is not guaranteed.** Take

$$
Q=\{\neg p\},\qquad T=\bigl\{\{p,\neg q\},\{q,\neg p\}\bigr\}.
$$

Both members of $T$ are valid [Horn clauses](../../../../../horn-clause.md) with distinct underlying [Boolean variables](../../../../../boolean-variable.md). The only possible continuation alternates

$$
\{\neg p\}\longmapsto\{\neg q\}\longmapsto\{\neg p\}\longmapsto\cdots.
$$

The empty query is unreachable. With the [admissible heuristic](../../../../../admissible-heuristic.md) $h=0$, ordinary [A-star search](../../../../../a-star-search.md) keeps generating the next [search node](../../../../../search-node.md) forever, despite there being only two reachable states.

A modification requiring no additional stored state collection is to impose the known [search depth](../../../../../search-depth.md) bound

$$
\boxed{L=2^N-1,\qquad\text{do not expand a non-goal node with }g=L.}
$$

The unit-cost $g$ already stored by [A-star search](../../../../../a-star-search.md) is also its [search depth](../../../../../search-depth.md); the bound is a scalar computed from the input, not a closed [set](../../../../../set-split.md). Apply the [goal test](../../../../../goal-test.md) before refusing expansion at the bound.

To prove completeness of this modification, remove any segment between two equal states in a successful proof. The successor choices after the later occurrence are available at the earlier occurrence because the [search transition model](../../../../../search-transition-model.md) depends only on the current query. Repeating this removal gives a proof with no repeated states, hence at most $2^N-1$ actions. In particular, a shortest proof never needs a repeated state, since every removed segment has positive cost. The depth restriction therefore preserves a shortest proof whenever one exists.

The restricted [search tree](../../../../../search-tree.md) has finite depth and finite [branching factor](../../../../../branching-factor.md), so it is finite. [A-star search](../../../../../a-star-search.md) must then either remove a goal or exhaust the [search frontier](../../../../../search-frontier.md) and report failure. Its existing [search frontier](../../../../../search-frontier.md) may still be large; the modification saves a separate visited-state collection, not all storage used by [tree search](../../../../../tree-search.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
