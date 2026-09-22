# Raster graphics

↑ **Parent:** [Computer graphics](computer-graphics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Raster_graphics)

[Raster graphics](raster-graphics.md) describe a picture by an [array](array-data-structure.md) of [pixels](pixel.md) on a grid. For a rectangular image of width $W$ and height $H$, write its stored values as $p_{rc}$, with $0\leq r<H$ and $0\leq c<W$. A [grayscale](grayscale.md) [pixel](pixel.md) can have one shade value; a colour [pixel](pixel.md) can have several component values. The grid specifies where values belong, while the encoding specifies what those values mean. A [raster image](raster-graphics.md) therefore needs dimensions and an interpretation of its samples, not just a string of numbers.

The appealing feature is that pictures become explicit data: selecting a rectangle selects entries of an [array](array-data-structure.md); comparing two images compares their [pixel](pixel.md) values; [image compression](image-compression.md) can exploit repeated or related values. [Raster sampling and reconstruction](raster-sampling-and-reconstruction.md) explains why the stored grid and the displayed picture are different objects. A square drawn around a sample is one display convention, not a claim that the original scene consisted of little squares.

For example, a $6\times4$ [grayscale](grayscale.md) [raster image](raster-graphics.md) stores 24 [pixel](pixel.md) values, even when displayed across a much larger rectangle. With one unsigned eight-[bit](bit.md) sample per [pixel](pixel.md), its uncompressed sample payload is $24\cdot8=192$ [bits](bit.md); a [file format](file-format.md) can additionally require a [file header](file-header.md), padding and other information, and [image compression](image-compression.md) can change the stored size.

Enlarging that image can copy each [pixel](pixel.md) into a block through [nearest-neighbor interpolation](nearest-neighbor-interpolation.md), or infer intermediate values through [interpolation](interpolation-split.md). Either procedure supplies a reconstruction rule; neither determines which unrecorded detail was present in the original. [Vector graphics](vector-graphics.md) use a different representation, specifying geometric objects to be rendered onto a chosen grid. Re-rendering such a description and enlarging an existing [raster image](raster-graphics.md) are different operations.

**Table of contents**

- [Pixel](pixel.md)
  - [Sample depth](sample-depth.md)
- [Grayscale](grayscale.md)
- [Raster sampling and reconstruction](raster-sampling-and-reconstruction.md)

## ↑ Ancestors (3)

1. [Computer graphics](computer-graphics-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Raster graphics](raster-graphics.md)
- [Vector graphics](vector-graphics.md)
