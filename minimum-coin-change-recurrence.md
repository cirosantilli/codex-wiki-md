# Minimum coin change recurrence

↑ **Parent:** [Coin change problem](coin-change-problem.md)

For positive [integer](integer-split.md) denominations, the [coin change problem](coin-change-problem.md) asks for coins summing to a target amount $v$; this recurrence minimizes their number. With unlimited supply, use the recurrence in the title, $M[0]=0$, and $\infty$ for an unreachable amount. Classifying a solution by its last coin proves the recurrence by [induction](mathematical-induction.md). Recording that coin reconstructs an optimum. The table uses $O(nv)$ [running time](running-time.md) and $O(v)$ [space complexity](space-complexity.md); this is a [pseudopolynomial time](pseudopolynomial-time.md) bound.

If each available coin can be used only once, update $M[t]\gets\min(M[t],1+M[t-x_i])$ for amounts in descending order for each coin. Descending order retains the previous row's value at $t-x_i$ and prevents reuse. Ascending order instead permits repeated use of the current coin. The distinction is a dependency invariant, not a cosmetic loop-order choice.

## ↑ Ancestors (6)

1. [Coin change problem](coin-change-problem.md)
2. [Dynamic programming](dynamic-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Dynamic programming recurrence](dynamic-programming-recurrence.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/6/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/7/b/i/solution.md)
