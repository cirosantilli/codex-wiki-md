# Bilinear square finite element

↑ **Parent:** [Finite element](finite-element.md)

A bilinear square [finite element](finite-element.md) uses [polynomials](polynomial-split.md) of degree at most one separately in each coordinate and takes values at the four corners as degrees of freedom. On the unit square its nodal [shape functions](shape-function.md) are $(1-\xi)(1-\eta)$, $\xi(1-\eta)$, $\xi\eta$, and $(1-\xi)\eta$, in anticlockwise corner order. Each is a [tensor product](tensor-product.md) of one-dimensional linear [shape functions](shape-function.md). A function in this space need not be affine, since $\xi\eta$ has total degree two. On a physical square of side $h$, its Laplacian [stiffness matrix](stiffness-matrix.md) has diagonal entries $2/3$, adjacent-corner entries $-1/6$ and opposite-corner entries $-1/3$. Its [Robin boundary condition](robin-boundary-condition.md) edge matrix has the two-node block $(h/6)\begin{pmatrix}2&1\\1&2\end{pmatrix}$ for a unit boundary coefficient.

## ↑ Ancestors (7)

1. [Finite element](finite-element.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford/2010/b/6/solution.md)
- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2011/1/solution.md)
- [Shape function](shape-function.md)
