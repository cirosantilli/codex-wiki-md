<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Continue the expansion established in part (b), with $p=\epsilon^2p_2+\cdots$ after removal of the background [pressure](../../../../../../pressure.md). The radial [momentum](../../../../../../momentum.md) equation at order $\epsilon^2$ gives

$$
p_{2y}=-D u_0v_{1x}=D\frac{u_0^2}{r}A_{xx}.
$$

Integrating across the core, then differentiating in $x$, gives

$$
p_{2x}(1)-p_{2x}(0)=\sigma A_{xxx},\qquad\sigma=D\int_0^1\frac{u_0^2}{R+y}\,dy.
$$

This is the dispersive contribution from transverse inertia.

At second order the axial [momentum](../../../../../../momentum.md) equation is

$$
u_0u_{2x}+v_2u_0'=-p_{2x}-\beta u_{1t}-u_1u_{1x}-v_1u_{1y}.
$$

For the [displacement](../../../../../../displacement.md) fields just obtained,

$$
u_1u_{1x}+v_1u_{1y}=AA_x\left[\frac{(u_0')^2-u_0u_0''}{r^2}+\frac{u_0u_0'}{r^3}\right].
$$

Use $u_0=0$ on each wall. The lower and upper regular core limits respectively give

$$
\begin{aligned}
p_{2x}(0)&=-\gamma_0v_2(0)-\beta\frac{\gamma_0}{R}A_t-\frac{\gamma_0^2}{R^2}AA_x,\\
p_{2x}(1)&=\beta\frac{\gamma_1}{R+1}A_t-\frac{\gamma_1^2}{(R+1)^2}AA_x,
\end{aligned}
$$

where $v_2(1)=0$ at the fixed outer wall.

At the moving inner wall $y=\epsilon F$, no penetration requires $v=\epsilon\lambda St F_t+\epsilon uF_x$. Expanding about $y=0$, the axial edge [velocity](../../../../../../velocity.md) is $\epsilon\gamma_0(F+A/R)+O(\epsilon^2)$ and $v_{1y}(0)=-\gamma_0A_x/R$. Thus

$$
\epsilon^2\left[v_2(0)-\frac{\gamma_0}{R}FA_x\right]=\epsilon^2\left[\beta F_t+\gamma_0(F+A/R)F_x\right]+o(\epsilon^2),
$$

or

$$
v_2(0)=\beta F_t+\gamma_0FF_x+\frac{\gamma_0}{R}(AF)_x.
$$

The thin wall layers do not change this normal-flux condition at the retained order, because their flux correction is $o(\epsilon^2)$.

Subtract the two axial pressure-gradient limits and use the radial-pressure difference. With $\alpha_1=\gamma_0/R+\gamma_1/(R+1)$ and $\alpha_2=\gamma_0^2/R^2-\gamma_1^2/(R+1)^2$, the result is the [forced annular displacement equation](../../../../../../forced-annular-displacement-equation.md)

$$
\boxed{\sigma A_{xxx}-\beta\alpha_1A_t-\alpha_2AA_x=\beta\gamma_0F_t+\gamma_0^2FF_x+\frac{\gamma_0^2}{R}(AF)_x}.
$$

Every coefficient follows from the given profile and wall slopes; no explicit base-flow solution has been used. The derivation is conditional on the regular core limits and wall layers remaining asymptotically thin.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
