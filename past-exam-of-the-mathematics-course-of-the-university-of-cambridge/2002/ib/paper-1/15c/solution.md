<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

For an inviscid fluid of constant [density](../../../../../density.md), with irrotational [velocity](../../../../../velocity.md) $\mathbf u=\nabla\Phi$ and conservative body-force potential $\Psi$, the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md) is

$$
\boxed{\Phi_t+\frac12|\mathbf u|^2+\frac p\rho+\Psi=C(t)}.
$$

It holds throughout a connected irrotational fluid region, up to the time-dependent gauge of $\Phi$. Indeed the [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) and $\nabla\times\mathbf u=0$ imply that the gradient of the left side is zero. In the bubble problem there is no body-force contribution compatible with the assumed spherical symmetry.

Spherical incompressibility gives $\partial_r(r^2u_r)=0$. The moving interface imposes $u_r(R,t)=\dot R$, so

$$
\boxed{\mathbf u(r,t)=\frac{R^2\dot R}{r^2}\mathbf e_r,\qquad\Phi(r,t)=-\frac{R^2\dot R}{r}},\qquad r>R(t).
$$

This potential tends to zero at infinity, where the [velocity](../../../../../velocity.md) tends to zero and $C(t)=p_\infty/\rho$. Differentiate $\Phi$ at fixed spatial $r$, not along the moving interface: $\Phi_t=-(2R\dot R^2+R^2\ddot R)/r$. At $r=R$, [pressure](../../../../../pressure.md) [continuity](../../../../../continuous-function.md) without [surface tension](../../../../../surface-tension.md) gives $p=p_\infty-\Delta p$. Bernoulli therefore yields $-2\dot R^2-R\ddot R+\dot R^2/2-\Delta p/\rho=0$, or the [Rayleigh equation for an inviscid spherical bubble](../../../../../rayleigh-equation-for-an-inviscid-spherical-bubble.md)

$$
\boxed{R\ddot R+\frac32\dot R^2=-\frac{\Delta p}{\rho}}.
$$

Integrating the [kinetic energy](../../../../../kinetic-energy.md) over the exterior fluid gives

$$
K=\frac12\rho\int_R^\infty\left(\frac{R^2\dot R}{r^2}\right)^24\pi r^2\,dr=\boxed{2\pi\rho R^3\dot R^2}.
$$

Differentiate and use the radius equation:

$$
\dot K=4\pi\rho R^2\dot R\left(R\ddot R+\frac32\dot R^2\right)=-4\pi\Delta pR^2\dot R.
$$

With $R(0)=R_0$ and $\dot R(0)=0$, the [pressure-work energy balance for a spherical bubble](../../../../../pressure-work-energy-balance-for-a-spherical-bubble.md) integrates to

$$
\boxed{2\pi\rho R^3\dot R^2=\frac{4\pi\Delta p}{3}(R_0^3-R^3)},
$$

or

$$
\boxed{\dot R^2=\frac{2\Delta p}{3\rho}\left(\frac{R_0^3}{R^3}-1\right)}.
$$

The collapsing branch takes the negative square root for $\dot R$. The energy gain is exactly the [pressure](../../../../../pressure.md) difference times the lost bubble volume, providing a check on the sign and numerical factor.

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
