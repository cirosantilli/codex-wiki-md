<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let item $j$ have weight $a_j$ and profit $p_j$. Define $D(j,b)$ as the largest profit obtainable from the first $j$ items with capacity at most the nonnegative [integer](../../../../integer-split.md) $b$. Set $D(0,b)=0$. The last item is either absent or present once, giving the [dynamic programming](../../../../dynamic-programming.md) recursion

$$
\boxed{D(j,b)=\begin{cases}
D(j-1,b),&b<a_j,\\
\max\{D(j-1,b),p_j+D(j-1,b-a_j)\},&b\geq a_j.
\end{cases}}
$$

The two alternatives exhaust the feasible binary decisions. In the second alternative, deleting item $j$ leaves exactly the smaller subproblem with capacity $b-a_j$, which proves the recurrence.

Fill rows $j=1,\ldots,4$, and within each row capacities $b=0,\ldots,7$. Store which alternative attains each maximum. Backtrack from $(4,7)$: when exclusion was chosen, set $x_j=0$ and move to $(j-1,b)$; when inclusion was chosen, set $x_j=1$ and move to $(j-1,b-a_j)$. Ties may be resolved either way. Thus the stored values yield an actual optimal selection, not just its objective value.

For $n$ items and capacity $B$, the [algorithm](../../../../algorithm-split.md) uses $O(nB)$ arithmetic operations and $O(nB)$ space with the full [backtracking](../../../../backtracking.md) table. It is a [pseudo-polynomial algorithm](../../../../pseudo-polynomial-time.md), since $B$ is a numerical capacity rather than its bit length. A value-only version can use one row, but must update capacities in decreasing order to avoid reusing the same item.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
