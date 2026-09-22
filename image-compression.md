# Image compression

↑ **Parent:** [Data compression](data-compression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Image_compression)

[Image compression](image-compression.md) applies [data compression](data-compression.md) to pictures, usually represented by [raster images](raster-graphics.md). Nearby [pixels](pixel.md) often have related shades; an encoder can exploit that structure. A flat region invites [run-length encoding](run-length-encoding.md), while [lossy block averaging](lossy-block-averaging.md) trades fine detail for fewer stored samples. The choice depends on whether exact [pixel](pixel.md) values matter and on the patterns in the image.

[Lossless source coding](lossless-source-coding.md) recovers the encoded [pixel](pixel.md) values exactly, including sharp text or numerical image data. [Lossy compression](lossy-compression.md) preserves an approximation and can remove features that later [image processing](image-processing.md) might need. A visually smooth result is therefore a different promise from exact recovery. Neither method has a universal compression ratio: the chosen [file format](file-format.md), its [file header](file-header.md) and the particular image all matter.

[PNG](png.md) is a real format with [lossless source coding](lossless-source-coding.md) of its encoded image data. Its specified compression uses [Deflate](deflate.md) on reversibly filtered rows, rather than our toy [RLE](run-length-encoding.md) format. The [lossy block averaging](lossy-block-averaging.md) example is also a teaching format, not a description of [PNG](png.md). A lossy preprocessing step followed by saving as [PNG](png.md) preserves the already changed [pixels](pixel.md), not the earlier original.[W3C, PNG Specification, Third Edition (2025), section 10, Compression](portable-network-graphics-png-specification-third-edition-by-mark-adler-and-others.md)

**Table of contents**

- [PNG](png.md)

## ↑ Ancestors (3)

1. [Data compression](data-compression.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Data compression](data-compression.md)
- [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md)
- [File header](file-header.md)
- [Image compression](image-compression.md)
- [Lossy block averaging](lossy-block-averaging.md)
- [Low-rank approximation](low-rank-approximation.md)
- [Raster graphics](raster-graphics.md)
- [Singular value decomposition](singular-value-decomposition.md)
- [Wavelet](wavelet.md)
