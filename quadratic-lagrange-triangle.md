# Quadratic Lagrange triangle

↑ **Parent:** [Finite element](finite-element.md)

The [quadratic Lagrange triangle](quadratic-lagrange-triangle.md) uses degree-at-most-two [polynomials](polynomial-split.md) on a nondegenerate [triangle](triangle.md), with [point evaluation](point-evaluation-functional.md) at its three [polygon vertices](vertex-of-a-polygon.md) and three edge [midpoints](midpoint.md) as the six [finite element degrees of freedom](finite-element-degree-of-freedom.md). If $\lambda_i$ are the [affine functions](affine-function.md) of its [barycentric coordinate system](barycentric-coordinate-system.md), the cardinal shape functions are

$$
N_i=\lambda_i(2\lambda_i-1),\qquad N_{ij}=4\lambda_i\lambda_j\quad(i<j).
$$

At a [polygon vertex](vertex-of-a-polygon.md), one coordinate in the [barycentric coordinate system](barycentric-coordinate-system.md) is one and the others vanish; at an edge [midpoint](midpoint.md), two are $1/2$ and the third is zero. These values prove the cardinal property. Since $\dim\mathcal P_2(K)=6$, this is an [unisolvent finite element](unisolvent-finite-element.md). Matching the two endpoint values and [midpoint](midpoint.md) value on a shared [edge of a polygon](side-of-a-polygon.md) matches the whole quadratic restriction, producing a continuous global [conforming finite element space](conforming-finite-element-space.md).

## ↑ Ancestors (7)

1. [Finite element](finite-element.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/2/a/solution.md)
- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/2/d/solution.md)
- [Quadratic Lagrange triangle](quadratic-lagrange-triangle.md)
