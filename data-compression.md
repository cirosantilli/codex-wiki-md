# Data compression

↑ **Parent:** [Computer science](computer-science-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_compression)

[Data compression](data-compression.md) represents data using fewer [bits](bit.md) than a specified original representation. The saving can reduce storage in a [file system](file-system.md) and reduce the number of [bits](bit.md) sent through a [communication channel](communication-channel.md). At a fixed transmission rate, fewer [bits](bit.md) arrive sooner; this makes better use of a fixed transmission budget. Both the encoded data and the instructions needed to interpret them contribute to the size of a stored file.

There are two different promises. [Lossless source coding](lossless-source-coding.md) preserves the original exactly: for an encoder $E$ and decoder $D$, $D(E(x))=x$ for every permitted [input](input-computer-science.md) $x$. Thus $E$ must be an [injective function](injective-function.md). [Lossy compression](lossy-compression.md) allows $D(E(x))$ to differ from $x$, with the difference judged by an explicit criterion. A program or numerical record may require exact recovery; a preview image may tolerate altered [pixels](pixel.md) in return for fewer [bits](bit.md).

The appeal of [lossless source coding](lossless-source-coding.md) is that repetition can be described rather than copied. [Run-length encoding](run-length-encoding.md) says "repeat this value twelve times"; a [prefix code](prefix-code.md) can give more frequent symbols shorter descriptions. These are distinct ways to exploit structure, and neither promises savings for every [input](input-computer-science.md). [Image compression](image-compression.md) supplies especially visible examples of both [lossless source coding](lossless-source-coding.md) and [lossy compression](lossy-compression.md).

Claude E. Shannon's 1948 paper made the role of [probability distributions](probability-distribution.md) precise. For a [memoryless classical information source](memoryless-classical-information-source.md) with [Shannon entropy](information-entropy.md) $H$ [bits](bit.md) per symbol, [Shannon's source coding theorem](shannon-s-source-coding-theorem.md) bounds achievable average lengths; sufficiently long blocks allow exact codes to approach $H$ [bits](bit.md) per symbol. This is a statement about a specified source and average lengths, not a promise to shorten every message.[Theorem 9 and its coding constructions](a-mathematical-theory-of-communication-by-claude-shannon.md)

**Table of contents**

- [Universal lossless shortening is impossible](universal-lossless-shortening-is-impossible.md)
- [Lossy compression](lossy-compression.md)
  - [Lossy block averaging](lossy-block-averaging.md)
- [Run-length encoding](run-length-encoding.md)
- [Deflate](deflate.md)
  - [Deflate literal byte](deflate-literal-byte.md)
  - [Deflate backreference](deflate-backreference.md)
    - [Deflate overlapping copy](deflate-overlapping-copy.md)
  - [Deflate Huffman coding](deflate-huffman-coding.md)
  - [Deflate block framing](deflate-block-framing.md)
  - [Deflate compression overhead](deflate-compression-overhead.md)
- [Image compression](image-compression.md)
  - [PNG](png.md)

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Data compression](data-compression.md)
- [File format](file-format.md)
- [Image compression](image-compression.md)
- [Sample depth](sample-depth.md)
