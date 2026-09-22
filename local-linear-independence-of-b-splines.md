# Local linear independence of B-splines

↑ **Parent:** [B-spline](b-spline.md)

The $k$ order-$k$ [B-splines](b-spline.md) active on a simple-knot cell form a [basis](basis.md) of its degree-$k-1$ [polynomials](polynomial-split.md). To see this from [Marsden's identity](marsden-identity.md), use the dual [polynomials](polynomial-split.md) $\psi_i(y)=\prod_{\ell=1}^{k-1}(y-t_{i+\ell})$. On $t_j<x<t_{j+1}$ the identity is $(y-x)^{k-1}=\sum_{i=j-k+1}^jN_i(x)\psi_i(y)$. Evaluation of the dual [polynomials](polynomial-split.md) at $t_j,t_{j-1},\ldots,t_{j-k+1}$ gives a triangular [coefficient](coefficient.md) [matrix](matrix.md) with nonzero diagonal. They are independent, and comparison of [coefficients](coefficient.md) of $y$ in the identity gives independence of the active [splines](spline-mathematics.md). Consequently a [spline](spline-mathematics.md) vanishes on a whole open cell exactly when all its active [coefficients](coefficient.md) vanish.

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
