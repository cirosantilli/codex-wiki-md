# Linear-spline mixed Gram matrix

↑ **Parent:** [Mixed-normalization spline Gram matrix](mixed-normalization-spline-gram-matrix.md)

For the distinct-knot linear [B-spline](b-spline.md) hats, let $h_i=t_{i+1}-t_i>0$. The [mixed-normalization spline Gram matrix](mixed-normalization-spline-gram-matrix.md) has entries

$$
g_{ii}=\frac23,\quad g_{i,i-1}=\frac{h_i}{3(h_i+h_{i+1})},\quad g_{i,i+1}=\frac{h_{i+1}}{3(h_i+h_{i+1})},\quad g_{ij}=0\quad(|i-j|\ge2).
$$

Only indices in the finite [basis](basis.md) are retained. This [matrix](matrix.md) has a row [strict diagonal dominance](strictly-diagonally-dominant-matrix.md) margin at least $1/3$, so the [inverse infinity-norm bound from diagonal dominance](inverse-infinity-norm-bound-from-diagonal-dominance.md) gives $\|G^{-1}\|_{\ell^\infty}\le3$. Equidistant [spline knots](spline-knot.md) give off-diagonal entries $1/6$. Both pieces of every hat are retained; repeated endpoint [spline knots](spline-knot.md) require different boundary formulas.

## ↑ Ancestors (9)

1. [Mixed-normalization spline Gram matrix](mixed-normalization-spline-gram-matrix.md)
2. [B-spline](b-spline.md)
3. [Spline approximation](spline-approximation.md)
4. [Spline (mathematics)](spline-mathematics.md)
5. [Uniform approximation](uniform-approximation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-69/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/5/c/solution.md)
