<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The ordered [Cartesian product](../../../../../cartesian-product.md) has **$n^4$ states**, including $n^2$ goal states. Each robot has at most five commands, so the [search tree](../../../../../search-tree.md) has **[branching factor](../../../../../branching-factor.md) at most $25$**, attained when both are interior for $n\ge3$. Boundary states have fewer actions under the legal-move convention. For $n=2$ the maximum is $3^2=9$, and for $n=1$ it is one if waiting is retained.

The [state space](../../../../../state-space.md) is finite, but the unrestricted [search tree](../../../../../search-tree.md) is infinite because both robots can wait repeatedly. $n^4$ counts physical states, not distinct action histories.

## ↑ Ancestors (11)

1. [B](../b.md)
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
