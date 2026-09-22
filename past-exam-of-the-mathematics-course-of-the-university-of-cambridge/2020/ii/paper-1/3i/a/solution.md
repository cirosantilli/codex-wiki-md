<h1 id="3i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [Shannon-Fano coding](../../../../../../shannon-fano-coding.md), a symbol of probability $p_i$ is assigned length

$$
\ell_i=\left\lceil-\log_2p_i\right\rceil,
$$

and codewords of those lengths are chosen in lexicographic probability intervals; the [Kraft inequality](../../../../../../kraft-mcmillan-inequality.md) guarantees that a binary [prefix code](../../../../../../prefix-code.md) exists. [Huffman coding](../../../../../../huffman-coding.md) repeatedly merges the two least probable current symbols, builds a binary tree from the resulting merges, and labels its two branches by zero and one. Reading from the root to each leaf gives an optimal prefix code.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3I](../../3i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
