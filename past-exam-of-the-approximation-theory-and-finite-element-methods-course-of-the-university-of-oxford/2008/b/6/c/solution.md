<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $V_h$ to be all continuous [functions](../../../../../function-split.md) affine on each triangle of the stated negative-diagonal [mesh](../../../../../finite-element-mesh.md). No boundary value is fixed, because the Neumann condition is natural. The discrete problem is

$$
\boxed{u_h\in V_h,\qquad a(u_h,v_h)=\ell(v_h)\quad(v_h\in V_h).}
$$

Its matrix is symmetric positive definite: the reaction contribution $\int u_hv_h$ removes the constant null mode that would occur for pure Neumann Poisson equations. Thus the solution exists uniquely.

For every $v_h\in V_h$, expand the [quadratic functional](../../../../../quadratic-functional.md) about $u_h$ and use the discrete weak equation to remove its linear term:

$$
J(v_h)=J(u_h)+\tfrac12a(v_h-u_h,v_h-u_h)\geq J(u_h).
$$

The continuous solution minimizes $J$ over the larger space $H^1$, so

$$
\boxed{J(u)\leq J(u_h)\leq J(v_h).}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
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
