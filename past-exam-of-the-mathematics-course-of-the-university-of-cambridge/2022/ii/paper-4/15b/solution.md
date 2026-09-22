<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

The gravitational three-body [Lagrangian](../../../../../lagrangian.md) is

$$
L
=\frac12\sum_{i=1}^3m_i|\dot{\mathbf r}_i|^2
+G\left(
\frac{m_1m_2}{|\mathbf r_1-\mathbf r_2|}
+\frac{m_1m_3}{|\mathbf r_1-\mathbf r_3|}
+\frac{m_2m_3}{|\mathbf r_2-\mathbf r_3|}
\right).
$$

Put $M_{12}=m_1+m_2$ and $M=M_{12}+m_3$. Solving the definitions of the [Jacobi coordinates for three particles](../../../../../jacobi-coordinates-for-three-particles.md) gives

$$
\begin{aligned}
\mathbf r_1&=\mathbf c+\frac{m_3}{M}\mathbf b
+\frac{m_2}{M_{12}}\mathbf a,\\
\mathbf r_2&=\mathbf c+\frac{m_3}{M}\mathbf b
-\frac{m_1}{M_{12}}\mathbf a,\\
\mathbf r_3&=\mathbf c-\frac{M_{12}}M\mathbf b.
\end{aligned}
$$

Substitution into the kinetic energy makes all cross terms cancel:

$$
\boxed{
T
=\frac12\alpha|\dot{\mathbf a}|^2
+\frac12\beta|\dot{\mathbf b}|^2
+\frac12\gamma|\dot{\mathbf c}|^2
},
$$

where

$$
\boxed{
\alpha=\frac{m_1m_2}{m_1+m_2},
\qquad
\beta=\frac{(m_1+m_2)m_3}{m_1+m_2+m_3},
\qquad
\gamma=m_1+m_2+m_3
}.
$$

The pair separations are

$$
\mathbf r_1-\mathbf r_2=\mathbf a,
\qquad
\mathbf r_1-\mathbf r_3
=\mathbf b+\frac{m_2}{M_{12}}\mathbf a,
\qquad
\mathbf r_2-\mathbf r_3
=\mathbf b-\frac{m_1}{M_{12}}\mathbf a.
$$

Hence the [gravitational potential energy](../../../../../potential-energy.md) is

$$
V(\mathbf a,\mathbf b)
=-\frac{Gm_1m_2}{|\mathbf a|}
-\frac{Gm_1m_3}
{\left|\mathbf b+\frac{m_2}{M_{12}}\mathbf a\right|}
-\frac{Gm_2m_3}
{\left|\mathbf b-\frac{m_1}{M_{12}}\mathbf a\right|},
$$

which is independent of $\mathbf c$. Thus $\mathbf c$ is an [ignorable coordinate](../../../../../ignorable-coordinate.md) and

$$
\frac d{dt}(\gamma\dot{\mathbf c})=0,
\qquad
\boxed{\ddot{\mathbf c}=0}.
$$

The center of mass moves uniformly because the isolated system has no external force.

Finally, substituting the inverse coordinate transformation into

$$
\mathbf L=\sum_i m_i\mathbf r_i\times\dot{\mathbf r}_i
$$

again cancels every cross term and yields

$$
\boxed{
\mathbf L
=\alpha\mathbf a\times\dot{\mathbf a}
+\beta\mathbf b\times\dot{\mathbf b}
+\gamma\mathbf c\times\dot{\mathbf c}
}.
$$

This is the [angular momentum decomposition in three-body Jacobi coordinates](../../../../../angular-momentum-decomposition-in-three-body-jacobi-coordinates.md).

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
