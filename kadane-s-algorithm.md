<h1 id="kadane-s-algorithm">Kadane's algorithm</h1>

↑ **Parent:** [Maximum subarray problem](maximum-subarray-problem.md)

For input $a_1,\ldots,a_n$, let $E_i$ be the largest sum of a nonempty contiguous block ending at $i$. The [recurrence relation](recurrence-relation.md) $E_1=a_1$ and $E_i=\max(a_i,E_{i-1}+a_i)$ is exact: an optimal block either starts at $i$ or extends an optimal block ending at $i-1$. The answer is $\max_i E_i$. Keeping only the current $E_i$ and best value gives linear [time complexity](time-complexity.md) and constant extra [space complexity](space-complexity.md).

## ↑ Ancestors (4)

1. [Maximum subarray problem](maximum-subarray-problem.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Maximum subarray problem](maximum-subarray-problem.md)
