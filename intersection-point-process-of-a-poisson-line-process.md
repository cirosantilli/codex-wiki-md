# Intersection point process of a Poisson line process

↑ **Parent:** [Poisson line process](poisson-line-process.md)

For an isotropic [Poisson line process](poisson-line-process.md) of intensity $c\,dp\,d\theta$, its pair intersections form a locally finite [point process](point-process.md). Coincident intersections and parallel pairs have [probability](probability.md) zero. Its [intensity measure](intensity-measure-of-a-point-process.md) is $\pi c^2$ times area. Indeed the [Poisson factorial moment measure](poisson-factorial-moment-measure.md) and the [change of variables](change-of-variables-formula.md) from signed distances to intersection location give

$$
\mathbb E\#(\Phi\cap A)=\frac{c^2|A|}{2}\int_0^\pi\int_0^\pi|\sin(\theta-\phi)|\,d\theta\,d\phi=\pi c^2|A|.
$$

The factor $1/2$ counts unordered line pairs. Shared lines create dependence between intersections; this process is not a [Poisson point process](poisson-point-process.md).

**Table of contents**

- [Strict disk-void bound for a Poisson line process](strict-disk-void-bound-for-a-poisson-line-process.md)

## ↑ Ancestors (7)

1. [Poisson line process](poisson-line-process.md)
2. [Poisson point process](poisson-point-process.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
