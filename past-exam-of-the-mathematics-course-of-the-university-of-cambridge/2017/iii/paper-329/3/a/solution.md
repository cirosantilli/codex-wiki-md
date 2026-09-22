<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First supply the introductory scaling and geometry. The leading tangential [Stokes equation](../../../../../../stokes-equation.md) in a thin gap balances $P/L$ against $\mu U/H^2$. The [shear stress](../../../../../../shear-stress.md) scale is $\tau\sim\mu U/H$, so [lubrication pressure dominates shear stress](../../../../../../lubrication-pressure-dominates-shear-stress.md):

$$
\boxed{P\sim\frac{\mu UL}{H^2},\qquad \frac\tau P\sim\frac HL\ll1.}
$$

The outer circle, viewed along a ray $r(\cos\theta,\sin\theta)$ from the inner centre, satisfies $r^2-2\alpha\Delta r\sin\theta+\alpha^2\Delta^2=(a+\Delta)^2$. Expanding its positive root to first order in $\Delta/a$ gives $r=a+\Delta+\alpha\Delta\sin\theta+O(\Delta^2/a)$, hence $h=\Delta(1+\alpha\sin\theta)$.

Take positive $\Omega$ to mean increasing $\theta$, and put $s=a\theta$, $y=r-a$, $U=\Omega a$. With [no-slip boundary conditions](../../../../../../no-slip-boundary-condition.md) at $y=0,h$, [lubrication theory](../../../../../../lubrication-theory.md) gives

$$
u_\theta=U\left(1-\frac yh\right)+\frac{p_s}{2\mu}y(y-h),\qquad
q=\frac{Uh}{2}-\frac{h^3}{12\mu}p_s.
$$

Steady [mass conservation](../../../../../../mass-conservation.md) makes $q$ independent of $\theta$. Single-valued [pressure](../../../../../../pressure.md) requires $\int_0^{2\pi}p_\theta\,d\theta=0$. Write $I_n=\int_0^{2\pi}(1+\alpha\sin\theta)^{-n}d\theta$ and $D_\alpha=1+\alpha^2/2$. It follows that

$$
\boxed{q=\frac{\Omega a\Delta}{2}\frac{I_2}{I_3}
=\frac{\Omega a\Delta}{2}\frac{1-\alpha^2}{D_\alpha},\qquad
p_s=\frac{6\mu\Omega a}{h^2}-\frac{12\mu q}{h^3}.}
$$

The tangential fluid tractions on the inner and outer solids, measured in the same increasing-$\theta$ direction, are respectively

$$
\boxed{\tau_i=\mu u_{\theta,y}(0)=\frac{6\mu q}{h^2}-\frac{4\mu\Omega a}{h},\qquad
\tau_o=-\mu u_{\theta,y}(h)=\frac{6\mu q}{h^2}-\frac{2\mu\Omega a}{h}.}
$$

This sign convention distinguishes the traction on a wall from the corresponding stress component in the fluid.

To leading order the holding [force](../../../../../../force.md) balances the [pressure](../../../../../../pressure.md) traction on the inner circle. [Integration by parts](../../../../../../integration-by-parts.md) gives

$$
F_x=a\int_0^{2\pi}p\cos\theta\,d\theta
=-a\int_0^{2\pi}p_\theta\sin\theta\,d\theta.
$$

Use $p_\theta=a p_s$ and $\int\sin\theta/(1+\alpha\sin\theta)^n\,d\theta=(I_{n-1}-I_n)/\alpha$, with the continuous limit at $\alpha=0$. Substituting the boxed flux yields

$$
\boxed{F_x=-\frac{6\pi\mu\Omega a^3}{\Delta^2}\frac{\alpha}{\sqrt{1-\alpha^2}\,D_\alpha},\qquad F_z=0.}
$$

The zero vertical component also follows from [reflection in mathematics](../../../../../../reflection-mathematics.md) in the vertical line: this leaves the geometry and vertical [force](../../../../../../force.md) unchanged, reverses $\Omega$, and [Linearity of Stokes flow](../../../../../../linearity-of-stokes-flow.md) then requires $F_z=0$.

[Pressure](../../../../../../pressure.md) gives no moment about either circular wall's own centre. Integrating the [viscous shear torque](../../../../../../viscous-shear-torque.md) with lever arm $a$ to leading order gives the fluid couples

$$
\boxed{C_i=-\frac{2\pi\mu\Omega a^3}{\Delta\sqrt{1-\alpha^2}}\frac{1+2\alpha^2}{D_\alpha},\qquad
C_o=\frac{2\pi\mu\Omega a^3\sqrt{1-\alpha^2}}{\Delta D_\alpha}.}
$$

Indeed $C_i=a^2\int\tau_i d\theta$ and $C_o=a^2\int\tau_o d\theta$ at this order. Applied holding or driving couples are the negatives of these fluid couples. They need not cancel because they are moments about different axes. The fluid [force](../../../../../../force.md) on the outer solid equals the holding [force](../../../../../../force.md) $F_x$ on the inner one. Transferring its moment to the inner axis adds $-\alpha\Delta F_x$, so [angular momentum](../../../../../../angular-momentum.md) balance about a common axis is

$$
\boxed{C_i+C_o=\alpha\Delta F_x.}
$$

For $\alpha=0$ the usual equal and opposite concentric couples are recovered. All these formulas are leading thin-gap expressions at fixed $|\alpha|<1$; taking the contact limit requires maintaining the local slender-gap assumptions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
