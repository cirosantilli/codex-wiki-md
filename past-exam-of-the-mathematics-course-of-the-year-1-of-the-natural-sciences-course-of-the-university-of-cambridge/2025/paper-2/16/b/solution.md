<h1 id="16/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\mathbf W=\nabla\times\mathbf F$ and $\mathbf v=\dot{\mathbf r}$. All [vector fields](../../../../../vector-field.md) and their spatial [partial derivatives](../../../../../partial-derivative.md) below are evaluated at $\mathbf r(t)$. The [product rule](../../../../../product-rule.md) for a [dot product](../../../../../dot-product.md) gives

$$
\frac d{dt}\bigl(\mathbf W(\mathbf r(t))\cdot\dot{\mathbf r}(t)\bigr)
=\frac{d\mathbf W(\mathbf r(t))}{dt}\cdot\dot{\mathbf r}(t)
+\mathbf W(\mathbf r(t))\cdot\ddot{\mathbf r}(t).
$$

Because the [vector field](../../../../../vector-field.md) has no explicit time dependence, the [multivariable chain rule](../../../../../multivariable-chain-rule.md) gives $d\mathbf W/dt=J_{\mathbf W}\dot{\mathbf r}$, where the [Jacobian matrix](../../../../../jacobian-matrix.md) has entries $(J_{\mathbf W})_{ij}=\partial_jW_i$. Consequently

$$
\boxed{\frac d{dt}\left[(\nabla\times\mathbf F)\cdot\dot{\mathbf r}\right]
=\dot{\mathbf r}^{\,T}J_{\nabla\times\mathbf F}\dot{\mathbf r}
+(\nabla\times\mathbf F)\cdot\ddot{\mathbf r}}.
$$

The first term measures the change of the [curl](../../../../../curl.md) sampled as the point moves; the second measures the change in the [velocity vector](../../../../../velocity-vector.md) used in the [dot product](../../../../../dot-product.md).

To give the result explicitly in $P,Q,R$, define the [directional derivative](../../../../../directional-derivative.md) operator $L=\dot x\partial_x+\dot y\partial_y+\dot z\partial_z$. Since

$$
\mathbf W=(R_y-Q_z,\ P_z-R_x,\ Q_x-P_y)^T,
$$

the same expression is

$$
\begin{aligned}
&\dot x\,L(R_y-Q_z)+\dot y\,L(P_z-R_x)+\dot z\,L(Q_x-P_y)\\
&\quad+\ddot x(R_y-Q_z)+\ddot y(P_z-R_x)+\ddot z(Q_x-P_y).
\end{aligned}
$$

For example $L(R_y-Q_z)=\dot x(R_{yx}-Q_{zx})+\dot y(R_{yy}-Q_{zy})+\dot z(R_{yz}-Q_{zz})$; the other two terms expand in the same way. Thus only the first and second spatial [partial derivatives](../../../../../partial-derivative.md) of $P,Q,R$, together with the [velocity](../../../../../velocity.md) and [acceleration](../../../../../acceleration.md) of the [parametric curve](../../../../../parametric-curve.md), occur.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [16](../../16.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
