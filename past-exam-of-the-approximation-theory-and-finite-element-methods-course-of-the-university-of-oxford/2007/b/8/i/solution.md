<h1 id="b/8/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $V=\{v\in H^1(0,1):v(0)=0\}$ and its continuous piecewise [linear subspace](../../../../../vector-subspace.md) $V_h=\operatorname{span}\{\phi_1,\ldots,\phi_N\}$. The condition at $x=1$ is natural, so the last [hat function](../../../../../piecewise-linear-hat-function.md) remains free. Set $u_h^0$ to the $L^2$ [orthogonal projection](../../../../../orthogonal-projection.md) of $u_0$ onto $V_h$: the stated $L^2$ initial data need not have nodal values.

For each $m$, find $u_h^{m+1}\in V_h$ such that

$$
\boxed{\left(\frac{u_h^{m+1}-u_h^m}{\Delta t},v_h\right)
+((u_h^{m+1})',v_h')+(u_h^{m+1},v_h)=0\quad(v_h\in V_h).}
$$

This applies [Backward Euler method](../../../../../backward-euler-method.md) to diffusion and reaction together. The step [bilinear form](../../../../../bilinear-form-split.md) is coercive, so each step has a unique solution.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
