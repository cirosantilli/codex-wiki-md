# Binary translation of a quaternary prefix code

↑ **Parent:** [Prefix code](prefix-code.md)

Replacing every quaternary digit by its fixed two-[bit](bit.md) representation preserves the [prefix code](prefix-code.md) property: a binary prefix between translated [codewords](codeword.md) would end at an even position and hence imply a quaternary prefix. Thus a translated [quaternary Huffman code](quaternary-huffman-coding.md) cannot beat binary [Huffman coding](huffman-coding.md) in [expected codeword length](expected-codeword-length.md).

For the reverse bound, binary [prefix code](prefix-code.md) lengths $\ell_i$ give candidate quaternary lengths $k_i=\lceil\ell_i/2\rceil$. Since $\sum_i4^{-k_i}\leq\sum_i2^{-\ell_i}\leq1$, the [Kraft inequality](kraft-mcmillan-inequality.md) supplies such a quaternary [prefix code](prefix-code.md). Optimality of [quaternary Huffman coding](quaternary-huffman-coding.md) and $2\lceil\ell_i/2\rceil\leq\ell_i+1$ give $2L_4^*\leq L_2^*+1$. These quantities are [expected codeword lengths](expected-codeword-length.md) for the same source [probability distribution](probability-distribution-split.md).

## ↑ Ancestors (8)

1. [Prefix code](prefix-code.md)
2. [Decipherable code](decipherable-code.md)
3. [Unique decodability](unique-decodability.md)
4. [Coding theory](coding-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
