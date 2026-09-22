<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For each [Volvox](../../../../../volvox.md) colony, the excess gravitational force is

$$
F=\frac{4\pi}{3}R^3(\rho-\rho_w)g
=\frac{4\pi}{3}\rho_w\epsilon gR^3.
$$

For a normal [Stokeslet](../../../../../stokeslet.md) a distance $R$ below a flat [stress-free interface](../../../../../stress-free-boundary-condition.md), the image is an oppositely directed Stokeslet a distance $R$ above it. The real force creates no lateral velocity at the other colony because both centres have the same height. Their separation from the image is $(x,-2R)$, however, so each colony moves toward the other with speed

$$
U_x=\frac{FRx}{4\pi\mu(x^2+4R^2)^{3/2}}.
$$

Both colonies move, and therefore

$$
\boxed{\frac{dx}{dt}
=-\frac{FRx}{2\pi\mu(x^2+4R^2)^{3/2}}
=-\frac{2\rho_w\epsilon gR^4}{3\mu}
\frac{x}{(x^2+4R^2)^{3/2}}.}
$$

Define

$$
\xi=\frac{x}{2R},
\qquad
\tau=\frac{Ft}{16\pi\mu R^2}
=\frac{\rho_w\epsilon gR}{12\mu}t.
$$

The dimensionless dynamics are

$$
\frac{d\xi}{d\tau}
=-\frac{\xi}{(1+\xi^2)^{3/2}}
=-\frac{dV}{d\xi},
\qquad
\boxed{V(\xi)=-\frac1{\sqrt{1+\xi^2}}.}
$$

This [gradient flow](../../../../../gradient-flow.md) descends an even attractive potential with minimum $V(0)=-1$ and $V\to0^-$ as $|\xi|\to\infty$.

For $\xi\gg1$, $d\xi/d\tau\simeq-1/\xi^2$, so the approach from $\xi_0=x_0/(2R)$ takes $\tau_c\simeq\xi_0^3/3$. Restoring dimensions,

$$
\boxed{T\simeq\frac{\mu x_0^3}
{2\rho_w\epsilon gR^4}.}
$$

With water viscosity $\mu\simeq10^{-3}\,\mathrm{Pa\,s}$, $\rho_w\simeq10^3\,\mathrm{kg\,m^{-3}}$, $\epsilon=0.03$, $R=200\,\mu\mathrm m$, and $x_0=5R$, this gives

$$
\boxed{T\simeq1.1\,\mathrm s.}
$$

Because $x_0/(2R)=2.5$ is only moderately large, this is a far-field estimate rather than the exact collision time.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 355](../../paper-355-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
