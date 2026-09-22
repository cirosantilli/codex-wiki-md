<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

The binary [Huffman coding](../../../../../huffman-coding.md) algorithm repeatedly merges the two currently least probable symbols into one meta-symbol whose probability is their sum. After recursively constructing a code for the smaller alphabet, append $0$ and $1$ to the meta-symbol's codeword to obtain codewords for the merged pair. The result is a binary [prefix code](../../../../../prefix-code.md).

To prove optimality, begin with an optimal prefix-code tree. It may be taken to be full, since an internal vertex with one child can be suppressed and all codewords below it shortened. Two leaves of maximum depth are siblings. By exchanging labels, without changing lengths, assign two least probable symbols to such a sibling pair: moving a smaller probability to a no-shorter codeword cannot increase the expected length. Contracting this pair to one leaf replaces their contribution $p_i\ell_i+p_j\ell_j$ by $(p_i+p_j)(\ell_i-1)$ plus the constant $p_i+p_j$. If the contracted code were not optimal for the reduced alphabet, replacing it by a better one and then expanding the merged leaf would improve the original code. [Mathematical induction](../../../../../mathematical-induction.md) on the number of symbols now proves that the Huffman construction minimizes expected word length.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
