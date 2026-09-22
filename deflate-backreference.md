# Deflate backreference

↑ **Parent:** [Deflate](deflate.md)

A [Deflate backreference](deflate-backreference.md) specifies a length $\ell$ and backward distance $d$, measured in decoded [bytes](byte.md). If $n$ [bytes](byte.md) have already been produced, append $\ell$ [bytes](byte.md) starting at [output](output-computing.md) index $n-d$, counting indices from zero. The permitted ranges are $3\leq\ell\leq258$ and $1\leq d\leq32768$. Without a supplied initial history, $d\leq n$ is also required. The distance refers to decoded history, not a position in the compressed [input](input-computer-science.md).[RFC 1951, sections 3.2.3 and 3.2.5: available history, overlap, length and distance ranges](deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch.md)

For the twelve [bytes](byte.md) `ABCABCABCABC`, an illustrative instruction sequence is three [Deflate literal bytes](deflate-literal-byte.md) `A`, `B`, `C`, followed by the [Deflate backreference](deflate-backreference.md) $(\ell,d)=(9,3)$. [Run-length encoding](run-length-encoding.md) sees twelve single-[byte](byte.md) runs because neighbouring values differ; the [Deflate backreference](deflate-backreference.md) describes a repeated three-[byte](byte.md) pattern instead. Conversely, a [Deflate literal byte](deflate-literal-byte.md) `A` followed by $(7,1)$ produces `AAAAAAAA`: distance one can express a single-value repetition. These are chosen instructional examples, not claims about an encoder's chosen instructions or complete serialized streams.

**Table of contents**

- [Deflate overlapping copy](deflate-overlapping-copy.md)

## ↑ Ancestors (4)

1. [Deflate](deflate.md)
2. [Data compression](data-compression.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Deflate](deflate.md)
- [Deflate backreference](deflate-backreference.md)
- [Deflate compression overhead](deflate-compression-overhead.md)
- [Deflate Huffman coding](deflate-huffman-coding.md)
- [Deflate literal byte](deflate-literal-byte.md)
- [Deflate overlapping copy](deflate-overlapping-copy.md)
