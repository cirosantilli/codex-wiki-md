<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

**[Breadth-first tree search](../../../../../breadth-first-tree-search.md) remains complete but is not optimal for maximizing the bonus.** Completeness depends on the finite [branching factor](../../../../../branching-factor.md) and a finite successful depth, not on the objective used to compare escapes.

Use the one-row, seven-square example from part (e). The one-round escape at column $3$ leaves the fox at column $2$, so its [graph distance](../../../../../distance-graph-theory.md) to the exit, and hence the bonus, is $1$. The two-round escape at column $6$ leaves the fox at column $4$, giving bonus $2$. The earliest successful node therefore has **bonus $1$ when bonus $2$ is achievable**. [Breadth-first tree search](../../../../../breadth-first-tree-search.md) orders by rounds rather than terminal [graph distance](../../../../../distance-graph-theory.md).

## ↑ Ancestors (11)

1. [G](../g.md)
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
