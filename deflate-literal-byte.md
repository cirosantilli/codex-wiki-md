# Deflate literal byte

↑ **Parent:** [Deflate](deflate.md)

A [Deflate literal byte](deflate-literal-byte.md) instructs the decoder to append one specified [byte](byte.md) directly to the [output](output-computing.md). For example, three [Deflate literal bytes](deflate-literal-byte.md) with values 65, 66 and 67 produce `ABC`. These values are symbols in the [Deflate Huffman coding](deflate-huffman-coding.md) stage, rather than necessarily eight raw stored [bits](bit.md) each. A [Deflate backreference](deflate-backreference.md) instead describes a copy from earlier [output](output-computing.md).

## ↑ Ancestors (4)

1. [Deflate](deflate.md)
2. [Data compression](data-compression.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Deflate backreference](deflate-backreference.md)
- [Deflate compression overhead](deflate-compression-overhead.md)
- [Deflate Huffman coding](deflate-huffman-coding.md)
- [Deflate literal byte](deflate-literal-byte.md)
