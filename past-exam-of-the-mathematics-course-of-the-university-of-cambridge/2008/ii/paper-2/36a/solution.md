<h1 id="36a/solution">Solution</h1>

↑ **Parent:** [36A](../36a.md)

The [lubrication approximation](../../../../../lubrication-theory.md) requires depth $h$ small compared with the horizontal variation scale $L$, small bottom slopes, and negligible inertia on the scale $\rho U h^2/(\mu L)\ll1$. Treat the prescribed flat surface as steady and impermeable to leading order. The leading [Stokes equations](../../../../../stokes-equation.md) give $p_z=0$ and $\mu\partial_z^2\boldsymbol u_H=\nabla_Hp$. No slip at $z=-h$ and the imposed shear $\mu\partial_z\boldsymbol u_H|_0=\boldsymbol S$ yield

$$
\boldsymbol u_H(z)=\frac{z^2-h^2}{2\mu}\nabla_Hp+\frac{z+h}{\mu}\boldsymbol S.
$$

Integration and depth-integrated [incompressibility](../../../../../incompressible-flow.md) now give

$$
\boxed{\nabla_H\cdot\boldsymbol q=0,\qquad\mu\boldsymbol q=-\frac{h^3}{3}\nabla_Hp+\frac{h^2}{2}\boldsymbol S.}
$$

The surface value is $\boldsymbol u_0=-h^2\nabla_Hp/(2\mu)+h\boldsymbol S/\mu$. Eliminate the pressure gradient with the flux relation to obtain

$$
\boxed{\boldsymbol u_0=\frac{3\boldsymbol q}{2h}+\frac{h\boldsymbol S}{4\mu}.}
$$

For the circular container, write $\boldsymbol q=\nabla\psi\times\hat z=(\psi_y,-\psi_x)$. Curl the relation $\mu\boldsymbol q/h^3=-\nabla p/3+\boldsymbol S/(2h)$ for $\boldsymbol S=(S_0,0)$. Its vertical component gives

$$
\boxed{\nabla\cdot\left(\frac{\nabla\psi}{h^3}\right)=-\frac{S_0}{2\mu h^2}h_y.}
$$

The wall condition $\boldsymbol q\cdot\boldsymbol n=0$ says $\psi$ is constant on the boundary; choose that constant zero. If $h=h_0$, the equation is Laplace's equation with zero Dirichlet data. The [strong maximum principle for harmonic functions](../../../../../strong-maximum-principle-for-harmonic-functions.md) gives $\psi=0$ and $\boldsymbol q=0$, though there is a sheared return flow through the depth. Its surface velocity is $\boxed{\boldsymbol u_0=(h_0S_0/(4\mu),0)}$.

For $h=h_0(1+\varepsilon y/a)$, the first-order equation is $h_0^{-3}\Delta\psi=-\varepsilon S_0/(2\mu h_0a)+O(\varepsilon^2)$. The zero-boundary quadratic solution is

$$
\boxed{\psi=\varepsilon C(x^2+y^2-a^2)+O(\varepsilon^2),\qquad C=-\frac{S_0h_0^2}{8\mu a}.}
$$

Thus $\boldsymbol q=2\varepsilon C(y,-x)+O(\varepsilon^2)$. Inserting this and the varying depth into the surface formula gives

$$
\boxed{\boldsymbol u_0=\frac{S_0h_0}{4\mu}\left(1-\frac{\varepsilon y}{2a},\ \frac{3\varepsilon x}{2a}\right)+O(\varepsilon^2).}
$$

The circulation is first order in the bottom slope, while its wall-normal flux remains zero.

## ↑ Ancestors (10)

1. [36A](../36a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
