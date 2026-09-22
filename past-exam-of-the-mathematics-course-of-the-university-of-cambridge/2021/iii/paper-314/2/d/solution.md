<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The pressure jump relation with $p_2/p_1=1+\epsilon$ gives

$$
M_{x1}^2=1+\frac{\gamma+1}{2\gamma}\epsilon.
$$

If $\beta_1$ is the angle between the upstream velocity and the shock front, then $M_{x1}=M_1\sin\beta_1$. To leading order,

$$
\boxed{\beta_1\simeq\beta_2\simeq
\arcsin(M_1^{-1})},
$$

the [Mach angle](../../../../../../mach-angle.md). Expansion of the compression ratio gives

$$
\frac{\rho_2}{\rho_1}=1+\frac\epsilon\gamma+O(\epsilon^2).
$$

Because $u_y$ is continuous and $\tan\beta=u_x/u_y$,

$$
\boxed{\frac{\tan\beta_1}{\tan\beta_2}
=\frac{u_{x1}}{u_{x2}}
=1+\frac\epsilon\gamma+O(\epsilon^2)}.
$$

Writing $\theta=\beta_1-\beta_2$ and linearizing the tangent about $\sin\beta_1=1/M_1$ gives the [weak-oblique-shock deflection](../../../../../../weak-oblique-shock-deflection.md)

$$
\boxed{\theta\simeq
\frac\epsilon\gamma\sin\beta_1\cos\beta_1
=\frac{\epsilon\sqrt{M_1^2-1}}{\gamma M_1^2}}.
$$

The normal component decreases while the tangential component is unchanged, so $\beta_2<\beta_1$: the flow turns toward the shock front.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
