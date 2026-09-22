<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Label the balls $a,b,c,d$ and buckets $1,2,3$. Ignoring unchanged static type facts, the initial state's true [planning fluents](../../../../../planning-fluent.md) are

$$
S_0=\{\operatorname{In}(a,1),\operatorname{In}(b,1),\operatorname{In}(c,2),\operatorname{Holding}(d),\operatorname{At}(1)\}.
$$

**Expanding it produces exactly three successors.** The held ball makes $\operatorname{Empty}$ false, so neither ball in bucket $1$ can be picked up yet.

For $\operatorname{Drop}(d,1)$, replace $\operatorname{Holding}(d)$ by $\operatorname{In}(d,1)$ and $\operatorname{Empty}$; the arm stays at bucket $1$. All four balls are then in buckets, with $a,b,d$ in $1$ and $c$ in $2$.

For $\operatorname{Move}(1,2)$, replace $\operatorname{At}(1)$ by $\operatorname{At}(2)$ and leave every ball [planning fluent](../../../../../planning-fluent.md) unchanged, including $\operatorname{Holding}(d)$.

For $\operatorname{Move}(1,3)$, similarly replace only the arm-location [planning fluent](../../../../../planning-fluent.md) by $\operatorname{At}(3)$. The arm is now over the destination while still holding $d$; it has not yet dropped that ball.

No other action is applicable: the other drop locations fail their arm-location [precondition](../../../../../precondition.md), no pick has an empty hand, and moves from another source bucket fail their source-location [precondition](../../../../../precondition.md). None of these three successors satisfies $\bigwedge_{z\in\{a,b,c,d\}}\operatorname{In}(z,3)$. This describes one [forward state-space planning](../../../../../forward-state-space-planning.md) expansion, not an assertion that the search has already found a complete [plan](../../../../../plan.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
