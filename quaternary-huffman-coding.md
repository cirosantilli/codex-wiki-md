# Quaternary Huffman coding

↑ **Parent:** [Huffman coding](huffman-coding.md)

[Huffman coding](huffman-coding.md) with a four-symbol output [alphabet](alphabet.md), minimizing [expected codeword length](expected-codeword-length.md) among quaternary [prefix codes](prefix-code.md). Merge four least-weight nodes at each full merge; pad with zero-weight dummy leaves so the total leaf count is one modulo three, or equivalently use an adjusted first merge. The [Huffman sibling property](huffman-sibling-property.md) and contraction argument extend to four children, proving optimality. Removing dummy [codewords](codeword.md) preserves the [prefix code](prefix-code.md) property and costs nothing in [expectation](expected-value-split.md).

## ↑ Ancestors (6)

1. [Huffman coding](huffman-coding.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Binary translation of a quaternary prefix code](binary-translation-of-a-quaternary-prefix-code.md)
