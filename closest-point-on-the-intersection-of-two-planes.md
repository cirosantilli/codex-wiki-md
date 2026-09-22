# Closest point on the intersection of two planes

↑ **Parent:** [Distance from a point to a line in three dimensions](distance-from-a-point-to-a-line-in-three-dimensions.md)

For two [planes](plane.md) $r\cdot b=\lambda$ and $r\cdot c=\mu$ with [linearly independent](linear-independence.md) [normal vectors](normal-vector.md), put $B=b\cdot b$, $C=c\cdot c$, $D=b\cdot c$ and $\Delta=BC-D^2>0$. Their intersection is a [line](straight-line.md) parallel to $b\times c$. Its closest point to the origin is [orthogonal](orthogonal-vectors.md) to that direction, hence has the form $a=\alpha b+\beta c$. The constraints give $B\alpha+D\beta=\lambda$, $D\alpha+C\beta=\mu$, so

$$
\alpha=\frac{C\lambda-D\mu}{\Delta},\qquad
\beta=\frac{B\mu-D\lambda}{\Delta},\qquad
|a|^2=\frac{C\lambda^2-2D\lambda\mu+B\mu^2}{\Delta}.
$$

For every other point $a+t(b\times c)$, [orthogonality](orthogonal-vectors.md) gives squared distance $|a|^2+t^2|b\times c|^2$, proving the global minimum and its uniqueness. The positive [determinant](determinant.md) $\Delta=|b\times c|^2$ also proves that an intersection exists for every real $\lambda,\mu$. Parallel normals require a separate consistency check and do not define a unique intersection line.

## ↑ Ancestors (9)

1. [Distance from a point to a line in three dimensions](distance-from-a-point-to-a-line-in-three-dimensions.md)
2. [Distance from a point to a line](distance-from-a-point-to-a-line.md)
3. [Euclidean distance](euclidean-distance.md)
4. [Metric space](metric-space.md)
5. [Topological analysis](topological-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/14/d/solution.md)
