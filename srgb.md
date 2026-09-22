# sRGB

↑ **Parent:** [Computer graphics](computer-graphics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/sRGB)

[sRGB](srgb.md) specifies a red-green-blue colour encoding. Restricting attention to component values in $[0,1]$, its encoded component $s$ corresponds to the linear-light component

$$
D(s)=\begin{cases}s/12.92,&0\leq s\leq0.04045,\\((s+0.055)/1.055)^{2.4},&0.04045<s\leq1.\end{cases}
$$

Thus the conversion is piecewise, not a single power law. The reverse conversion used here is

$$
E(l)=\begin{cases}12.92l,&0\leq l\leq0.0031308,\\1.055l^{1/2.4}-0.055,&0.0031308<l\leq1.\end{cases}
$$

These conventional rounded thresholds are used by the W3C conversion routines; they give a tiny mismatch at the join rather than a mathematically exact pair of inverses everywhere.[W3C, CSS Color Module Level 4, section 10.2: encoded and linear-light sRGB](https://www.w3.org/TR/css-color-4/#predefined-sRGB)[W3C, CSS Color Module Level 4, sample colour-conversion code: lin\_sRGB and gam\_sRGB](https://www.w3.org/TR/css-color-4/#color-conversion-code)

For an eight-[bit](bit.md) neutral [grayscale](grayscale.md) code $q$, use $s=q/255$ in all three components. Its [relative luminance](relative-luminance.md) is then $D(s)$. For example, $D(0.5)\approx0.21404$, whereas $E(0.5)\approx0.73536$. This is why averaging encoded values and averaging linear light give different answers. [sRGB](srgb.md) is a specified interpretation; merely calling a [raster image](raster-graphics.md) [grayscale](grayscale.md) does not imply it uses [sRGB](srgb.md).

**Table of contents**

- [Relative luminance](relative-luminance.md)

## ↑ Ancestors (3)

1. [Computer graphics](computer-graphics-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Grayscale](grayscale.md)
- [Relative luminance](relative-luminance.md)
- [Sample depth](sample-depth.md)
- [sRGB](srgb.md)
- [Vector graphics](vector-graphics.md)
