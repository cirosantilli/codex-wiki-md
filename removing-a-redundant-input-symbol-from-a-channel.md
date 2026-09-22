# Removing a redundant input symbol from a channel

↑ **Parent:** [Channel capacity](channel-capacity.md)

Suppose one row of a finite [discrete memoryless channel](discrete-memoryless-channel.md) is a [convex combination](convex-combination.md) of other rows: $W(\cdot\mid x_0)=\sum_j\alpha_jW(\cdot\mid x_j)$. Deleting input $x_0$ leaves the [channel capacity](channel-capacity.md) unchanged. Given any input law with mass $t$ on $x_0$, move that mass to the other symbols in proportions $\alpha_j$. The output law stays the same. By the [concavity of information entropy](concavity-of-information-entropy.md), $H(W(\cdot\mid x_0))\geq\sum_j\alpha_jH(W(\cdot\mid x_j))$, so this replacement cannot increase [conditional entropy](conditional-entropy.md) $H(Y\mid X)$ and cannot decrease [mutual information](mutual-information.md). Taking maxima proves the claim; the smaller channel is also trivially a restriction of the original one. If the entropy inequality is strict, every positive use of the redundant row is strictly suboptimal compared with its redistribution.

## ↑ Ancestors (6)

1. [Channel capacity](channel-capacity.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2010/3/c/iii/solution.md)
