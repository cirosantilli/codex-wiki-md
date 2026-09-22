<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the cylinder frame the wall moves at velocity $-U$. The [parabolic lubrication gap](../../../../../parabolic-lubrication-gap.md) and its natural stretched coordinate are

$$
h(x)=\frac{\epsilon a}{2}+\frac{x^2}{2a}
=\frac{\epsilon a}{2}(1+\xi^2),
\qquad
\xi=\frac{x}{a\sqrt\epsilon}.
$$

The wall values are $u(0)=-U$ and $u(h)=\Omega a$ to leading order. The [Couette-Poiseuille flow in a thin gap](../../../../../couette-poiseuille-flow-in-a-thin-gap.md) is therefore

$$
u(x,y)=-U+\frac{U+\Omega a}{h}y
+\frac{p_x}{2\mu}y(y-h),
$$

and its constant flux is

$$
q=\frac h2(\Omega a-U)-\frac{h^3}{12\mu}p_x.
$$

The [pressure recovery condition in lubrication flow](../../../../../pressure-recovery-condition-in-lubrication-flow.md) gives $\int_{-\infty}^{\infty}p_xdx=0$. Since

$$
\frac{\int h^{-2}dx}{\int h^{-3}dx}
=\frac{2\epsilon a}{3},
$$

it follows that

$$
\boxed{q=\frac13\epsilon a(\Omega a-U),}
\qquad
p_x=\frac{6\mu(\Omega a-U)}{h^2}-\frac{12\mu q}{h^3}.
$$

Differentiating the velocity profile gives the two surface shear stresses

$$
\boxed{
\left.\frac{\sigma_{xy}}\mu\right|_{y=0}
=\frac{4U-2\Omega a}{h}+\frac{6q}{h^2},
\qquad
\left.\frac{\sigma_{xy}}\mu\right|_{y=h}
=\frac{-2U+4\Omega a}{h}-\frac{6q}{h^2}.}
$$

Using $\int h^{-1}dx=2\pi/\sqrt\epsilon$ and $\int h^{-2}dx=2\pi/(a\epsilon^{3/2})$, the shear force exerted by the fluid on the wall is

$$
\boxed{F^{(s)}_{\rm wall}=\frac{4\pi\mu U}{\sqrt\epsilon},}
$$

and that exerted by the fluid on the cylinder is

$$
\boxed{F^{(s)}_{\rm cyl}=-\frac{4\pi\mu\Omega a}{\sqrt\epsilon}.}
$$

They are not equal and opposite because pressure acting on the sloping cylinder surface also transfers tangential momentum. Indeed, integration by parts gives the cylinder's pressure force

$$
F^{(p)}_{\rm cyl}=\int hp_x\,dx
=\frac{4\pi\mu(\Omega a-U)}{\sqrt\epsilon},
$$

so its total leading hydrodynamic force is $-4\pi\mu U/\sqrt\epsilon$.

The cylinder's excess weight per unit axial length is $\pi a^2\Delta\rho g$ in the falling direction, and it has no gravitational couple about its axis. Force and couple balance therefore give

$$
\boxed{U=\frac{a^2\Delta\rho g}{4\mu}\sqrt\epsilon,}
\qquad
\boxed{\Omega=0\quad\hbox{at leading order}.}
$$

The second result follows because the leading viscous couple is $-4\pi\mu\Omega a^2/\sqrt\epsilon$.

For $\Omega=0$, write $h=(\epsilon a/2)(1+\xi^2)$. Then

$$
p_x=\frac{2\mu U}{h^2}\frac{1-3\xi^2}{1+\xi^2},
\qquad
\sigma_{xy}(x,h)=\frac{2\mu U}{h}\frac{1-\xi^2}{1+\xi^2}.
$$

Thus $p$ is an odd pressure disturbance that vanishes at $x=0$ and at both infinities; its extrema occur at $\xi=\pm1/\sqrt3$. The cylinder shear is positive near the narrowest point, negative in the outer parts of the gap, and vanishes at

$$
\boxed{x=\pm a\sqrt\epsilon.}
$$

The [streamlines](../../../../../streamline.md) pass through the gap in the wall's direction overall. Pressure-driven backflow bends the interior streamlines and creates the two shear-reversal locations on the cylinder; the streamline sketch is symmetric under a half-turn combined with reversal of the flow direction.

For the final [Couette flow](../../../../../couette-flow.md), the lower and upper minimum gaps are $\epsilon a(1+\lambda)/2$ and $\epsilon a(1-\lambda)/2$. If the cylinder translates at speed $V$, the two leading lubrication drags are proportional to

$$
-\frac{U+V}{\sqrt{1+\lambda}}
\quad\hbox{and}\quad
\frac{U-V}{\sqrt{1-\lambda}}.
$$

The [force-free](../../../../../force-free.md) condition gives

$$
\boxed{
V=U\frac{\sqrt{1+\lambda}-\sqrt{1-\lambda}}
{\sqrt{1+\lambda}+\sqrt{1-\lambda}}
=\frac{\lambda U}{1+\sqrt{1-\lambda^2}}.}
$$

For $\lambda=0$, $V=0$ and the streamlines in the two equal gaps are mirror images with opposite directions. The $O(\mu U a)$ subleading wall-driven couple must balance the leading rotational resistance $O(\mu\Omega a^2/\sqrt\epsilon)$, so

$$
\boxed{\Omega=O(\epsilon^{1/2}U/a).}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
