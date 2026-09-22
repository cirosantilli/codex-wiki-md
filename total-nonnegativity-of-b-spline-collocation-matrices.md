# Total nonnegativity of B-spline collocation matrices

↑ **Parent:** [B-spline collocation matrix](b-spline-collocation-matrix.md)

For increasing sites and an ordered nonnegative normalized [B-spline](b-spline.md) basis, the [matrix](matrix.md) $A_{ij}=N_j(x_i)$ is a [totally nonnegative matrix](total-nonnegativity-of-a-matrix.md). One way to see the minors' signs is [knot insertion](knot-insertion.md). Each inserted knot changes coefficients by $b_j=\alpha_j a_j+(1-\alpha_j)a_{j-1}$ with $0\leq\alpha_j\leq1$, using the standard constant endpoint pieces. This is a nonnegative rectangular bidiagonal map, whose minors are nonnegative. Products preserve that property by the [Cauchy–Binet formula](cauchy-binet-formula.md). Insert each site to full knot multiplicity; a suitable refined coefficient is then the value $s(x_i)$. Thus collocation is an ordered row submatrix of the refinement map, and has nonnegative minors. The strict support conditions $t_i<x_i<t_{i+k}$ give invertibility by the [Schoenberg–Whitney theorem](schoenberg-whitney-theorem.md); its inverse has the [checkerboard inverse of a totally nonnegative matrix](checkerboard-inverse-of-a-totally-nonnegative-matrix.md) sign pattern.

## ↑ Ancestors (9)

1. [B-spline collocation matrix](b-spline-collocation-matrix.md)
2. [B-spline](b-spline.md)
3. [Spline approximation](spline-approximation.md)
4. [Spline (mathematics)](spline-mathematics.md)
5. [Uniform approximation](uniform-approximation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/5/a/solution.md)
