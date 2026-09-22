<h1 id="13c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the displayed integrand be $F$. Since it has no explicit dependence on $u$ or $v$, the [Euler-Lagrange equations for two fields](../../../../../../../euler-lagrange-equations-for-two-fields.md) are

$$
\partial_xF_{u_x}+\partial_yF_{u_y}=0,
\qquad
\partial_xF_{v_x}+\partial_yF_{v_y}=0.
$$

Its derivatives are

$$
F_{u_x}=(\lambda+2\mu)u_x+(\lambda+\mu)v_y,
\qquad F_{u_y}=\mu u_y,
$$



$$
F_{v_x}=\mu v_x,
\qquad F_{v_y}=(\lambda+2\mu)v_y+(\lambda+\mu)u_x.
$$

Thus

$$
(\lambda+2\mu)u_{xx}+\mu u_{yy}
+(\lambda+\mu)v_{xy}=0,
$$



$$
\mu v_{xx}+(\lambda+2\mu)v_{yy}
+(\lambda+\mu)u_{xy}=0.
$$

Using the [Laplacian](../../../../../../../laplacian.md), [gradient](../../../../../../../gradient.md), and [divergence](../../../../../../../divergence.md), these combine into the static [Navier-Cauchy equation](../../../../../../../navier-cauchy-equation.md)

$$
\boxed{\mu\nabla^2\mathbf u
+(\lambda+\mu)\nabla(\nabla\cdot\mathbf u)=0}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [13C](../../../13c.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
