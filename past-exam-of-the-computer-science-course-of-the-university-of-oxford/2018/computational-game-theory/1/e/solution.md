<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $0<h<d$ and the feasible threshold $2\leq k\leq n$. An unsuccessful deer hunter would gain by switching to hare, so an equilibrium with deer participants must have $s\geq k$. A deer hunter then earns $d/s$ and must not gain by changing to hare; this requires $d/s\geq h$. A hare hunter who joins would earn $d/(s+1)$, so staying with hare requires $h\geq d/(s+1)$. Hence the necessary and sufficient conditions for the stated range $0<s<n$ are

$$
\boxed{k\leq s<n,\qquad \frac d{s+1}\leq h\leq\frac ds.}
$$

These conditions check every possible unilateral change in this two-action [game](../../../../../game.md), so they also prove sufficiency. Equality is allowed because a [Nash equilibrium](../../../../../nash-equilibrium.md) rules out strict improvements, not indifferent deviations. The endpoint $s=n$ has no hare hunter to check; it is an equilibrium exactly when $d/n\geq h$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
