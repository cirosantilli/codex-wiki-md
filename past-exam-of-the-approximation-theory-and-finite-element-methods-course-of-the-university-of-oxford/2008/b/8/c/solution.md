<h1 id="b/8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $u_h^m=\sum_iU_i^m\varphi_i$ and define the [mass matrix](../../../../../mass-matrix.md) and reaction-diffusion [stiffness matrix](../../../../../stiffness-matrix.md)

$$
M_{ij}=\int_0^1\varphi_i\varphi_j,\qquad
S_{ij}=\int_0^1(\varphi_i'\varphi_j'+e^x\varphi_i\varphi_j).
$$

Then each step is

$$
\boxed{AU^{m+1}=(M/\Delta t-S/2)U^m,\qquad
A=M/\Delta t+S/2.}
$$

Both component matrices are symmetric, so $A$ is symmetric. For a nonzero coefficient vector $v$, its [finite element](../../../../../finite-element.md) [function](../../../../../function-split.md) $v_h$ is nonzero and

$$
v^TAv=\Delta t^{-1}\|v_h\|_2^2+\tfrac12a(v_h,v_h)>0.
$$

Thus $A$ is also positive definite and every update has a unique solution. Because nonneighboring hats have disjoint interior supports, the matrix is tridiagonal in nodal order.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
