<h1 id="5f/solution">Solution</h1>

↑ **Parent:** [5F](../5f.md)

A real [harmonic function](../../../../../harmonic-function.md) on a planar open set is a twice continuously differentiable function satisfying $f_{xx}+f_{yy}=0$. The ordered pair $(f,g)$ consists of [harmonic conjugates](../../../../../harmonic-conjugate.md) when $f+ig$ is holomorphic; the corresponding [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) are $f_x=g_y$ and $f_y=-g_x$.

To prove [composition of harmonic conjugate pairs](../../../../../composition-of-harmonic-conjugate-pairs.md), denote $P=p(u,v)$ and $Q=q(u,v)$, and assume the inner pair's image lies in the outer pair's domain. Their equations are $u_x=v_y$, $u_y=-v_x$, $p_u=q_v$ and $p_v=-q_u$. The [chain rule](../../../../../chain-rule.md) gives

$$
P_x=p_uu_x+p_vv_x=p_uu_x-q_uv_x=Q_y,
$$



$$
P_y=p_uu_y+p_vv_y=-p_uv_x-q_uu_x=-Q_x.
$$

Thus the composite satisfies the Cauchy-Riemann equations. Its components are $C^2$, and differentiating gives $P_{xx}+P_{yy}=Q_{yx}-Q_{xy}=0$ and similarly $Q_{xx}+Q_{yy}=0$. **The composite pair is harmonic conjugate**, including when the inner map has a critical point.

## ↑ Ancestors (10)

1. [5F](../5f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
