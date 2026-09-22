# Deflate Huffman coding

↑ **Parent:** [Deflate](deflate.md)

For a compressed block, [Deflate Huffman coding](deflate-huffman-coding.md) uses one [alphabet](alphabet.md) for [Deflate literal bytes](deflate-literal-byte.md), length symbols and the end-of-block symbol, and another [alphabet](alphabet.md) for distance symbols. Values 0 through 255 denote [Deflate literal bytes](deflate-literal-byte.md), 256 ends the block, and 257 through 285 select lengths. A [Deflate backreference](deflate-backreference.md) is encoded as a length symbol, any length extra [bits](bit.md), a distance symbol, then any distance extra [bits](bit.md). Those extra [bits](bit.md) select an offset within the symbol's prescribed range; they are not additional [codewords](codeword.md).[RFC 1951, section 3.2.5, length and distance tables](deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch.md)

In the illustrative $(9,3)$ [Deflate backreference](deflate-backreference.md), length 9 uses symbol 263 and distance 3 uses symbol 2; neither needs extra [bits](bit.md). Under the fixed [Huffman codes](huffman-code.md), `A`, `B` and `C` each cost eight [bits](bit.md), symbol 263 costs seven, and distance symbol 2 costs five. Adding the seven-[bit](bit.md) end-of-block symbol and three-[bit](bit.md) block header gives $3+3\cdot8+7+5+7=46$ [bits](bit.md), packed into six [bytes](byte.md) for a single final block. This is a cost calculation for the explicitly chosen instructions, not a displayed compressed stream.[RFC 1951, sections 3.2.5 and 3.2.6: length 9, distance 3 and fixed code lengths](deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch.md)

Dynamic blocks transmit [codeword lengths](codeword-length.md) from which the decoder reconstructs the prescribed [prefix codes](prefix-code.md). The code descriptions themselves use a smaller [Huffman code](huffman-code.md) and repeat instructions for successive [codeword lengths](codeword-length.md), including runs of zero lengths. Here [run-length encoding](run-length-encoding.md) describes repeated code lengths, a separate role from copying repeated data [bytes](byte.md). Fixed blocks use predefined [Huffman codes](huffman-code.md) and avoid transmitting those descriptions.[RFC 1951, sections 3.2.2, 3.2.6 and 3.2.7: code reconstruction, fixed codes and dynamic code-length repeats](deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch.md)

## ↑ Ancestors (4)

1. [Deflate](deflate.md)
2. [Data compression](data-compression.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Deflate](deflate.md)
- [Deflate compression overhead](deflate-compression-overhead.md)
- [Deflate Huffman coding](deflate-huffman-coding.md)
- [Deflate literal byte](deflate-literal-byte.md)
