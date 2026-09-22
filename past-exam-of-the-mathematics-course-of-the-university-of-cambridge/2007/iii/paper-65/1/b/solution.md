<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $V=\dot R$, $a=2/(5-\beta)$ and

$$
\xi=\frac rR,\qquad u(r,t)=V U(\xi),\qquad
\rho(r,t)=CR^{-\beta}D(\xi),\qquad
p(r,t)=CR^{-\beta}V^2P(\xi).
$$

Here $u$ is the outward radial [velocity](../../../../../../velocity.md); $U,D,P$ are dimensionless. The relations

$$
\partial_t\xi=-\frac VR\xi,\qquad
\partial_r\xi=\frac1R,\qquad
q\equiv\frac{R\dot V}{V^2}=\frac{a-1}{a}=\frac{\beta-3}{2}
$$

are sufficient for the reduction. In smooth post-shock gas the spherical [continuity equation](../../../../../../continuity-equation.md), [Euler equations](../../../../../../euler-equations-for-an-inviscid-fluid.md) and adiabatic [pressure](../../../../../../pressure.md) equation are

$$
\partial_t\rho+u\partial_r\rho=-\rho(\partial_ru+2u/r),\qquad
\partial_tu+u\partial_ru=-\frac1\rho\partial_rp,
$$



$$
\partial_tp+u\partial_rp=-\gamma p(\partial_ru+2u/r).
$$

For example, the [mass density](../../../../../../density.md) [material derivative](../../../../../../material-derivative.md) is $CR^{-\beta}(V/R)[(U-\xi)D'-\beta D]$, and the [velocity](../../../../../../velocity.md) [material derivative](../../../../../../material-derivative.md) is $(V^2/R)[(U-\xi)U'+qU]$. After cancellation of the dimensional factors the [spherical blast wave in a power-law ambient density](../../../../../../spherical-blast-wave-in-a-power-law-ambient-density.md) obeys

$$
\boxed{(U-\xi)D'+D\left(U'+\frac{2U}{\xi}-\beta\right)=0,}
$$



$$
\boxed{(U-\xi)U'+\frac{\beta-3}{2}U=-\frac{P'}D,}
$$



$$
\boxed{(U-\xi)P'+\left[\gamma\left(U'+\frac{2U}{\xi}\right)-3\right]P=0.}
$$

Primes here mean $d/d\xi$. In the [pressure](../../../../../../pressure.md) equation the scale derivative $2q-\beta=-3$ explains the constant term. Once the profiles are found, their finite [energy](../../../../../../energy.md) integral fixes $A$ through

$$
E=4\pi CR^{3-\beta}V^2\int_0^1\left[\frac12DU^2+\frac{P}{\gamma-1}\right]\xi^2\,d\xi.
$$

No global constant in $p/\rho^\gamma$ is assumed: the [shock wave](../../../../../../shock-wave.md) generates different [entropies](../../../../../../entropy.md) in shells swept up at different times.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
