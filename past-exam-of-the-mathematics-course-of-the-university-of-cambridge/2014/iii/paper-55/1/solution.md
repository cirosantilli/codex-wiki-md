<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a spherical [stellar polytrope](../../../../../stellar-polytrope.md) in [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md), combine $dm_r/dr=4\pi r^2\rho$ with $dP/dr=-Gm_r\rho/r^2$ to eliminate the [enclosed mass](../../../../../enclosed-mass.md):

$$
\frac1{r^2}\frac d{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G\rho.
$$

For $n>0$, put $P=K\rho^{1+1/n}$, $\rho=\rho_c\theta^n$, $P=P_c\theta^{n+1}$ and $r=a\xi$. Since $\rho^{-1}dP/dr=(n+1)P_c\theta'/(a\rho_c)$, choose

$$
a^2=\frac{(n+1)P_c}{4\pi G\rho_c^2}
=\frac{(n+1)K}{4\pi G}\rho_c^{(1-n)/n}.
$$

The [Lane-Emden equation](../../../../../lane-emden-equation.md) is then

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}(\xi^2\theta')=-\theta^n.}
$$

A regular center requires **$\theta(0)=1$ and $\theta'(0)=0$**, with positive chosen central [mass density](../../../../../density.md) and [pressure](../../../../../pressure.md). Locally $\theta=1-\xi^2/6+n\xi^4/120+\cdots$. The stellar surface is the first positive zero $\xi_1$, where the idealized external [pressure](../../../../../pressure.md) is zero; retain the positive solution before it. Thus $R=a\xi_1$ and the [Lane-Emden mass formula](../../../../../lane-emden-mass-formula.md) is

$$
M=4\pi a^3\rho_c\omega_n,\qquad
\omega_n=-\xi_1^2\theta'(\xi_1)
=\int_0^{\xi_1}\xi^2\theta^n\,d\xi.
$$

The surface condition selects where to stop a centrally regular solution, rather than replacing its central regularity conditions.

For a [polytrope of index zero](../../../../../polytrope-of-index-zero.md), the density is constant and $(\xi^2\theta')'=-\xi^2$. Regularity gives

$$
\boxed{\theta_0=1-\xi^2/6,\quad\xi_1=\sqrt6,\quad R=\sqrt6\,a.}
$$

The [pressure](../../../../../pressure.md) is $P_c\theta_0$ and $a^2=P_c/(4\pi G\rho_c^2)$, so $R^2=3P_c/(2\pi G\rho_c^2)$. **Index zero is the structural incompressible limit**: the expression $K\rho^{1+1/n}$ is not itself defined at $n=0$.

For a [polytrope of index one](../../../../../polytrope-of-index-one.md), set $u=\xi\theta$. The equation becomes $u''+u=0$, while central regularity requires $u(0)=0$, $u'(0)=1$. Hence

$$
\boxed{\theta_1=\frac{\sin\xi}{\xi},\quad\xi_1=\pi,\quad
R=\pi a=\sqrt{\frac{\pi K}{2G}},\quad\omega_1=\pi.}
$$

The mass is $4\pi^2a^3\rho_c$, so it can change with central [mass density](../../../../../density.md) while the radius stays fixed.

The [moment of inertia of a polytropic star](../../../../../moment-of-inertia-of-a-polytropic-star.md) about any axis through its center follows by integrating $r^2\sin^2\vartheta$ over spherical shells:

$$
I=\frac{8\pi}{3}\int_0^R\rho(r)r^4\,dr
=\frac{8\pi}{3}\rho_ca^5\int_0^{\xi_1}\xi^4\theta^n\,d\xi.
$$

For constant [mass density](../../../../../density.md) this gives **$I_0=2MR^2/5$**. For index one, [integration by parts](../../../../../integration-by-parts.md) gives $\int_0^\pi\xi^3\sin\xi\,d\xi=\pi(\pi^2-6)$, and therefore

$$
\boxed{I_1=\frac23\left(1-\frac6{\pi^2}\right)MR^2\simeq0.26138MR^2.}
$$

These are axial [moments of inertia](../../../../../moment-of-inertia.md), not the scalar second mass moment $\int r^2dm$.

For a finite-radius centrally regular [stellar polytrope](../../../../../stellar-polytrope.md) with $0<n<5$ and $n\ne1$, eliminate $\rho_c$ from $R=a\xi_1$ and $M=4\pi a^3\rho_c\omega_n$. The resulting [polytropic mass-radius relation](../../../../../polytropic-mass-radius-relation.md) is

$$
\boxed{M=AR^{p(n)},\quad p(n)=\frac{n-3}{n-1},\quad
A=4\pi\omega_n\,\xi_1^{-p(n)}
\left(\frac{(n+1)K}{4\pi G}\right)^{n/(n-1)}.}
$$

Here $\xi_1,\omega_n$ are dimensionless functions of $n$. **At $n=1$ no such single-valued mass-as-a-power-of-radius relation exists at fixed $K$**: the radius is fixed instead. At $n=3$ the exponent is zero and $M=4\pi\omega_3(K/(\pi G))^{3/2}$ is independent of central [mass density](../../../../../density.md). For the incompressible case, $M=(4\pi\rho_c/3)R^3$ at fixed [mass density](../../../../../density.md). Regular $n\ge5$ solutions have no finite zero-pressure surface, so the finite-radius formula does not apply to them.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
