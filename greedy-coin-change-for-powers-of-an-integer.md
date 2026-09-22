# Greedy coin change for powers of an integer

↑ **Parent:** [Coin change problem](coin-change-problem.md)

For an [integer](integer-split.md) $p\geq2$ and $k\geq0$, unlimited denominations $1,p,\ldots,p^k$ admit optimal [greedy algorithm](greedy-algorithm.md). In a minimum-count solution, no smaller denomination can occur $p$ times: carrying those stamps to the next denomination reduces their count by $p-1$. Thus all counts below the maximum are base-$p$ digits, whose total value is at most $p^k-1$. The maximum-denomination count is forced to be the quotient on division by $p^k$, and repeating the argument forces every greedy remainder step.

## ↑ Ancestors (6)

1. [Coin change problem](coin-change-problem.md)
2. [Dynamic programming](dynamic-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms-resit/7/e/solution.md)
