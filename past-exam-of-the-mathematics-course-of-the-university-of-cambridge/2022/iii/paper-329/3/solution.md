<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [nearly occluding sphere in a cylindrical tube](../../../../../nearly-occluding-sphere-in-a-cylindrical-tube.md) has gap thickness $H=O(\epsilon a)$ and axial length $L=O(\sqrt{aH})=O(a\sqrt\epsilon)$. In the gap, [lubrication theory](../../../../../lubrication-theory.md) therefore gives

$$
p_x=O\left(\frac{\mu U}{\epsilon^2a^2}\right),
\qquad
p=O\left(\frac{\mu U}{a\epsilon^{3/2}}\right),
\qquad
\sigma_{xy}=O\left(\frac{\mu U}{\epsilon a}\right).
$$

Far ahead of and behind the sphere, the length and width scales are both $a$, so

$$
p_x=O\left(\frac{\mu U}{a^2}\right),
\qquad
\sigma_{rx}=O\left(\frac{\mu U}{a}\right).
$$

In the sphere frame the tube wall at $y=0$ moves with velocity $-U$ and the sphere surface at $y=h$ is stationary. The local [Couette-Poiseuille flow in a thin gap](../../../../../couette-poiseuille-flow-in-a-thin-gap.md) is

$$
u=-U+\frac Uh y+\frac{p_x}{2\mu}y(y-h).
$$

Its axial [volume flux](../../../../../volumetric-flow-rate.md) per unit circumferential width is

$$
\boxed{q=-\frac{h^3}{12\mu}p_x-\frac{Uh}{2}.}
$$

Differentiating the profile and eliminating $p_x$ gives the two wall stresses

$$
\boxed{
\left.\frac{\sigma_{xy}}\mu\right|_{y=0}
=\frac{4U}{h}+\frac{6q}{h^2},
\qquad
\left.\frac{\sigma_{xy}}\mu\right|_{y=h}
=-\frac{2U}{h}-\frac{6q}{h^2}.}
$$

The [continuity equation](../../../../../continuity-equation.md) integrated across the gap says that changes of $q$ along $x$ are balanced by circumferential flux divergence. Circumferential variations occur on scale $a$, much longer than the axial scale $a\sqrt\epsilon$, so $q=q(\theta)$ is independent of $x$ at leading order.

Put $h=h_0(1+\xi^2)$ with $x=\sqrt{2ah_0}\,\xi$. The leading $O(\epsilon^{-3/2})$ pressure jump must vanish in the global balance from part ii. Equivalently, the [pressure recovery condition in lubrication flow](../../../../../pressure-recovery-condition-in-lubrication-flow.md) gives

$$
0=\int_{-\infty}^{\infty}p_x\,dx
=-12\mu q\int h^{-3}\,dx-6\mu U\int h^{-2}\,dx.
$$

Using $I_2=\pi/2$ and $I_3=3\pi/8$,

$$
\frac{\int h^{-2}dx}{\int h^{-3}dx}=\frac43h_0,
\qquad
\boxed{q=-\frac23Uh_0(\theta).}
$$

The total flux through the gap is consequently

$$
Q=a\int_0^{2\pi}q\,d\theta
=-\frac43\pi\epsilon Ua^2.
$$

Far from the sphere, translation of the tube contributes $-\pi a^2U$, while [Hagen-Poiseuille flow](../../../../../hagen-poiseuille-equation.md) contributes $\pi a^4p_x/(8\mu)$. Equating these fluxes gives

$$
\boxed{p_x\sim\frac{8\mu U}{a^2}\left(1-\frac43\epsilon\right).}
$$

At the next order, substitute $q=-2Uh_0/3$ into the tube-wall shear and integrate through the gap:

$$
\int_{-\infty}^{\infty}\sigma_{xy}(x,0)\,dx
=4\mu U\int\left(\frac1h-\frac{h_0}{h^2}\right)dx
=2\pi\mu U\sqrt{\frac{2a}{h_0}}.
$$

The balance in part ii then gives the leading pressure drop

$$
\boxed{
\Delta p
=\sqrt{\frac2\epsilon}\frac{2\mu U}{a}
\int_0^{2\pi}\frac{d\theta}{\sqrt{1+\lambda\cos\theta}}.}
$$

Finally, the shear on the sphere integrates to

$$
\int_{-\infty}^{\infty}\sigma_{xy}(x,h)\,dx
=\mu U\int\left(-\frac2h+\frac{4h_0}{h^2}\right)dx=0,
$$

because $I_1=\pi$ and $I_2=\pi/2$. Thus the narrow gap exerts no net leading axial shear force on the sphere even though its local shear is nonzero; the leading hydrodynamic force transfer to the sphere is through the large lubrication pressure acting on its gently sloping surface.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
