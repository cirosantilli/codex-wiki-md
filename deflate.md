# Deflate

↑ **Parent:** [Data compression](data-compression-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deflate)

[Deflate](deflate.md) is the [lossless source coding](lossless-source-coding.md) method specified for [PNG](png.md) compression. It can describe repeated stretches of earlier data, going beyond the single-value repetitions of [run-length encoding](run-length-encoding.md).[W3C, PNG Specification, Third Edition, section 10.1, compression method 0](portable-network-graphics-png-specification-third-edition-by-mark-adler-and-others.md)

The format combines [Deflate backreferences](deflate-backreference.md), which describe repeated stretches, with [Deflate Huffman coding](deflate-huffman-coding.md), which represents the resulting instructions using [prefix codes](prefix-code.md). [Deflate block framing](deflate-block-framing.md) tells the decoder which codes apply and where decoding stops. RFC 1951, [DEFLATE Compressed Data Format Specification version 1.3](https://www.rfc-editor.org/rfc/rfc1951) (May 1996), defines the format; different encoders can choose different instructions for the same [input](input-computer-science.md).[RFC 1951, heading and sections 2 and 4: format and encoder choices](deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch.md)

This separation is useful: discovering a repeated phrase and choosing short [codewords](codeword.md) solve different problems. A repeated phrase can contain many distinct [bytes](byte.md), while unequal [codeword lengths](codeword-length.md) can help even when no phrase repeats. Neither mechanism removes [Deflate compression overhead](deflate-compression-overhead.md) or guarantees a saving on every [input](input-computer-science.md).

**Table of contents**

- [Deflate literal byte](deflate-literal-byte.md)
- [Deflate backreference](deflate-backreference.md)
  - [Deflate overlapping copy](deflate-overlapping-copy.md)
- [Deflate Huffman coding](deflate-huffman-coding.md)
- [Deflate block framing](deflate-block-framing.md)
- [Deflate compression overhead](deflate-compression-overhead.md)

## ↑ Ancestors (3)

1. [Data compression](data-compression-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Deflate](deflate.md)
- [Deflate block framing](deflate-block-framing.md)
- [Deflate compression overhead](deflate-compression-overhead.md)
- [Image compression](image-compression.md)
