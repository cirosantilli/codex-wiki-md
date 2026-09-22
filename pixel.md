# Pixel

↑ **Parent:** [Raster graphics](raster-graphics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pixel)

A [pixel](pixel.md) is one picture element at an indexed position in a [raster image](raster-graphics.md). It can contain a single [grayscale](grayscale.md) value or several colour components. The word can also refer to a physical display element; the indexed element of the stored image is the meaning used here. One stored [pixel](pixel.md) need not occupy exactly one physical display element when the image is resized. Microsoft's bitmap documentation likewise distinguishes an image's grid and its numerical colour representation.[Microsoft Learn, About Bitmaps: pixel grids and bitmap representations](https://learn.microsoft.com/en-us/windows/win32/gdi/about-bitmaps)

Separate _position_ from _value_: [raster sampling and reconstruction](raster-sampling-and-reconstruction.md) concerns the spatial grid, while [sample depth](sample-depth.md) concerns how many [bits](bit.md) encode each component. Four times as many [pixels](pixel.md) can describe a finer grid without improving the [quantization](quantization-signal-processing.md) of any value. Conversely, more [bits](bit.md) per sample can distinguish more shades without locating an edge more precisely.

In the binary example under [run-length encoding](run-length-encoding.md), one [bit](bit.md) per [pixel](pixel.md) selects black or white. In the [grayscale](grayscale.md) example under [lossy block averaging](lossy-block-averaging.md), eight [bits](bit.md) per [pixel](pixel.md) select one of 256 codes. Calling them codes keeps their numerical values distinct from the physical light that a display emits.

**Table of contents**

- [Sample depth](sample-depth.md)

## ↑ Ancestors (4)

1. [Raster graphics](raster-graphics.md)
2. [Computer graphics](computer-graphics.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Confocal optical sectioning](confocal-optical-sectioning.md)
- [Data compression](data-compression.md)
- [Fluorescence microscope](fluorescence-microscope.md)
- [Grayscale](grayscale.md)
- [Image compression](image-compression.md)
- [Lossy block averaging](lossy-block-averaging.md)
- [Lossy compression](lossy-compression.md)
- [Nearest-neighbor interpolation](nearest-neighbor-interpolation.md)
- [Pixel](pixel.md)
- [Raster graphics](raster-graphics.md)
- [Raster sampling and reconstruction](raster-sampling-and-reconstruction.md)
- [Relative luminance](relative-luminance.md)
- [Run-length encoding](run-length-encoding.md)
- [Sample depth](sample-depth.md)
- [Vector graphics](vector-graphics.md)
