<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Use $H=\max(h_1,h_2)$** if each estimate is available at comparable cost. For every $\alpha\in[0,1]$,

$$
\min(h_1,h_2)\le\alpha h_1+(1-\alpha)h_2\le H\le h^*.
$$

Thus $H$ has [heuristic dominance](../../../../../heuristic-dominance.md) over all the other combinations guaranteed to remain [admissible heuristics](../../../../../admissible-heuristic.md). [A-star search](../../../../../a-star-search.md) orders nodes by $f=g+h$, where $g$ is the accumulated path cost. A larger [admissible heuristic](../../../../../admissible-heuristic.md) excludes more nodes from the compulsory $f<C^*$ region, where $C^*$ is the optimal solution cost. Under the usual nonnegative-cost and goal-normalization assumptions, this gives at least as informative a search guide while preserving the optimality guarantee of [A-star search](../../../../../a-star-search.md) with [tree search](../../../../../tree-search.md).

The unweighted sum loses that guarantee. The dominance statement does not promise smaller wall-clock time in every implementation: evaluating estimates costs time, and nodes with $f=C^*$ depend on tie handling. Nor does admissibility of the inputs alone imply [consistent heuristics](../../../../../consistent-heuristic.md). If both inputs are [consistent heuristics](../../../../../consistent-heuristic.md), however, their pointwise maximum is also a [consistent heuristic](../../../../../consistent-heuristic.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
