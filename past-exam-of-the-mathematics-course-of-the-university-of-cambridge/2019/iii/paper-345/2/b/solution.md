<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [shallow-water approximation](../../../../../../shallow-water-approximation.md) requires a small depth-to-horizontal-scale ratio, slow streamwise variation of the channel and interface, small vertical acceleration, and rapid enough cross-sectional mixing for $u$ and $\phi$ to be representative averages. Near the channel apex, or during the initial collapse at a sharp front, these conditions need not hold. The high [Reynolds number](../../../../../../reynolds-number.md) permits neglect of leading viscous resistance; weak stirring mixes the particles without appreciable ambient [fluid entrainment](../../../../../../fluid-entrainment.md).

Put $\lambda=\beta/H$. At elevation $z$, the channel width is $2\lambda xz$, so the occupied area and interface width are

$$
A=\lambda xh^2,\qquad T=2\lambda xh.
$$

[Volume conservation](../../../../../../volume-conservation.md) and suspended-particle conservation give

$$
A_t+(Au)_x=0,\qquad (A\phi)_t+(Au\phi)_x=-W_sT\phi.
$$

The excess [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) is $\rho_0d\phi(h-z)$. Its streamwise gradient averaged over the triangular section gives acceleration $-d\phi h_x-(dh/3)\phi_x$: the weighted mean of $h-z$ is $h/3$. Thus the [triangular-channel shallow water equations](../../../../../../triangular-channel-shallow-water-equations.md) are

$$
\boxed{
\begin{aligned}
h_t+uh_x+\frac h2u_x&=-\frac{uh}{2x},\\
u_t+uu_x+d\phi h_x+\frac{dh}{3}\phi_x&=0,\\
\phi_t+u\phi_x&=-\frac{2W_s\phi}{h}.
\end{aligned}}
$$

The quasilinear coefficient [matrix](../../../../../../matrix.md) in $(h,u,\phi)$ is

$$
\begin{pmatrix}u&h/2&0\\d\phi&u&dh/3\\0&0&u\end{pmatrix}.
$$

Its three distinct real [eigenvalues](../../../../../../eigenvalue.md), for $h,d\phi>0$, establish strict [hyperbolicity](../../../../../../hyperbolicity.md):

$$
\boxed{\frac{dx}{dt}=u,\qquad\frac{dx}{dt}=u\pm c,\qquad c=\sqrt{\frac{d\phi h}{2}}.}
$$

On the material [characteristic curve](../../../../../../characteristic-curve.md), $d\phi/dt=-2W_s\phi/h$. On each of the other two [characteristic curves](../../../../../../characteristic-curve.md), multiplying by the left [eigenvector](../../../../../../eigenvector.md) $(\pm2c/h,1,\pm dh/(3c))$ gives the compatibility [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\boxed{\frac{du}{dt}\pm\frac{2c}{h}\frac{dh}{dt}\pm\frac{h}{3c}\frac{d g'}{dt}
=\mp c\left(\frac ux+\frac{4W_s}{3h}\right),\qquad \frac{dx}{dt}=u\pm c.}
$$

The derivatives are along the indicated characteristic, with $g'=d\phi$. At vanishing concentration, the gravity-wave speeds coalesce and strict [hyperbolicity](../../../../../../hyperbolicity.md) is lost.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
