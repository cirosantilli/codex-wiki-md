<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

At the initial instant the [circulation](../../../../../circulation-physics.md) around every closed curve is zero because the fluid is at rest. A smooth material-flow map carries closed curves bijectively between times. Conservation of [circulation](../../../../../circulation-physics.md) around every [material curve](../../../../../material-curve.md) therefore makes the line integral of the velocity zero around every closed curve at the current time, not just small contractible loops. Fix a reference point in a connected fluid region and define

$$
\phi(x)=\int_{x_0}^{x}\mathbf u\cdot d\mathbf l.
$$

The vanishing closed-curve integrals make this independent of the path. Thus $\mathbf u=\nabla\phi$: the fluid has a globally defined [velocity potential](../../../../../velocity-potential.md). Its [incompressible flow](../../../../../incompressible-flow.md) condition is $\nabla\cdot\mathbf u=0$, hence **$\nabla^2\phi=0$**. This argument establishes the global potential without silently assuming the fluid region is [simply connected](../../../../../simply-connected-space.md).

Use the laboratory frame, with the sphere instantaneously centred at the origin and moving in the $\theta=0$ direction. Impermeability equates fluid and sphere normal velocities, while the fluid is at rest at infinity:

$$
\phi_r(a,\theta)=U\cos\theta,\qquad\nabla\phi\longrightarrow0\quad(r\to\infty).
$$

Choose the additive constant so that $\phi\to0$ at infinity. Substitution of $\phi=f(r)\cos\theta$ into the [Laplace equation](../../../../../laplace-equation.md) in [spherical polar coordinates](../../../../../spherical-coordinate-system.md) gives

$$
(r^2f')'-2f=0,\qquad f(r)=Ar+Br^{-2}.
$$

The far-field condition gives $A=0$, and $f'(a)=U$ gives $B=-Ua^3/2$. Therefore

$$
\boxed{\phi(r,\theta)=-\frac{Ua^3\cos\theta}{2r^2}.}
$$

The radial and polar velocity components are

$$
u_r=\phi_r=\frac{Ua^3\cos\theta}{r^3},\qquad u_\theta=\frac1r\phi_\theta=\frac{Ua^3\sin\theta}{2r^3}.
$$

For fluid density $\rho$, its [kinetic energy](../../../../../kinetic-energy.md) is

$$
\begin{aligned}
T_f&=\frac\rho2\int_a^\infty\int_0^{2\pi}\int_0^\pi\frac{U^2a^6}{r^6}\left(\cos^2\theta+\frac14\sin^2\theta\right)r^2\sin\theta\,d\theta\,d\varphi\,dr\\
&=\frac\rho2U^2a^6\cdot\frac1{3a^3}\cdot2\pi
=\boxed{\frac{\pi\rho a^3U^2}{3}}.
\end{aligned}
$$

Thus $T_f=\frac12m_aU^2$ with [added mass of a sphere](../../../../../added-mass-of-a-sphere.md) $m_a=2\pi\rho a^3/3$, half the mass of displaced fluid.

For the initial acceleration after release, let $\dot U$ denote the upward acceleration, $\mathcal V=4\pi a^3/3$, and $m_b=\rho_b\mathcal V$. At the instant $U=0$, the velocity-squared term in the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md) vanishes. The time derivative of the potential at the sphere is $\phi_t(a,\theta)=-a\dot U\cos\theta/2$; centre-motion corrections also vanish at this instant. Relative to hydrostatic pressure, the additional pressure is consequently

$$
p_{\mathrm{acc}}=-\rho\phi_t=\frac12\rho a\dot U\cos\theta.
$$

Its upward force on the sphere is

$$
F_{\mathrm{acc}}=-\int_{r=a}p_{\mathrm{acc}}\cos\theta\,dS=-\frac12\rho a\dot U\cdot\frac{4\pi a^2}{3}=-m_a\dot U.
$$

Adding [buoyancy](../../../../../buoyancy.md) and weight, [Newton's second law](../../../../../newton-s-second-law.md) gives $(m_b+m_a)\dot U=(\rho-\rho_b)\mathcal Vg$. Therefore

$$
\boxed{\dot U=\frac{2(\rho-\rho_b)g}{\rho+2\rho_b}.}
$$

This is the [acceleration of a freely falling sphere with added mass](../../../../../acceleration-of-a-freely-falling-sphere-with-added-mass.md), with upward chosen positive. If $\rho_b>\rho$, the negative value represents a downward acceleration.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
