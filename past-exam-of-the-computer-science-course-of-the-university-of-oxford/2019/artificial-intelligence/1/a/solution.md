<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The first assertion is false.** Give the root a first child that is a [goal state](../../../../../goal-state.md) of cost ten and another child leading to many cheaper non-goal [search nodes](../../../../../search-node.md). [Depth-first search](../../../../../depth-first-search.md) can take the first child and stop immediately. [A-star search](../../../../../a-star-search.md) with the [admissible heuristic](../../../../../admissible-heuristic.md) $h=0$ behaves as [uniform-cost search](../../../../../uniform-cost-search.md) and expands the cheaper non-goal [search nodes](../../../../../search-node.md) before selecting that goal. Thus an [admissible heuristic](../../../../../admissible-heuristic.md) does not make [A-star search](../../../../../a-star-search.md) expand fewer nodes than every possible [depth-first search](../../../../../depth-first-search.md) ordering. The latter need not return an optimal solution.

**The second assertion is true under the usual finite-[branching factor](../../../../../branching-factor.md) assumption.** [Breadth-first search](../../../../../breadth-first-search.md) orders by [search depth](../../../../../search-depth.md), not [path cost](../../../../../path-cost.md). Every finite depth contains finitely many [search nodes](../../../../../search-node.md), so a goal at finite depth is eventually reached even if some steps cost zero. Zero-cost steps can affect cost optimality, but do not obstruct this completeness argument. An infinite [branching factor](../../../../../branching-factor.md) would invalidate the argument irrespective of [step costs](../../../../../step-cost.md).

**The third assertion is true as a worst-case black-box requirement, with a finite optimum assumed.** If outgoing actions are known only by expanding a state, an unexamined reachable branch can conceal a sufficiently negative-cost action followed by a route to a goal. Its total cost can beat the current solution by an arbitrarily large amount. Without additional lower bounds or structural information, finding one cheap solution cannot justify stopping; exhaustive examination can be necessary. This does not assert that every already-described irrelevant state must be visited on every input. Moreover, a reachable negative-cost [cycle in a graph](../../../../../cycle-in-a-graph.md) that can still reach a goal can make costs unbounded below, in which case no finite-cost optimal solution exists at all.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
