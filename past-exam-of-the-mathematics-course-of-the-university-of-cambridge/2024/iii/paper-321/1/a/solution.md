<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the [surface density of a disk](../../../../../../surface-density-of-a-disk.md), outward [mass flux](../../../../../../mass-flux.md), internal torque, and surface magnetic torque by

$$
\Sigma=\int_{-\infty}^{\infty}\rho\,dz,
\qquad
F_M=2\pi r\int_{-\infty}^{\infty}\rho u_r\,dz,
$$



$$
\mathcal G=-2\pi r^2\int_{-\infty}^{\infty}
\left(\Pi_{r\phi}+\frac{B_rB_\phi}{4\pi}\right)dz,
\qquad
\mathcal T=2\pi r
\left[\frac{B_\phi B_z}{4\pi}\right]_{-\infty}^{\infty}.
$$

The sign convention makes $\mathcal G$ positive for outward [angular momentum transport](../../../../../../angular-momentum-transport.md) in an ordinary [Keplerian accretion disk](../../../../../../keplerian-accretion-disk.md). Vertical integration of [mass conservation](../../../../../../mass-conservation.md) gives

$$
2\pi r\,\partial_t\Sigma+\partial_rF_M=0.
$$

The [specific angular momentum](../../../../../../specific-angular-momentum.md) is $h=ru_\phi=r^2\Omega$. Multiply the azimuthal equation by $r$, use the continuity equation to put its left-hand side in conservative form, and integrate over $z$. The assumed decay removes the vertical mass and viscous fluxes, whereas the magnetic surface stress remains:

$$
\partial_t(2\pi r\Sigma h)+\partial_r(F_Mh)
=-\partial_r\mathcal G+r\mathcal T.
$$

Subtracting $h$ times the integrated mass equation yields

$$
F_M\frac{dh}{dr}=-\partial_r\mathcal G+r\mathcal T.
$$

Since $F_M=-(dh/dr)^{-1}(\partial_r\mathcal G-r\mathcal T)$, substitution in mass conservation gives the required one-dimensional [advection-diffusion equation](../../../../../../advection-diffusion-equation.md)

$$
\boxed{\partial_t\Sigma
=\frac1{2\pi r}\partial_r\left[
\left(\frac{dr}{dh}\right)
(\partial_r\mathcal G-r\mathcal T)\right]}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
