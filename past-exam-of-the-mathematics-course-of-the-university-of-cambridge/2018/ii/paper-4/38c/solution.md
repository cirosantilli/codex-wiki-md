<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

The exact gap between the plane and the circle is

$$
h(x)=h_0+a-\sqrt{a^2-x^2}.
$$

In the narrow region relevant to [lubrication theory](../../../../../lubrication-theory.md),

$$
\boxed{h(x)\simeq h_0+\frac{x^2}{2a}},
$$

so changes occur over the streamwise scale $x=O(\sqrt{ah_0})$; below use $x=\sqrt{2ah_0}X$.

Choose the positive $x$ direction to be the direction of the cylinder surface velocity $U=a\Omega$ in the gap, and write $\mu=\rho\nu$ for the [dynamic viscosity](../../../../../dynamic-viscosity.md). The lubrication velocity profile and [volume flux](../../../../../volumetric-flow-rate.md) per unit axial length are

$$
u(y)=\frac{p_x}{2\mu}y(y-h)+\frac{Uy}{h},
\qquad
Q=\int_0^hu\,dy=-\frac{h^3p_x}{12\mu}+\frac{Uh}{2}.
$$

Since $Q$ is constant and the pressure returns to the same ambient value as $x\to\pm\infty$, $\int_{-\infty}^{\infty}p_xdx=0$. Therefore

$$
Q=\frac U2
\frac{\int_{-\infty}^{\infty}h^{-2}dx}
{\int_{-\infty}^{\infty}h^{-3}dx}.
$$

Using $h=h_0(1+X^2)$ and the supplied integrals gives

$$
\boxed{Q=\frac23Uh_0=\frac23a\Omega h_0},
$$

in the direction of the cylinder surface motion.

The [shear stress](../../../../../shear-stress.md) exerted by the fluid on the cylinder is opposite to

$$
\mu u_y(h)=\frac h2p_x+\frac{\mu U}{h}.
$$

Eliminating $p_x$ and inserting $Q=2Uh_0/3$ gives

$$
\boxed{\tau(x)=-4\mu U\left(\frac1h-\frac{h_0}{h^2}\right)},
$$

where the sign is relative to $U$. Since

$$
\int_{-\infty}^{\infty}
\left(\frac1h-\frac{h_0}{h^2}\right)dx
=\frac\pi2\sqrt{\frac{2a}{h_0}},
$$

the resisting [torque](../../../../../torque.md) per unit axial length is

$$
\boxed{T=a\int_{-\infty}^{\infty}\tau\,dx
=-2\sqrt2\,\pi\rho\nu\Omega
\frac{a^{5/2}}{h_0^{1/2}}}.
$$

Finally, the ratio of streamwise fluid inertia $U^2/\sqrt{ah_0}$ to transverse viscous acceleration $\nu U/h_0^2$ is of order

$$
\frac{a^{1/2}\Omega h_0^{3/2}}{\nu}.
$$

The stated restriction makes this lubrication-scale [Reynolds number](../../../../../reynolds-number.md) small, justifying neglect of inertia.

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
