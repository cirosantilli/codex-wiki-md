# Data compression

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_compression)

[Data compression](data-compression.md) represents data using fewer [bits](information-theory.md#bit) than a specified original representation. The saving can reduce storage in a [file system](file-system.md) and reduce the number of [bits](information-theory.md#bit) sent through a [communication channel](information-theory.md#communication-channel). At a fixed transmission rate, fewer [bits](information-theory.md#bit) arrive sooner; this makes better use of a fixed transmission budget. Both the encoded data and the instructions needed to interpret them contribute to the size of a stored file.

There are two different promises. [Lossless source coding](information-theory.md#lossless-source-coding) preserves the original exactly: for an encoder $E$ and decoder $D$, $D(E(x))=x$ for every permitted [input](theoretical-computer-science.md#input-computer-science) $x$. Thus $E$ must be an [injective function](algebra.md#injective-function). [Lossy compression](#lossy-compression) allows $D(E(x))$ to differ from $x$, with the difference judged by an explicit criterion. A program or numerical record may require exact recovery; a preview image may tolerate altered [pixels](computer-graphics.md#pixel) in return for fewer [bits](information-theory.md#bit).

The appeal of [lossless source coding](information-theory.md#lossless-source-coding) is that repetition can be described rather than copied. [Run-length encoding](#run-length-encoding) says "repeat this value twelve times"; a [prefix code](coding-theory.md#prefix-code) can give more frequent symbols shorter descriptions. These are distinct ways to exploit structure, and neither promises savings for every [input](theoretical-computer-science.md#input-computer-science). [Image compression](#image-compression) supplies especially visible examples of both [lossless source coding](information-theory.md#lossless-source-coding) and [lossy compression](#lossy-compression).

Claude E. Shannon's 1948 paper made the role of [probability distributions](probability-distribution.md) precise. For a [memoryless classical information source](information-theory.md#memoryless-classical-information-source) with [Shannon entropy](information-entropy.md) $H$ [bits](information-theory.md#bit) per symbol, [Shannon's source coding theorem](coding-theory.md#shannon-s-source-coding-theorem) bounds achievable average lengths; sufficiently long blocks allow exact codes to approach $H$ [bits](information-theory.md#bit) per symbol. This is a statement about a specified source and average lengths, not a promise to shorten every message.[Theorem 9 and its coding constructions](mathematics-bibliography.md#a-mathematical-theory-of-communication-by-claude-shannon)

**Table of contents**

- [Universal lossless shortening is impossible](#universal-lossless-shortening-is-impossible)
- [Lossy compression](#lossy-compression)
  - [Lossy block averaging](#lossy-block-averaging)
- [Run-length encoding](#run-length-encoding)
- [Deflate](#deflate)
  - [Deflate literal byte](#deflate-literal-byte)
  - [Deflate backreference](#deflate-backreference)
    - [Deflate overlapping copy](#deflate-overlapping-copy)
  - [Deflate Huffman coding](#deflate-huffman-coding)
  - [Deflate block framing](#deflate-block-framing)
  - [Deflate compression overhead](#deflate-compression-overhead)
- [Image compression](#image-compression)
  - [PNG](#png)

## Universal lossless shortening is impossible

↑ **Parent:** [Data compression](data-compression.md)

Fix $n\geq1$. There is no [injective function](algebra.md#injective-function) from all length-$n$ [binary strings](theoretical-computer-science.md#binary-string) to [binary strings](theoretical-computer-science.md#binary-string) of length strictly less than $n$. There are $2^n$ possible [inputs](theoretical-computer-science.md#input-computer-science), but even allowing the empty string gives only

$$
\sum_{k=0}^{n-1}2^k=2^n-1
$$

possible shorter [outputs](theoretical-computer-science.md#output-computing). The [finite geometric series](sequence-and-series.md#finite-geometric-series) and [pigeonhole principle](combinatorics.md#pigeonhole-principle) leave at least two [inputs](theoretical-computer-science.md#input-computer-science) sharing an [output](theoretical-computer-science.md#output-computing), which prevents exact decoding. For $n=3$, eight [inputs](theoretical-computer-science.md#input-computer-science) compete for the empty string and the six strings `0`, `1`, `00`, `01`, `10`, `11`.

This counting argument includes any [file header](computer-science.md#file-header) or other information sent to the decoder. An [algorithm](algorithm.md) chosen separately for each [input](theoretical-computer-science.md#input-computer-science) must also be identified to the receiver; its description is not free. A useful compressor saves space on some [inputs](theoretical-computer-science.md#input-computer-science) while leaving others unchanged or making them longer. [Lossy compression](#lossy-compression) avoids the exact-recovery requirement by deliberately allowing several [inputs](theoretical-computer-science.md#input-computer-science) to share an [output](theoretical-computer-science.md#output-computing).

## Lossy compression

↑ **Parent:** [Data compression](data-compression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lossy_compression)

[Lossy compression](#lossy-compression) reduces a representation while permitting irreversible changes to the original. The encoder can map distinct [inputs](theoretical-computer-science.md#input-computer-science) to the same [output](theoretical-computer-science.md#output-computing), so its decoder cannot recover both originals exactly. The useful question becomes how much storage is saved for an acceptable amount of distortion: [mean squared error](statistical-modelling.md#mean-squared-error) is one numerical criterion, but it does not by itself measure how noticeable a visual change is.

For example, storing the [arithmetic mean](arithmetic.md#arithmetic-mean) of four [grayscale](computer-graphics.md#grayscale) [pixels](computer-graphics.md#pixel) retains their average shade while discarding their arrangement. Blocks $\left(\begin{smallmatrix}0&100\\100&0\end{smallmatrix}\right)$ and $\left(\begin{smallmatrix}50&50\\50&50\end{smallmatrix}\right)$ both produce 50. The former has detail and the latter is uniform, yet the decoder receives the same value. [Lossy block averaging](#lossy-block-averaging) makes this ambiguity, its [bit](information-theory.md#bit) saving and its [mean squared error](statistical-modelling.md#mean-squared-error) exact.

### Lossy block averaging

↑ **Parent:** [Lossy compression](#lossy-compression)

This toy [image compression](#image-compression) method stores one rounded [arithmetic mean](arithmetic.md#arithmetic-mean) for each disjoint $2\times2$ block of [grayscale](computer-graphics.md#grayscale) [pixels](computer-graphics.md#pixel). The [quantization](computer-science.md#quantization-signal-processing) rule is round to the nearest [integer](integer.md), with exact halves rounded upward. Each stored value is an unsigned eight-[bit](information-theory.md#bit) [integer](integer.md). Reconstruction fills the original block with that value, a form of [nearest-neighbor interpolation](computer-science.md#nearest-neighbor-interpolation). Averaging already discards information; rounding can discard more.

Here is an exact $16\times16$ source [array](data-structure.md#array-data-structure). Index rows and columns by $r,c\in\{0,\ldots,15\}$ and define

$$
\begin{aligned}
b_{rc}&=40+10\lfloor r/2\rfloor+12\lfloor c/2\rfloor,\\
x_{rc}&=b_{rc}+20(-1)^{r+c}+\mathbf{1}_{\{r\text{ even},\ c\text{ even}\}}.
\end{aligned}
$$

The [floor function](calculus.md#floor-function) makes $b$ constant within each block; the [indicator function](measure-theory.md#indicator-function) adds 1 only to its upper-left [pixel](computer-graphics.md#pixel). All values are [integers](integer.md) from 20 to 215. Each block therefore has the exact form

$$
\begin{pmatrix}b+21&b-20\\b-20&b+20\end{pmatrix},\qquad m=b+\tfrac14,\qquad q=\lfloor m+\tfrac12\rfloor=b.
$$

For example, the upper-left block $\left(\begin{smallmatrix}61&20\\20&60\end{smallmatrix}\right)$ has [arithmetic mean](arithmetic.md#arithmetic-mean) $161/4=40.25$ and is stored as 40. The block immediately to its right $\left(\begin{smallmatrix}73&32\\32&72\end{smallmatrix}\right)$ is stored as 52. The complete stored $8\times8$ [array](data-structure.md#array-data-structure) is specified by $q_{ij}=40+10i+12j$ for $0\leq i,j\leq7$. Its first row is $40,52,64,76,88,100,112,124$; its last is $110,122,134,146,158,170,182,194$.

This toy [file format](computer-science.md#file-format) again has eight-[bit](information-theory.md#bit) width and height fields followed by a one-[bit](information-theory.md#bit) mode: 0 means raw eight-[bit](information-theory.md#bit) [grayscale](computer-graphics.md#grayscale) [pixels](computer-graphics.md#pixel), 1 means the rounded block [arithmetic means](arithmetic.md#arithmetic-mean). This profile accepts only width and height 16. The decoder knows the block size and reconstruction rule from the format, reads the 64 stored values in row order, and repeats each across its corresponding $2\times2$ block. The original 256 [pixels](computer-graphics.md#pixel) cost $256\cdot8=2048$ payload [bits](information-theory.md#bit); the 64 stored values cost $64\cdot8=512$ payload [bits](information-theory.md#bit). The reduction is $75\%$. These payload counts exclude the common 17-[bit](information-theory.md#bit) [file header](computer-science.md#file-header); complete sizes are 2065 and 529 [bits](information-theory.md#bit), or 2072 and 536 [bits](information-theory.md#bit) after final zero padding to eight-[bit](information-theory.md#bit) units. There is no stored codebook or additional prediction rule.

The empirical [mean squared error](statistical-modelling.md#mean-squared-error) averages squared differences over the 256 original [pixel](computer-graphics.md#pixel) positions:

$$
\operatorname{MSE}=\frac1{256}\sum_{r=0}^{15}\sum_{c=0}^{15}(x_{rc}-\widehat x_{rc})^2
=\frac{21^2+20^2+20^2+20^2}{4}=410.25.
$$

Every block has the same four errors, so this value is exact in squared stored shade units. If the unrounded [arithmetic mean](arithmetic.md#arithmetic-mean) $b+1/4$ could be reconstructed, the error would instead be $410.1875$; eight-[bit](information-theory.md#bit) [quantization](computer-science.md#quantization-signal-processing) adds $0.0625$. That hypothetical comparison does not count fractional means as free eight-[bit](information-theory.md#bit) values.

The broad shade pattern survives, while the alternating bright and dark [pixels](computer-graphics.md#pixel) vanish. Indeed, a second source with every block constant at $b$ produces the identical stored [array](data-structure.md#array-data-structure) $q$: exact decoding of both sources is impossible. This makes the storage benefit and the lost detail visible at once. Block averaging is useful for a coarse preview when the individual [pixels](computer-graphics.md#pixel) are dispensable; choosing an acceptable [mean squared error](statistical-modelling.md#mean-squared-error) or visual result is part of the application, not a guarantee supplied by the encoder.

<a id="image-rounded-2-by-2-block-means-reduce-the-payload-by-75-percent-while-destroying-fine-detail"></a>
![](lossy-block-image-comparison.png)

**[Figure 1](#image-rounded-2-by-2-block-means-reduce-the-payload-by-75-percent-while-destroying-fine-detail). Rounded 2 by 2 block means reduce the payload by 75 percent while destroying fine detail**.

## Run-length encoding

↑ **Parent:** [Data compression](data-compression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Run-length_encoding)

[Run-length encoding](#run-length-encoding) replaces each maximal consecutive group of equal values, called a run, by its value and length. Decoding repeats each value the specified number of times. It is [lossless source coding](information-theory.md#lossless-source-coding): no values are discarded. For a [binary string](theoretical-computer-science.md#binary-string), successive maximal runs alternate between 0 and 1, so storing the first [bit](information-theory.md#bit) and all run lengths is enough.

Take this $8\times8$ [raster image](computer-graphics.md#raster-graphics), with 0 black and 1 white, read left to right across each row and then top to bottom:
```
00000000
00001111
11110000
00001111
11110000
00001111
11110000
00000000
```
Reading the whole image as one 64-[bit](information-theory.md#bit) [binary string](theoretical-computer-science.md#binary-string) gives exactly seven runs:

$$
(\text{value},\text{length})=(0,12),(1,8),(0,8),(1,8),(0,8),(1,8),(0,12).
$$

The lengths sum to $12+8+8+8+8+8+12=64$. Repeating the alternating values for these lengths and splitting after every eighth [pixel](computer-graphics.md#pixel) reconstructs every displayed row exactly.

Here is a complete toy [file format](computer-science.md#file-format). Its [file header](computer-science.md#file-header) is an eight-[bit](information-theory.md#bit) unsigned width, an eight-[bit](information-theory.md#bit) unsigned height, then a one-[bit](information-theory.md#bit) mode: 0 means raw [pixels](computer-graphics.md#pixel), 1 means [run-length encoding](#run-length-encoding). Fields are written most significant [bit](information-theory.md#bit) first; this profile accepts only width and height 8, so both decoders know to stop at 64 [pixels](computer-graphics.md#pixel). Raw mode contains 64 [bits](information-theory.md#bit). [RLE](#run-length-encoding) mode contains the initial [bit](information-theory.md#bit), followed by seven-[bit](information-theory.md#bit) unsigned run lengths in the range 1 to 64. Zero and lengths above 64 are invalid; a decoder rejects a run that would exceed the remaining [pixel](computer-graphics.md#pixel) count. It stops when the decoded lengths sum to 64, so no run-count field or end marker is needed.

For this image, the complete [RLE](#run-length-encoding) serialization is:
```
00001000 00001000 1 | 0 | 0001100 0001000 0001000 0001000 0001000 0001000 0001100
```
Spaces and vertical bars are explanatory separators, not stored characters. The seven-[bit](information-theory.md#bit) fields directly store the lengths; 64 would be `1000000`. The payload costs $1+7\cdot7=50$ [bits](information-theory.md#bit), versus 64 raw [bits](information-theory.md#bit). The 17-[bit](information-theory.md#bit) [file header](computer-science.md#file-header) has the same size in either mode, giving complete sizes of 67 versus 81 [bits](information-theory.md#bit). If packed into eight-[bit](information-theory.md#bit) units, append zero padding only at the end: the sizes become 72 versus 88 [bits](information-theory.md#bit). These are sizes of this toy representation, not sizes of [PNG](#png) files.

The field design matters. Restarting [RLE](#run-length-encoding) on every row costs eight initial [bits](information-theory.md#bit) plus four [bits](information-theory.md#bit) per run when lengths are stored directly: three [bits](information-theory.md#bit) represent only 0 through 7, whereas a row can have length 8. This pattern has row-run counts $1,2,2,2,2,2,2,1$, totalling 14, so that payload costs $8+4\cdot14=64$ [bits](information-theory.md#bit), with no saving. Storing length minus one would instead fit lengths 1 through 8 into three [bits](information-theory.md#bit), but is a different declared [file format](computer-science.md#file-format). An alternating flat 64-[bit](information-theory.md#bit) [binary string](theoretical-computer-science.md#binary-string) has 64 runs and costs $1+7\cdot64=449$ payload [bits](information-theory.md#bit) in our flat format; restarting each row costs $8+4\cdot64=264$ payload [bits](information-theory.md#bit). A one-run image costs only eight payload [bits](information-theory.md#bit). These extremes explain when [RLE](#run-length-encoding) is useful: long uninterrupted regions make short instructions, while frequent changes make instructions expensive.

[Prefix codes](coding-theory.md#prefix-code) of unequal lengths can replace fixed-width run lengths, provided the decoder knows the code and any necessary code description is counted. [Run-length encoding](#run-length-encoding) names a technique, not one universal serialization. For a real implementation, Microsoft's bitmap documentation specifies `BI_RLE8` with count and value fields plus special commands, rather than our initial-[bit](information-theory.md#bit) convention.[Microsoft, Bitmap Compression, BI\_RLE8 encoded and absolute modes](https://learn.microsoft.com/en-us/windows/win32/gdi/bitmap-compression)

<a id="image-seven-runs-serialize-an-8-by-8-binary-image-and-reconstruct-every-pixel-exactly"></a>
![](run-length-image-compression.png)

**[Figure 2](#image-seven-runs-serialize-an-8-by-8-binary-image-and-reconstruct-every-pixel-exactly). Seven runs serialize an 8 by 8 binary image and reconstruct every pixel exactly**.

## Deflate

↑ **Parent:** [Data compression](data-compression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deflate)

[Deflate](#deflate) is the [lossless source coding](information-theory.md#lossless-source-coding) method specified for [PNG](#png) compression. It can describe repeated stretches of earlier data, going beyond the single-value repetitions of [run-length encoding](#run-length-encoding).[W3C, PNG Specification, Third Edition, section 10.1, compression method 0](computer-science-bibliography.md#portable-network-graphics-png-specification-third-edition-by-mark-adler-and-others)

The format combines [Deflate backreferences](#deflate-backreference), which describe repeated stretches, with [Deflate Huffman coding](#deflate-huffman-coding), which represents the resulting instructions using [prefix codes](coding-theory.md#prefix-code). [Deflate block framing](#deflate-block-framing) tells the decoder which codes apply and where decoding stops. RFC 1951, [DEFLATE Compressed Data Format Specification version 1.3](https://www.rfc-editor.org/rfc/rfc1951) (May 1996), defines the format; different encoders can choose different instructions for the same [input](theoretical-computer-science.md#input-computer-science).[RFC 1951, heading and sections 2 and 4: format and encoder choices](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

This separation is useful: discovering a repeated phrase and choosing short [codewords](coding-theory.md#codeword) solve different problems. A repeated phrase can contain many distinct [bytes](computer-science.md#byte), while unequal [codeword lengths](coding-theory.md#codeword-length) can help even when no phrase repeats. Neither mechanism removes [Deflate compression overhead](#deflate-compression-overhead) or guarantees a saving on every [input](theoretical-computer-science.md#input-computer-science).

### Deflate literal byte

↑ **Parent:** [Deflate](#deflate)

A [Deflate literal byte](#deflate-literal-byte) instructs the decoder to append one specified [byte](computer-science.md#byte) directly to the [output](theoretical-computer-science.md#output-computing). For example, three [Deflate literal bytes](#deflate-literal-byte) with values 65, 66 and 67 produce `ABC`. These values are symbols in the [Deflate Huffman coding](#deflate-huffman-coding) stage, rather than necessarily eight raw stored [bits](information-theory.md#bit) each. A [Deflate backreference](#deflate-backreference) instead describes a copy from earlier [output](theoretical-computer-science.md#output-computing).

### Deflate backreference

↑ **Parent:** [Deflate](#deflate)

A [Deflate backreference](#deflate-backreference) specifies a length $\ell$ and backward distance $d$, measured in decoded [bytes](computer-science.md#byte). If $n$ [bytes](computer-science.md#byte) have already been produced, append $\ell$ [bytes](computer-science.md#byte) starting at [output](theoretical-computer-science.md#output-computing) index $n-d$, counting indices from zero. The permitted ranges are $3\leq\ell\leq258$ and $1\leq d\leq32768$. Without a supplied initial history, $d\leq n$ is also required. The distance refers to decoded history, not a position in the compressed [input](theoretical-computer-science.md#input-computer-science).[RFC 1951, sections 3.2.3 and 3.2.5: available history, overlap, length and distance ranges](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

For the twelve [bytes](computer-science.md#byte) `ABCABCABCABC`, an illustrative instruction sequence is three [Deflate literal bytes](#deflate-literal-byte) `A`, `B`, `C`, followed by the [Deflate backreference](#deflate-backreference) $(\ell,d)=(9,3)$. [Run-length encoding](#run-length-encoding) sees twelve single-[byte](computer-science.md#byte) runs because neighbouring values differ; the [Deflate backreference](#deflate-backreference) describes a repeated three-[byte](computer-science.md#byte) pattern instead. Conversely, a [Deflate literal byte](#deflate-literal-byte) `A` followed by $(7,1)$ produces `AAAAAAAA`: distance one can express a single-value repetition. These are chosen instructional examples, not claims about an encoder's chosen instructions or complete serialized streams.

#### Deflate overlapping copy

↑ **Parent:** [Deflate backreference](#deflate-backreference)

In a [Deflate overlapping copy](#deflate-overlapping-copy), $\ell>d$: some source [bytes](computer-science.md#byte) are created by the very copy being decoded. For each step $i=0,\ldots,\ell-1$, read the current [output](theoretical-computer-science.md#output-computing) at index $n+i-d$ and append that [byte](computer-science.md#byte) at index $n+i$. Because $d\geq1$, the source index is always smaller than the destination index, so the needed [byte](computer-science.md#byte) exists when it is read.[RFC 1951, section 3.2.3, printed p. 11: overlapping string references](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

For `ABC` followed by $(9,3)$, the source indices are $0,1,2,3,4,5,6,7,8$ and the destination indices are $3,4,5,6,7,8,9,10,11$. Steps 0 through 2 copy the original `ABC`; steps 3 through 5 copy the `ABC` just appended; steps 6 through 8 copy the next newly appended `ABC`. Thus the final [output](theoretical-computer-science.md#output-computing) is exactly `ABCABCABCABC`. Taking a snapshot of the original three-[byte](computer-science.md#byte) source slice would produce only three [bytes](computer-science.md#byte); that operation does not implement the specified nine-[byte](computer-science.md#byte) copy.

<a id="image-nine-successive-copies-at-distance-three-extend-abc-to-abcabcabcabc-using-newly-produced-bytes"></a>
![](deflate-overlapping-copy-trace.png)

**[Figure 3](#image-nine-successive-copies-at-distance-three-extend-abc-to-abcabcabcabc-using-newly-produced-bytes). Nine successive copies at distance three extend ABC to ABCABCABCABC using newly produced bytes**.

The reusable idea is a short description of periodic continuation: the decoder repeatedly looks a fixed distance behind its growing [output](theoretical-computer-science.md#output-computing). A [Deflate backreference](#deflate-backreference) can also reach across a [Deflate block framing](#deflate-block-framing) boundary. Changing the block's [Huffman codes](information-theory.md#huffman-code) does not by itself erase the decoded history.[RFC 1951, sections 2 and 3.2.3: independent block codes, references across blocks](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

### Deflate Huffman coding

↑ **Parent:** [Deflate](#deflate)

For a compressed block, [Deflate Huffman coding](#deflate-huffman-coding) uses one [alphabet](information-theory.md#alphabet) for [Deflate literal bytes](#deflate-literal-byte), length symbols and the end-of-block symbol, and another [alphabet](information-theory.md#alphabet) for distance symbols. Values 0 through 255 denote [Deflate literal bytes](#deflate-literal-byte), 256 ends the block, and 257 through 285 select lengths. A [Deflate backreference](#deflate-backreference) is encoded as a length symbol, any length extra [bits](information-theory.md#bit), a distance symbol, then any distance extra [bits](information-theory.md#bit). Those extra [bits](information-theory.md#bit) select an offset within the symbol's prescribed range; they are not additional [codewords](coding-theory.md#codeword).[RFC 1951, section 3.2.5, length and distance tables](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

In the illustrative $(9,3)$ [Deflate backreference](#deflate-backreference), length 9 uses symbol 263 and distance 3 uses symbol 2; neither needs extra [bits](information-theory.md#bit). Under the fixed [Huffman codes](information-theory.md#huffman-code), `A`, `B` and `C` each cost eight [bits](information-theory.md#bit), symbol 263 costs seven, and distance symbol 2 costs five. Adding the seven-[bit](information-theory.md#bit) end-of-block symbol and three-[bit](information-theory.md#bit) block header gives $3+3\cdot8+7+5+7=46$ [bits](information-theory.md#bit), packed into six [bytes](computer-science.md#byte) for a single final block. This is a cost calculation for the explicitly chosen instructions, not a displayed compressed stream.[RFC 1951, sections 3.2.5 and 3.2.6: length 9, distance 3 and fixed code lengths](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

Dynamic blocks transmit [codeword lengths](coding-theory.md#codeword-length) from which the decoder reconstructs the prescribed [prefix codes](coding-theory.md#prefix-code). The code descriptions themselves use a smaller [Huffman code](information-theory.md#huffman-code) and repeat instructions for successive [codeword lengths](coding-theory.md#codeword-length), including runs of zero lengths. Here [run-length encoding](#run-length-encoding) describes repeated code lengths, a separate role from copying repeated data [bytes](computer-science.md#byte). Fixed blocks use predefined [Huffman codes](information-theory.md#huffman-code) and avoid transmitting those descriptions.[RFC 1951, sections 3.2.2, 3.2.6 and 3.2.7: code reconstruction, fixed codes and dynamic code-length repeats](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

### Deflate block framing

↑ **Parent:** [Deflate](#deflate)

Each block starts with a one-[bit](information-theory.md#bit) `BFINAL` flag and a two-[bit](information-theory.md#bit) `BTYPE` field. The `BTYPE` values are 0 for stored data, 1 for fixed [Huffman codes](information-theory.md#huffman-code), 2 for dynamic [Huffman codes](information-theory.md#huffman-code), and 3 for an invalid reserved value. For compressed blocks, symbol 256 ends the current block; `BFINAL = 1` says this is the last block. An end-of-block symbol does not mean a literal zero [byte](computer-science.md#byte), and in a nonfinal block it does not end the whole stream.[RFC 1951, section 3.2.3: header, block types and decoding loop](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

<a id="image-deflate-separates-literal-and-copy-instructions-from-huffman-coding-and-final-block-framing-stored-blocks-bypass-both-stages"></a>
![](deflate-token-block-pipeline.png)

**[Figure 4](#image-deflate-separates-literal-and-copy-instructions-from-huffman-coding-and-final-block-framing-stored-blocks-bypass-both-stages). Deflate separates literal and copy instructions from Huffman coding and final-block framing; stored blocks bypass both stages**.

A stored block instead skips to the next [byte](computer-science.md#byte) boundary, reads the sixteen-[bit](information-theory.md#bit) `LEN` and its sixteen-[bit](information-theory.md#bit) one's complement `NLEN`, then copies exactly `LEN` raw [bytes](computer-science.md#byte). Its length field replaces the compressed block's end-of-block symbol. A compressed block need not end at a [byte](computer-science.md#byte) boundary, so the next block header can start inside the current [byte](computer-science.md#byte).[RFC 1951, sections 3.2.3 and 3.2.4: alignment, LEN, NLEN and stored data](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

The diagram shows logical fields, not a serialization into [bits](information-theory.md#bit). RFC 1951 specifies [bit](information-theory.md#bit) packing separately, including different conventions for [codewords](coding-theory.md#codeword) and other fields (section 3.1.1). For [PNG](#png), the filtered image data is compressed inside a zlib wrapper with its own header and checksum; raw [Deflate](#deflate) and a complete [PNG](#png) file therefore have different framing.[PNG Specification, Third Edition, sections 10.1 and 10.2: zlib wrapper and filtered image data](computer-science-bibliography.md#portable-network-graphics-png-specification-third-edition-by-mark-adler-and-others)

### Deflate compression overhead

↑ **Parent:** [Deflate](#deflate)

Short [inputs](theoretical-computer-science.md#input-computer-science) can spend much of their size on [Deflate block framing](#deflate-block-framing), the end-of-block symbol and, for dynamic blocks, [Deflate Huffman coding](#deflate-huffman-coding) descriptions. A repeated phrase is useful only if its [Deflate backreference](#deflate-backreference) costs less than the [Deflate literal bytes](#deflate-literal-byte) it replaces. [Huffman coding](information-theory.md#huffman-coding) adapts instruction costs; it does not make either references or code descriptions free.

For an exact expansion example, take the 256 [bytes](computer-science.md#byte) with values $0,1,\ldots,255$, each appearing once. A single fixed block containing only [Deflate literal bytes](#deflate-literal-byte) costs $144\cdot8+112\cdot9+7+3=2170$ [bits](information-theory.md#bit), or 272 [bytes](computer-science.md#byte) after final packing. One stored block starting at a [byte](computer-science.md#byte) boundary instead costs five overhead [bytes](computer-science.md#byte) plus the 256 data [bytes](computer-science.md#byte), or 261 [bytes](computer-science.md#byte). Both exceed the 256-[byte](computer-science.md#byte) [input](theoretical-computer-science.md#input-computer-science); these counts follow the specified layouts and are not measurements of an encoder's automatic choice. The example illustrates [universal lossless shortening is impossible](#universal-lossless-shortening-is-impossible).[RFC 1951, sections 3.2.3, 3.2.4 and 3.2.6: header, stored layout and fixed literal lengths](computer-science-bibliography.md#deflate-compressed-data-format-specification-version-1-3-by-l-peter-deutsch)

The following independent experiment obtains an actual raw [Deflate](#deflate) stream using the standard library's `zlib` module, then checks exact recovery. Negative `wbits` selects raw framing; the three lines of compressed-data handling make no assumptions about which [Deflate backreferences](#deflate-backreference) the library selects.[Python 3.14 zlib documentation, compressobj, decompress and negative wbits](computer-science-bibliography.md#python-3-14-documentation/zlib-compression-compatible-with-gzip-python-3-14-documentation)
```
import zlib
data = b"ABCABCABCABC"
encoder = zlib.compressobj(level=6, wbits=-15)
packed = encoder.compress(data) + encoder.flush()
assert zlib.decompress(packed, wbits=-15) == data
print(len(data), len(packed), packed.hex())
```
The printed [bytes](computer-science.md#byte) describe this library run. Exact roundtrip recovery is the check; a particular compressed length or instruction choice is not a guarantee for other [inputs](theoretical-computer-science.md#input-computer-science) or library versions.

## Image compression

↑ **Parent:** [Data compression](data-compression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Image_compression)

[Image compression](#image-compression) applies [data compression](data-compression.md) to pictures, usually represented by [raster images](computer-graphics.md#raster-graphics). Nearby [pixels](computer-graphics.md#pixel) often have related shades; an encoder can exploit that structure. A flat region invites [run-length encoding](#run-length-encoding), while [lossy block averaging](#lossy-block-averaging) trades fine detail for fewer stored samples. The choice depends on whether exact [pixel](computer-graphics.md#pixel) values matter and on the patterns in the image.

[Lossless source coding](information-theory.md#lossless-source-coding) recovers the encoded [pixel](computer-graphics.md#pixel) values exactly, including sharp text or numerical image data. [Lossy compression](#lossy-compression) preserves an approximation and can remove features that later [image processing](computer-science.md#image-processing) might need. A visually smooth result is therefore a different promise from exact recovery. Neither method has a universal compression ratio: the chosen [file format](computer-science.md#file-format), its [file header](computer-science.md#file-header) and the particular image all matter.

[PNG](#png) is a real format with [lossless source coding](information-theory.md#lossless-source-coding) of its encoded image data. Its specified compression uses [Deflate](#deflate) on reversibly filtered rows, rather than our toy [RLE](#run-length-encoding) format. The [lossy block averaging](#lossy-block-averaging) example is also a teaching format, not a description of [PNG](#png). A lossy preprocessing step followed by saving as [PNG](#png) preserves the already changed [pixels](computer-graphics.md#pixel), not the earlier original.[W3C, PNG Specification, Third Edition (2025), section 10, Compression](computer-science-bibliography.md#portable-network-graphics-png-specification-third-edition-by-mark-adler-and-others)

### PNG

↑ **Parent:** [Image compression](#image-compression)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/PNG)

[PNG](#png) is a [file format](computer-science.md#file-format) for [raster images](computer-graphics.md#raster-graphics) with [lossless source coding](information-theory.md#lossless-source-coding) of the encoded image data. Its first W3C Recommendation, dated 1 October 1996, described a portable replacement for earlier image formats; this situates the design in exchanging images reliably between systems.[W3C, PNG (Portable Network Graphics) Specification, 1 October 1996, status and abstract](https://www.w3.org/TR/REC-png-961001)

## ↑ Ancestors (2)

1. [Computer science](computer-science.md)
2. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Data compression](data-compression.md)
- [File format](computer-science.md#file-format)
- [Image compression](#image-compression)
- [Sample depth](computer-graphics.md#sample-depth)
