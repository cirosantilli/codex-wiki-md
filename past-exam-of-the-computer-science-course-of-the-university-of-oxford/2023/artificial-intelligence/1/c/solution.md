<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [branching factor](../../../../../branching-factor.md) of the [search tree](../../../../../search-tree.md) is at most five, so through depth $d$ it has at most

$$
1+5+\cdots+5^d=\frac{5^{d+1}-1}{4}=O(5^d)
$$

nodes in [Big O notation](../../../../../big-o-notation.md). With no depth bound, **the [search tree](../../../../../search-tree.md) can be infinite**, despite the finite [state space](../../../../../state-space.md): [tree search](../../../../../tree-search.md) retains different action histories even when they end at the same position pair.

For a concrete repeating history, use a two-row, three-column board, indexed from zero, with the sole obstacle $(0,1)$, rabbit at $(0,2)$ and fox at $(0,0)$. Repeated rabbit stays leave the fox blocked horizontally with no vertical separation to reduce. Hence the same live state can repeat forever. An exit at $(1,2)$ is nevertheless safely reachable in one round.

## ↑ Ancestors (11)

1. [C](../c.md)
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
