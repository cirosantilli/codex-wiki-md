# Deflate compression overhead

↑ **Parent:** [Deflate](deflate.md)

Short [inputs](input-computer-science.md) can spend much of their size on [Deflate block framing](deflate-block-framing.md), the end-of-block symbol and, for dynamic blocks, [Deflate Huffman coding](deflate-huffman-coding.md) descriptions. A repeated phrase is useful only if its [Deflate backreference](deflate-backreference.md) costs less than the [Deflate literal bytes](deflate-literal-byte.md) it replaces. [Huffman coding](huffman-coding.md) adapts instruction costs; it does not make either references or code descriptions free.

For an exact expansion example, take the 256 [bytes](byte.md) with values $0,1,\ldots,255$, each appearing once. A single fixed block containing only [Deflate literal bytes](deflate-literal-byte.md) costs $144\cdot8+112\cdot9+7+3=2170$ [bits](bit.md), or 272 [bytes](byte.md) after final packing. One stored block starting at a [byte](byte.md) boundary instead costs five overhead [bytes](byte.md) plus the 256 data [bytes](byte.md), or 261 [bytes](byte.md). Both exceed the 256-[byte](byte.md) [input](input-computer-science.md); these counts follow the specified layouts and are not measurements of an encoder's automatic choice. The example illustrates [universal lossless shortening is impossible](universal-lossless-shortening-is-impossible.md).[RFC 1951, sections 3.2.3, 3.2.4 and 3.2.6: header, stored layout and fixed literal lengths](deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch.md)

The following independent experiment obtains an actual raw [Deflate](deflate.md) stream using the standard library's `zlib` module, then checks exact recovery. Negative `wbits` selects raw framing; the three lines of compressed-data handling make no assumptions about which [Deflate backreferences](deflate-backreference.md) the library selects.[Python 3.14 zlib documentation, compressobj, decompress and negative wbits](python-3-14-documentation/zlib-compression-compatible-with-gzip-python-3-14-documentation.md)
```
import zlib
data = b"ABCABCABCABC"
encoder = zlib.compressobj(level=6, wbits=-15)
packed = encoder.compress(data) + encoder.flush()
assert zlib.decompress(packed, wbits=-15) == data
print(len(data), len(packed), packed.hex())
```
The printed [bytes](byte.md) describe this library run. Exact roundtrip recovery is the check; a particular compressed length or instruction choice is not a guarantee for other [inputs](input-computer-science.md) or library versions.

## ↑ Ancestors (4)

1. [Deflate](deflate.md)
2. [Data compression](data-compression-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Deflate](deflate.md)
