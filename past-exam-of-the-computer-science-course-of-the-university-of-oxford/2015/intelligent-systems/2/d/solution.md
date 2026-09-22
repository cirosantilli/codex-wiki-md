<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In terms of minimum [plan](../../../../../plan.md) length, allowing more stacks can only help:

$$
\boxed{L^*(n,k+1)\le L^*(n,k).}
$$

Every legal [plan](../../../../../plan.md) using at most $k$ stacks remains legal with $k+1$ available: simply ignore the new stack. The inequality need not be strict. For $n=1$, one move suffices for every $k\ge2$.

With $k\ge n+1$, put each of the $n-1$ smaller coins on its own spare stack, move the largest coin to the destination, and then place the smaller coins on it in decreasing size order. This uses $2n-1$ moves. Every smaller coin must leave the initial stack before the largest coin's first move. It cannot move just once directly to the final stack and stay there, since that would block the largest coin's eventual arrival. Thus each smaller coin requires at least two moves, while the largest coin requires at least one. Hence

$$
L^*(n,k)=2n-1\qquad(k\ge n+1).
$$

Compared with the three-stack value $2^n-1$, the physical task can therefore become substantially easier.

The difficulty of _finding_ an optimal [plan](../../../../../plan.md) is a different issue. Each legal state is determined by assigning every coin to one of the $k$ labelled stacks, whose size order is then forced. There are $k^n$ such assignments, so the [state space](../../../../../state-space.md) and possible [branching factor](../../../../../branching-factor.md) grow with $k$. An uninformed [search algorithm](../../../../../search-algorithm.md) can therefore face more alternatives even when the optimal [plan](../../../../../plan.md) becomes shorter. Likewise, a simple recursive strategy for three stacks need not immediately supply the best strategy with more stacks. The defensible answer is that the required number of moves never increases, while computational search effort need not decrease.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
