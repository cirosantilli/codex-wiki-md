# Non-uniform rational B-spline

↑ **Parent:** [B-spline](b-spline.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-uniform_rational_B-spline)

A [non-uniform rational B-spline](non-uniform-rational-b-spline.md) surface is

$$
F(u,v)=\frac{\sum_{i,j}w_{ij}N_{i,p}(u)M_{j,q}(v)P_{ij}}{\sum_{i,j}w_{ij}N_{i,p}(u)M_{j,q}(v)}.
$$

Here the $N_{i,p}$ and $M_{j,q}$ are [B-spline](b-spline.md) basis functions for possibly nonuniform [spline knot sequences](spline-knot-sequence.md), and the $w_{ij}$ are weights. Positive weights make each evaluated point a [convex combination](convex-combination.md) of the active [control points](control-point.md), supplying [bounding volumes](bounding-volume.md) for geometric searches. The denominator must remain nonzero for the parametrization to be defined.

## ↑ Ancestors (8)

1. [B-spline](b-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Non-uniform rational B-spline](non-uniform-rational-b-spline.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/3/solution.md)
