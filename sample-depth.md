# Sample depth

↑ **Parent:** [Pixel](pixel.md)

The [sample depth](sample-depth.md) $b$ is the number of [bits](bit.md) allocated to one stored sample. An unsigned $b$-[bit](bit.md) [integer](integer-split.md) has $2^b$ codes, $0,\ldots,2^b-1$. This is per component, not automatically per [pixel](pixel.md): three eight-[bit](bit.md) components require 24 payload [bits](bit.md) per [pixel](pixel.md). A [raster image](raster-graphics.md) with $W H$ [pixels](pixel.md) and $k$ such components requires $WHkb$ payload [bits](bit.md) before [data compression](data-compression-split.md), padding or a [file header](file-header.md).

For a toy normalized shade $x\in[0,1]$, define uniform [quantization](quantization-signal-processing.md) with endpoints included by

$$
q_b(x)=\left\lfloor(2^b-1)x+\frac12\right\rfloor,\qquad \widehat x_b=\frac{q_b(x)}{2^b-1}.
$$

The [floor function](floor-function.md) implements rounding to the nearest code, with exact halves rounded upward. The reconstruction step is $\delta_b=1/(2^b-1)$, and $|\widehat x_b-x|\leq\delta_b/2$. For $b=2$, the levels are $0,1/3,2/3,1$; for $b=8$ they are $0,1/255,\ldots,1$. Increasing [sample depth](sample-depth.md) refines this value grid without changing the spatial grid. These levels are uniform in $x$; if $x$ is encoded [sRGB](srgb.md), they are not uniform in [relative luminance](relative-luminance.md).

[PNG](png.md) uses a bit-depth field per sample or palette index. Its [grayscale](grayscale.md) type without alpha permits 1, 2, 4, 8 or 16 [bits](bit.md) per sample; its truecolour type permits 8 or 16 [bits](bit.md) per component. These are format-specific restrictions, not a rule for every [raster image](raster-graphics.md).[W3C, PNG Specification, Third Edition, section 11.2.1, IHDR, Table 12](https://www.w3.org/TR/png-3/#11IHDR)

## ↑ Ancestors (5)

1. [Pixel](pixel.md)
2. [Raster graphics](raster-graphics.md)
3. [Computer graphics](computer-graphics-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Grayscale](grayscale.md)
- [Pixel](pixel.md)
- [Sample depth](sample-depth.md)
