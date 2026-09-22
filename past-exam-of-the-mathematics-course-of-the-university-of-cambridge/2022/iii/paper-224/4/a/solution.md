<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The binary [Kraft inequality](../../../../../../kraft-mcmillan-inequality.md) says that codeword lengths $l_1,l_2,\ldots$ of a [prefix code](../../../../../../prefix-code.md) satisfy

$$
\sum_i2^{-l_i}\leq1.
$$

Conversely, suppose positive integer lengths obey this inequality and arrange them in nondecreasing order. Construct codewords greedily in the infinite binary tree. Before assigning length $l_i$, each earlier codeword of length $l_j\leq l_i$ excludes exactly $2^{l_i-l_j}$ nodes at depth $l_i$. Thus the number excluded is

$$
\sum_{j<i}2^{l_i-l_j}
=2^{l_i}\sum_{j<i}2^{-l_j}
<2^{l_i},
$$

where strictness follows because the remaining term $2^{-l_i}$ occurs in the full Kraft sum. A free depth-$l_i$ node therefore exists. Assign it as the next codeword; choosing a node not below an earlier codeword preserves prefix-freeness. Induction constructs the required prefix code.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
