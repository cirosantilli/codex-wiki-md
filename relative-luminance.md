# Relative luminance

↑ **Parent:** [sRGB](srgb.md)

For the normalized [sRGB](srgb.md) calculations here, [relative luminance](relative-luminance.md) is the linear-light weighted sum

$$
Y=0.2126R+0.7152G+0.0722B,
$$

where $R,G,B$ are decoded linear-light components, not encoded code values. This is the [sRGB](srgb.md) calculation specified in W3C's WCAG 2.2 definition of [relative luminance](relative-luminance.md). It places reference black at 0 and reference white at 1; it does not by itself specify an absolute display light level.[W3C, WCAG 2.2, definition of relative luminance: sRGB decoding and weights](https://www.w3.org/TR/WCAG22/#dfn-relative-luminance)

For a neutral [sRGB](srgb.md) shade, $R=G=B=l$, and the weights sum to 1, so $Y=l$. For a coloured [pixel](pixel.md), [relative luminance](relative-luminance.md) can be encoded as a neutral [sRGB](srgb.md) shade with all three encoded components $E(Y)$. This preserves the specified $Y$ while discarding colour differences; it is one precisely defined [grayscale](grayscale.md) conversion, not a unique way to turn all colour images into [grayscale](grayscale.md).

## ↑ Ancestors (4)

1. [sRGB](srgb.md)
2. [Computer graphics](computer-graphics.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Grayscale](grayscale.md)
- [Relative luminance](relative-luminance.md)
- [Sample depth](sample-depth.md)
- [sRGB](srgb.md)
- [Vector graphics](vector-graphics.md)
