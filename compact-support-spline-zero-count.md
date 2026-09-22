# Compact-support spline zero count

↑ **Parent:** [B-spline](b-spline.md)

Let the real [spline](spline-mathematics.md) $s=\sum_{i=p}^qc_iN_i$ have distinct knots, order $k\ge2$, nonzero endpoint [coefficients](coefficient.md), and no identically zero knot cell in its [support](support.md). It and its first $k-2$ [derivatives](derivative.md) vanish at both [support](support.md) endpoints. If $Z$ is its number of interior distinct zeros, there are initially $Z+2$ zero components. Each differentiation through order $k-2$ increases this count by at least one: a nonzero gap between zero components has an interior extremum, and the two endpoint zeros remain separate. The final [derivative](derivative.md) is continuous piecewise linear on $q-p+k$ cells, and each cell can meet at most one zero component unless it is identically zero, in which case all its zeros belong to the same component. It therefore has at most $q-p+k$ zero components. Thus $Z+k\le q-p+k$, proving the bound.

## ↑ Ancestors (8)

1. [B-spline](b-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/7/solution.md)
