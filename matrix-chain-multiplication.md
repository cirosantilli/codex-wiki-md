# Matrix-chain multiplication

↑ **Parent:** [Algorithm](algorithm-split.md)

Given a fixed [sequence](sequence.md) of compatible [matrices](matrix.md) $A_1,\ldots,A_m$, choose a binary parenthesization of $A_1\cdots A_m$ that minimizes the number of scalar multiplications in ordinary [matrix multiplication](matrix-multiplication.md). The order of the [matrices](matrix.md) is fixed: parenthesization changes the grouping, not the operand order. [Associativity](associative-property.md) preserves the product while intermediate [matrix](matrix.md) dimensions change the cost. The possible binary groupings are counted by the [Catalan number](catalan-number.md) $C_{m-1}$ for $m\geq1$.

**Table of contents**

- [Matrix-chain cost model](matrix-chain-cost-model.md)
- [Matrix-chain dynamic programming](matrix-chain-dynamic-programming.md)
- [Matrix-chain split reconstruction](matrix-chain-split-reconstruction.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Binary parenthesization](binary-parenthesization.md)
