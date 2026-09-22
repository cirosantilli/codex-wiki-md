<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Solving the $m$ unrelated shifted systems by separate [Gaussian elimination](../../../../../gaussian-elimination.md) costs $\boxed{\tfrac23m^4+O(m^3)}$ [floating-point operations](../../../../../floating-point-operation.md).

Instead compute $H=Q^TAQ$ once in $O(m^3)$ work. For each shift, solve

$$
(H-\lambda_jI)z_j=Q^Tb_j,\qquad x_j=Qz_j.
$$

The shift changes only the diagonal, so $H-\lambda_jI$ remains an [upper Hessenberg matrix](../../../../../upper-hessenberg-matrix.md). In each elimination column only the entry immediately below the pivot needs removal. With partial pivoting the only possible nonzero candidate rows are the current row and the next, and each update touches $O(m)$ entries. Factorization therefore costs $O(m^2)$ per shift; the triangular solve and both orthogonal-vector transformations also cost $O(m^2)$ each.

Thus $m$ shifted solves plus the initial [Hessenberg reduction](../../../../../hessenberg-reduction.md) cost $\boxed{O(m^3)}$ in total. Pivoting is still needed in general: nonsingularity excludes a singular system but does not by itself guarantee that every unpivoted elimination pivot is nonzero.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
