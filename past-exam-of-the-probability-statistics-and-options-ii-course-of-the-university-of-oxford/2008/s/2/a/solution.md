<h1 id="s/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the fixed margins are compatible, so the finite state space is nonempty. At state $X$, draw an index table $Y$ from the stipulated uniform proposal law. If $X+Y$ has any negative entry, reject and stay at $X$; otherwise accept and set the next state to $X+Y$. The margins stay fixed because the proposal has zero row and column sums.

The proposal set is invariant under $Y\mapsto-Y$. Hence proposals between two feasible distinct states are symmetric. The target density is constant, so the Metropolis–Hastings acceptance probability for a feasible proposal is one. The explicit rejection of infeasible proposals is essential: fixed margins by themselves do not guarantee nonnegative entries.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [S](../../../s.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
