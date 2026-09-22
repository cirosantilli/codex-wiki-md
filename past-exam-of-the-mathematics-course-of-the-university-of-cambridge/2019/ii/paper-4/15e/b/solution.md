<h1 id="15e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $z=x_3$. The body is a [solid of revolution](../../../../../../solid-of-revolution.md) with disk radius

$$
R(z)=z\sqrt{1-\frac zh},
\qquad 0\leq z\leq h.
$$

Its volume and uniform [mass density](../../../../../../density.md) are

$$
V=\pi\int_0^hR(z)^2\,dz
=\pi\int_0^h\left(z^2-\frac{z^3}{h}\right)dz
=\frac{\pi h^3}{12},
\qquad
\rho=\frac{12M}{\pi h^3}.
$$

By the continuous [center of mass](../../../../../../center-of-mass.md) formula, the distance of the center of mass from the pointed origin is

$$
l=\frac{\rho\pi}{M}\int_0^h zR(z)^2\,dz
=\frac{12}{h^3}\left(\frac{h^4}{4}-\frac{h^4}{5}\right)
=\boxed{\frac{3h}{5}}.
$$

For a disk of radius $R$, $\int r^2\,dA=\pi R^4/2$. Therefore the axial moment is

$$
I_3=\frac{\rho\pi}{2}\int_0^hR(z)^4\,dz
=\frac{\rho\pi}{2}h^5\int_0^1u^4(1-u)^2\,du
=\boxed{\frac{2}{35}Mh^2}.
$$

For the transverse $x_1$-axis, $\int x_2^2\,dA=\pi R^4/4$, while every slice also contributes $z^2$ times its mass. Hence

$$
\begin{aligned}
I_1
&=\rho\pi\int_0^h\left(\frac{R(z)^4}{4}+z^2R(z)^2\right)dz\\
&=\rho\pi h^5\left(\frac1{4\cdot105}+\frac1{30}\right)
=\boxed{\frac37Mh^2}.
\end{aligned}
$$

By axial symmetry $I_2=I_1$. These values agree with the [moment of inertia of a pointed cubic-profile solid of revolution](../../../../../../moment-of-inertia-of-a-pointed-cubic-profile-solid-of-revolution.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15E](../../15e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
