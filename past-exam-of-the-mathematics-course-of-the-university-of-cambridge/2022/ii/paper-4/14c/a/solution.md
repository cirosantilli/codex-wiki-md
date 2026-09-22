<h1 id="14c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
M=\begin{pmatrix}f_u&f_v\\g_u&g_v\end{pmatrix}
$$

be the reaction Jacobian at the homogeneous equilibrium. Stability without diffusion gives

$$
f_u+g_v<0,
\qquad
J=\det M=f_ug_v-f_vg_u>0.
$$

For a spatial Fourier mode with $-\nabla^2$ eigenvalue $k^2$, the linearized matrix is

$$
M-k^2\begin{pmatrix}D_u&0\\0&D_v\end{pmatrix}.
$$

Its trace is even more negative than $\operatorname{tr}M$, so instability occurs exactly when its determinant becomes negative. Put $z=D_vk^2$ and $d=D_u/D_v$. Then

$$
\Delta(z)
=J-(f_u+dg_v)z+dz^2.
$$

This upward-opening quadratic is negative for some $z>0$ exactly when its minimum occurs at positive $z$ and lies below zero:

$$
f_u+dg_v>0,
\qquad
J-\frac{(f_u+dg_v)^2}{4d}<0.
$$

The second strict inequality implies the first when written with a positive square root, so the [two-species diffusion-driven instability criterion](../../../../../../two-species-diffusion-driven-instability-criterion.md) becomes

$$
\boxed{f_u+dg_v>2\sqrt{dJ}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14C](../../14c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
