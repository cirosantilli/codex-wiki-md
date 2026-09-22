<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**TODO: the classifications, chosen [heuristic functions](../../../../../heuristic-function.md) and least-cost outcomes for G1–G5 cannot be established from the corrupted original Figure 1.** The missing [edges](../../../../../edge-of-a-graph.md), costs, priority labels and lower portions of the five [search trees](../../../../../search-tree.md) are required inputs. The surviving portions and the two [heuristic function](../../../../../heuristic-function.md) tables do not determine those answers. No reconstructed [graph](../../../../../graph-split.md) or invented expansion trace is assumed.

For a readable instance, [depth-first search](../../../../../depth-first-search.md) follows the deepest pending branch and [breadth-first search](../../../../../breadth-first-search.md) expands by [search depth](../../../../../search-depth.md); neither generally minimizes unequal [edge](../../../../../edge-of-a-graph.md) costs. [Uniform-cost search](../../../../../uniform-cost-search.md) orders by [path cost](../../../../../path-cost.md) $g$, whereas [A-star search](../../../../../a-star-search.md) orders by $g+h$. A displayed [A-star search](../../../../../a-star-search.md) score would identify the estimate by subtracting the accumulated [path cost](../../../../../path-cost.md). Under nonnegative costs and the usual terminating-search assumptions, [uniform-cost search](../../../../../uniform-cost-search.md) returns a least-cost [goal state](../../../../../goal-state.md) when testing goals on removal from the [search frontier](../../../../../search-frontier.md); [A-star search](../../../../../a-star-search.md) additionally needs an [admissible heuristic](../../../../../admissible-heuristic.md) with appropriate reopening, or a [consistent heuristic](../../../../../consistent-heuristic.md) for the usual closed-set implementation. These rules explain how the missing information would be used, but cannot identify a particular damaged [search tree](../../../../../search-tree.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
