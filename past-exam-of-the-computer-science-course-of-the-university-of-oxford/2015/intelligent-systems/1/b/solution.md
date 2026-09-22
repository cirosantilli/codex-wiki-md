<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[A-star search](../../../../../a-star-search.md) is [best-first search](../../../../../best-first-search.md) with priority

$$
\boxed{f(u)=g(u)+h(s(u)),\qquad 0\le h(s)\le h^*(s),\qquad h(\text{goal})=0.}
$$

Here $u$ is a [search node](../../../../../search-node.md), $s(u)$ is its state, $g(u)$ is its accumulated [path cost](../../../../../path-cost.md), and $h^*(s)$ is the minimum remaining cost to any [goal state](../../../../../goal-state.md), interpreted as $\infty$ if no goal is reachable. The inequality defines an [admissible heuristic](../../../../../admissible-heuristic.md). Thus $f(u)$ is a lower bound on the cost of any solution extending that particular action history.

Initialize the [search frontier](../../../../../search-frontier.md) with the root. Repeatedly remove a [search node](../../../../../search-node.md) of least $f$, apply the [goal test](../../../../../goal-test.md), and, if it is not a goal, insert its applicable-action children with their updated $g$ and $f$. In [tree search](../../../../../tree-search.md), different action histories remain distinct [search nodes](../../../../../search-node.md) even when they reach the same state; there is no global visited-state [set](../../../../../set-split.md).

For the finite [branching factor](../../../../../branching-factor.md) and unit costs here, an [admissible heuristic](../../../../../admissible-heuristic.md) ensures that any first goal removed is optimal. If a cheaper solution existed, the [search frontier](../../../../../search-frontier.md) would contain an unexpanded prefix of it with $f$ at most that cheaper cost, contradicting selection of the more expensive goal. Nonnegative $h$ also means only finitely many [search nodes](../../../../../search-node.md) can have $f$ below any fixed finite cost, so a finite solution will eventually be reached. This does not guarantee termination when no proof exists.

## ↑ Ancestors (11)

1. [B](../b.md)
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
