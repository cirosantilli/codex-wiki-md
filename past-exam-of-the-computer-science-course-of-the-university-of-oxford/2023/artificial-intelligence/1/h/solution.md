<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

**[Breadth-first tree search](../../../../../breadth-first-tree-search.md) is complete and is still not bonus-optimal.** Fix any deterministic rule for choosing among equally short fox routes; the completeness argument again uses only the finite [branching factor](../../../../../branching-factor.md). The unobstructed corridor of part (g) has unique [shortest paths](../../../../../shortest-path.md), so its fox moves are exactly the same under the new strategy. The one-round bonus is $1$ and the two-round bonus is $2$, proving nonoptimality without any tie-breaking ambiguity.

If there is no route between fox and rabbit, the printed shortest-path rule needs a convention; letting the fox stay supplies a natural extension. The completeness argument is unchanged, and the counterexample above uses only connected squares. When the fox and rabbit initially belong to the same [connected component of a graph](../../../../../component-graph-theory.md), the [shortest-path pursuit distance bound](../../../../../shortest-path-pursuit-distance-bound.md) also makes every surviving branch finite. That additional property does not make the first escape maximize its bonus.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
