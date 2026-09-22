# Matrix-chain cost model

↑ **Parent:** [Matrix-chain multiplication](matrix-chain-multiplication.md)

For [matrix dimensions](matrix-dimensions.md) $r\times s$ and $s\times t$, ordinary [matrix multiplication](matrix-multiplication.md) computes $rt$ [matrix entries](matrix-entry.md), each using $s$ [scalar multiplications](scalar-multiplication.md). Thus its cost is $rst$ [scalar multiplications](scalar-multiplication.md), with $rt(s-1)$ [additions](addition.md) if each sum starts from its first term. Here we minimize only the [scalar multiplication](scalar-multiplication.md) count, using this dense [matrix multiplication](matrix-multiplication.md) rule throughout. The counts describe [arithmetic operations](arithmetic-operation.md), rather than measured elapsed time; [matrix multiplication](matrix-multiplication.md) methods that exploit structure or use faster formulas require a different cost rule.

Take [matrices](matrix.md) $A$, $B$, $C$ with [matrix dimensions](matrix-dimensions.md) $12\times5$, $5\times40$, $40\times3$. Both groupings produce a $12\times3$ [matrix product](matrix-product.md), but their intermediate [matrix dimensions](matrix-dimensions.md) differ:

$$
\begin{aligned}
(AB)C &: \quad 12\cdot5\cdot40+12\cdot40\cdot3=2400+1440=3840,\\
A(BC) &: \quad 5\cdot40\cdot3+12\cdot5\cdot3=600+180=780.
\end{aligned}
$$

The second grouping first compresses $BC$ into a $5\times3$ [matrix](matrix.md), avoiding the $12\times40$ intermediate [matrix](matrix.md) $AB$. The saving is $3060$ [scalar multiplications](scalar-multiplication.md), although both groupings use exactly two [matrix multiplications](matrix-multiplication.md). This is why counting only [matrix multiplication](matrix-multiplication.md) operations hides the interesting choice.

<a id="image-the-same-matrix-product-can-require-3840-or-780-scalar-multiplications"></a>
![](matrix-chain-parenthesization-cost-trees.png)

**[Figure 1](#image-the-same-matrix-product-can-require-3840-or-780-scalar-multiplications). The same matrix product can require 3840 or 780 scalar multiplications**. Original [binary trees](binary-tree.md) for the three-[matrix](matrix.md) example. Leaves keep $A,B,C$ in the same order. Each internal node gives its resulting [matrix dimensions](matrix-dimensions.md) and the local [scalar multiplication](scalar-multiplication.md) cost; adding those costs gives the total.

[Associativity](associative-property.md) permits these regroupings in exact arithmetic; [commutativity](commutativity.md) is neither assumed nor generally true for [matrix multiplication](matrix-multiplication.md). Swapping $A$ and $B$ here would even make their [matrix product](matrix-product.md) undefined. In [floating-point arithmetic](floating-point-arithmetic-split.md), [round-off error](round-off-error.md) can make the two groupings yield different computed [matrix entries](matrix-entry.md); the cost optimum alone does not guarantee the smallest numerical error.

## ↑ Ancestors (4)

1. [Matrix-chain multiplication](matrix-chain-multiplication.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
