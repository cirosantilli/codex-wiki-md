# Raster sampling and reconstruction

↑ **Parent:** [Raster graphics](raster-graphics.md)

A point-sampling model assigns $p_{rc}=f(x_c,y_r)$ to a [pixel](pixel.md) on a grid, where $f$ is a [continuous function](continuous-function.md) representing an [image signal](image-signal.md). An area-sampling model instead assigns the [average value of a function](average-value-of-a-function.md) over a specified footprint. These are different models: a narrow feature between point samples can be missed, whereas its contribution to an area sample depends on its width and shade. Neither model says that the recorded value uniquely determines everything inside a grid cell.

<a id="image-a-toy-raster-grid-two-reconstructions-and-distinct-signals-with-identical-samples"></a>
![](raster-pixels-grayscale-sampling.png)

**[Figure 2](#image-a-toy-raster-grid-two-reconstructions-and-distinct-signals-with-identical-samples). A toy raster grid, two reconstructions, and distinct signals with identical samples**.

The upper panels start with exactly the same $6\times4$ [array](array-data-structure.md). [Nearest-neighbor interpolation](nearest-neighbor-interpolation.md) repeats its values into a $24\times16$ display; successive [linear interpolations](linear-interpolation.md) in the two coordinate directions produce a smoother $24\times16$ display. Original sample positions are marked. Both displays use 384 output [pixels](pixel.md), but only the same 24 recorded values. The extra values follow the chosen [interpolation](interpolation.md) rule. Between-grid appearance is inferred, not independently recorded.

Spatial resolution needs a stated meaning. A grid over a rectangle of width $L_x$ and height $L_y$ has nominal cell pitches $\Delta x=L_x/W$ and $\Delta y=L_y/H$. Over the same rectangle, doubling both dimensions halves these pitches and quadruples the [pixel](pixel.md) count. That is a finer grid, not a guarantee of more recoverable detail. Blurring before sampling, [quantization](quantization-signal-processing.md) and [aliasing](aliasing.md) can make different originals share the same recorded [array](array-data-structure.md). Enlarging the rectangle without adding samples instead increases the displayed pitch.

A reproducible computational demonstration makes the ambiguity exact. Take the one-dimensional profiles $f(x)=0.5+0.4\sin(2\pi x)$ and $g(x)=0.5+0.4\sin(10\pi x)$, repeated identically along every row. Sample at $x_j=j/4$ for $j=0,\ldots,8$. Since $10\pi x_j=2\pi x_j+2\pi j$, the fact that the [sine](sine.md) is a [periodic function](periodic-function.md) gives $f(x_j)=g(x_j)$. Both yield $0.5,0.9,0.5,0.1,0.5,0.9,0.5,0.1,0.5$, although at $x=1/8$ they give approximately $0.78284$ and $0.21716$. The lower panel draws both originals and their common samples: no operation on those samples alone can identify the original profile. This is [aliasing](aliasing.md) in an ideal point-sampling model, without [image noise](image-noise.md) or rounding.

The [Nyquist–Shannon sampling theorem](nyquist-shannon-sampling-theorem.md) describes reconstruction under a bandwidth restriction and ideal sampling assumptions; it does not grant uniqueness for arbitrary [image signals](image-signal.md) from a finite [raster image](raster-graphics.md).[Shannon, Communication in the Presence of Noise (1949), section II, Theorem 1 and reconstruction from the infinite sample sequence](https://fab.cba.mit.edu/classes/S62.12/docs/Shannon_noise.pdf) The beautiful lesson is constructive: choose what detail the grid should preserve before sampling, and choose a reconstruction rule suited to the information actually retained.

## ↑ Ancestors (4)

1. [Raster graphics](raster-graphics.md)
2. [Computer graphics](computer-graphics.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Pixel](pixel.md)
- [Raster graphics](raster-graphics.md)
- [Vector graphics](vector-graphics.md)
