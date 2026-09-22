<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

Work per unit axial length, with $y$ vertically upward and $x$ across the thin gap. In the frame of the downward-translating cylinder, the wall moves upward at speed $U$ and the cylinder surface is stationary. Let $\eta$ be [viscosity](../../../../../dynamic-viscosity.md) and use the leading [lubrication theory](../../../../../lubrication-theory.md)

$$
h(y)=h_0+\frac{y^2}{2a},\qquad h_0\ll a.
$$

The transverse [pressure](../../../../../pressure.md) [gradient](../../../../../gradient.md) is negligible; solving $\eta u_{xx}=p_y$ with $u(0)=U$, $u(h)=0$ gives

$$
u(x,y)=U\left(1-\frac xh\right)+\frac{p_y}{2\eta}x(x-h),\qquad
q=\int_0^h u\,dx=\frac{Uh}2-\frac{h^3p_y}{12\eta}.
$$

The flux $q$ is constant by [incompressibility](../../../../../incompressible-flow.md). Equal ambient [pressure](../../../../../pressure.md) at both ends implies $\int p_y\,dy=0$. With $I_j=\int_{-\infty}^{\infty}h^{-j}\,dy$ and $I_2/I_3=4h_0/3$, this yields

$$
q=\frac{2Uh_0}3,\qquad p_y=\frac{6\eta U}{h^2}-\frac{8\eta Uh_0}{h^3},\qquad
\boxed{p(y)=-\frac{2\eta Uy}{h(y)^2}.}
$$

The tangential traction on the cylinder is

$$
\tau=-\eta u_x(h)=-\frac{2\eta U}h+\frac{4\eta Uh_0}{h^2}.
$$

Since $I_2=I_1/(2h_0)$, its integrated force is $-2\eta UI_1+4\eta Uh_0I_2=0$. [Pressure](../../../../../pressure.md) acts radially on a circular cylinder and contributes no torque; the tangential traction has moment arm $a$ to leading order. Hence

$$
\boxed{F_{\rm tangential}=0,\qquad\text{torque}=0\quad\text{to leading lubrication order}.}
$$

For clarity, the total vertical hydrodynamic force is not zero. Its leading [pressure](../../../../../pressure.md) contribution is

$$
F_{\rm drag}=-\int p h'\,dy=\boxed{2\pi\eta U\sqrt{\frac{2a}{h_0}}}
$$

upward, while the leading shear contribution just calculated vanishes. Thus **this model predicts no induced rolling direction**: a freely rotating cylinder can remain nonrotating, rather than rolling like a wheel in contact with the wall. This is the [torque-free cylinder in a lubrication gap](../../../../../torque-free-cylinder-in-a-lubrication-gap.md) cancellation; finite ends or different boundary conditions would require a different model.

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
