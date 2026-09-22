<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $X=x-x_{L_3}$ and $Y=y$ be the displacement from the [L3 Lagrange point](../../../../../../l3-lagrange-point.md), and put $U=\dot X$, $W=\dot Y$. The first-order [linearization of a dynamical system](../../../../../../linearization-of-a-dynamical-system.md) is

$$
\ddot X-2\dot Y=F_xX+F_yY,
\qquad
\ddot Y+2\dot X=G_xX+G_yY,
$$

where every derivative is evaluated at $L_3$. For the [state vector](../../../../../../state-vector.md) $\boldsymbol\xi=(X,Y,U,W)^{\mathsf T}$, this becomes

$$
\boxed{
\dot{\boldsymbol\xi}=A\boldsymbol\xi,
\qquad
A=
\begin{pmatrix}
0&0&1&0\\
0&0&0&1\\
F_x&F_y&0&2\\
G_x&G_y&-2&0
\end{pmatrix}_{L_3}}.
$$

The question's reuse of $\mathbf X$ for the state vector is only notation; its first two entries are the small displacements $X,Y$, not the absolute coordinates.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
