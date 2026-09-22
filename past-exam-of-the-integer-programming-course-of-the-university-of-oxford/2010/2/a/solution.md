<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [totally unimodular matrix](../../../../totally-unimodular-matrix.md) has the property that every square submatrix has [determinant](../../../../determinant.md) zero, one or minus one. This includes the one-by-one submatrices, so every entry belongs to $\{0,1,-1\}$.

Its importance is integrality of linear-programming vertices: if $A$ is totally unimodular and $b$ is integral, every vertex of $\{x:Ax\leq b,\ x\geq0\}$ is integral. Adding rows of the identity preserves total unimodularity. A nonsingular active basis therefore has [determinant](../../../../determinant.md) $\pm1$ and an [integer](../../../../integer-split.md) inverse by the [cofactor](../../../../cofactor.md) formula, making its basic solution integral. Thus a finite optimum attained at a vertex of the [linear programming relaxation](../../../../linear-programming-relaxation.md) gives an [integer](../../../../integer-split.md) optimum without branching.

One sufficient condition is: **entries belong to $\{0,1,-1\}$, each column has at most two nonzero entries, and any column with two has one $+1$ and one $-1$.** This is the [signed column condition for total unimodularity](../../../../signed-column-condition-for-total-unimodularity.md), satisfied by directed vertex-edge incidence matrices. It is sufficient, not necessary.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
