<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Regard the rooms as the [vertices](../../../../../vertex-graph-theory.md) of a [grid graph](../../../../../grid-graph.md). Let $C=\{1,\ldots,n\}^2$ and let the two robot positions be $p,q\in C$. A single controller chooses both commands, so the [state space](../../../../../state-space.md) is the ordered [Cartesian product](../../../../../cartesian-product.md) $S=C\times C$, with initial state $(p_0,q_0)$. Distinguishing the robots matters because their later action laws need not be identical.

For a room $x$, let $A(x)$ consist of wait and all cardinal moves remaining in $C$; write $\delta(x,u)$ for the resulting room. At $(p,q)$ an action is the ordered pair $(u,v)\in A(p)\times A(q)$, and the deterministic [search transition model](../../../../../search-transition-model.md) is

$$
T((p,q),(u,v))=(\delta(p,u),\delta(q,v)).
$$

The [goal test](../../../../../goal-test.md) is **$p=q$**, checked at integer time boundaries, and every joint action costs one. Swapping two distinct rooms does not satisfy the [goal test](../../../../../goal-test.md). No internal walls are supplied; if walls were specified, they would simply restrict the move relation.

## ↑ Ancestors (11)

1. [A](../a.md)
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
