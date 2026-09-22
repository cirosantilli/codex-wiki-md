# Fenwick tree

↑ **Parent:** [Data structure](data-structure-split.md)

A Fenwick tree stores a changing array so that a point update and a [prefix sum](prefix-sum.md) query each take $O(\log n)$ time with $O(n)$ storage. With indices starting at $1$, the entry at $i$ stores the sum over the final block of length $i\mathbin{\&}(-i)$ ending at $i$. A query repeatedly removes that final block, while an update visits the blocks containing the changed position.

## ↑ Ancestors (3)

1. [Data structure](data-structure-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)
