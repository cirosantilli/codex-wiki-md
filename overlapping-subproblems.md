# Overlapping subproblems

↑ **Parent:** [Memoization](memoization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Overlapping_subproblems)

[Overlapping subproblems](overlapping-subproblems.md) occur when several parts of a calculation request the same smaller problem. [Memoization](memoization.md) can share its answer if the [memoization key](memoization-key.md) identifies that problem completely. For the [Fibonacci numbers](fibonacci-number.md), both $F_5$ and $F_4$ require $F_3$. In [dynamic programming](dynamic-programming.md), the [dynamic programming state](dynamic-programming-state.md) plays the corresponding role of identifying a reusable continuation. Overlap explains potential savings; the [recurrence relation](recurrence-relation.md) and its base cases still need to be correct.

## ↑ Ancestors (4)

1. [Memoization](memoization.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Matrix-chain dynamic programming](matrix-chain-dynamic-programming.md)
- [Memoization](memoization.md)
- [Overlapping subproblems](overlapping-subproblems.md)
