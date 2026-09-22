# Isoparametric finite element

↑ **Parent:** [Finite element](finite-element.md)

An isoparametric [finite element](finite-element.md) uses the same reference [shape functions](shape-function.md) to interpolate its geometry and its unknown field. With reference functions $N_i$ and physical nodes $\mathbf x_i$, the geometry map is $F=\sum_i\mathbf x_iN_i$ and the physical functions are $N_i\circ F^{-1}$. The map must be one-to-one and have a nonvanishing [Jacobian determinant](jacobian-determinant.md). For bilinear quadrilaterals, compatible common edges have affine geometry maps and identical linear field traces, giving a continuous [conforming finite element space](conforming-finite-element-space.md). On a general quadrilateral the pulled-back functions need not be [polynomials](polynomial-split.md) in physical coordinates.

## ↑ Ancestors (7)

1. [Finite element](finite-element.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford/2010/b/6/solution.md)
