<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Maintain a certified solution-cost ceiling and prune only [search nodes](../../../../../search-node.md) whose lower bound strictly exceeds it.** Initially let $B=\infty$, or set $B=u(r)$ at the root $r$ when that value is finite. Whenever a [search node](../../../../../search-node.md) $n$ is generated, update

$$
B\leftarrow\min\{B,\ g(n)+u(n)\}.
$$

Run ordinary [A-star search](../../../../../a-star-search.md) with $f(n)=g(n)+h(n)$ and a [goal test](../../../../../goal-test.md) when removing a [search node](../../../../../search-node.md) from the [search frontier](../../../../../search-frontier.md). Discard a generated [search node](../../../../../search-node.md), or a queued [search node](../../../../../search-node.md) encountered after a later bound improvement, if

$$
\boxed{f(n)>B.}
$$

This is [branch and bound](../../../../../branch-and-bound.md) using a lower bound $f$ and an upper bound $B$. A finite $u(n)$ certifies that some goal is reachable from $n$ within that remaining-cost ceiling; for a dead end, $h^*(n)=\infty$ forces $u(n)=\infty$ too. Every finite quantity $g(n)+u(n)$ is consequently at least the global optimum $C^*$.

On an optimal solution path, [admissible heuristic](../../../../../admissible-heuristic.md) estimates ensure $f(n)\le C^*\le B$. Hence no [search node](../../../../../search-node.md) of that path is pruned. The finite-[branching factor](../../../../../branching-factor.md) and positive step-cost hypotheses from (a) still ensure completeness, and the usual [A-star search](../../../../../a-star-search.md) argument makes the first selected goal optimal. A smaller bound can remove branches earlier; it need not improve every instance.

The strict inequality matters: $u$ is only a numerical bound and need not provide an actual stored solution path. If $B=C^*$, pruning at $f(n)\ge B$ could remove every optimal continuation. Nor may the algorithm return a path merely because its lower bound meets $B$ when no witnessing path has been constructed. With an actual incumbent solution, the familiar equality-pruning variant can instead retain and return that incumbent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
