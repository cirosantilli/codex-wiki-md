<h1 id="3k/solution">Solution</h1>

↑ **Parent:** [3K](../3k.md)

For a binary [prefix code](../../../../../prefix-code.md) with word lengths $l_1,\ldots,l_m$, choose $L\geq\max l_i$. Each codeword is the prefix of exactly $2^{L-l_i}$ words of length $L$, and these descendant sets are disjoint. Hence

$$
\sum_i2^{L-l_i}\leq2^L,\qquad\text{so}\qquad\sum_i2^{-l_i}\leq1.
$$

This is [Kraft inequality](../../../../../kraft-mcmillan-inequality.md). Conversely, if integer lengths satisfy this inequality, place words greedily as leaves of the binary tree; the unused capacity ensures that the requested leaves can all be chosen, giving a prefix code.

For Shannon--Fano coding, order symbols by probability and assign

$$
l_i=\lceil-\log_2p_i\rceil.
$$

Kraft's inequality applies because $2^{-l_i}\leq p_i$ and therefore $\sum_i2^{-l_i}\leq1$. Thus codewords of those lengths exist. Since

$$
-\log_2p_i\leq l_i< -\log_2p_i+1,
$$

the expected length obeys

$$
H(X)\leq\mathbb E L<H(X)+1.
$$

## ↑ Ancestors (10)

1. [3K](../3k.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
