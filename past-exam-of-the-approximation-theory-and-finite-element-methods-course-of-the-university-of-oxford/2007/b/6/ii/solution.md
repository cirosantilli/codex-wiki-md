<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $V=\{v\in H^1(\Omega):v=0\text{ on }\Gamma_D\}$, with boundary values interpreted as traces. The outward [unit normal](../../../../../unit-normal.md) on $\Gamma_N$ is $(-1,-1)/\sqrt2$, so the stated [derivative](../../../../../derivative.md) condition is precisely $\partial_nu=0$. [integration by parts](../../../../../integration-by-parts.md) gives

$$
u\in V,\qquad \int_\Omega\nabla u\cdot\nabla v\,dx\,dy=\int_\Omega v\,dx\,dy\quad(v\in V).
$$

The Dirichlet boundary has positive length, so the [Poincaré inequality](../../../../../poincare-inequality.md) makes the form coercive. Let $V_h\subset V$ be the continuous piecewise affine space on the four triangles. The [finite element](../../../../../finite-element.md) approximation satisfies the same identity for every $v_h\in V_h$.

Nodes $A,C,D,E,F$ have zero values, leaving $V_h=\operatorname{span}\{\phi_B\}$. Although isolated endpoints have zero boundary measure, continuity along the Dirichlet edges forces the nodal values at $A$ and $C$ to vanish.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
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
