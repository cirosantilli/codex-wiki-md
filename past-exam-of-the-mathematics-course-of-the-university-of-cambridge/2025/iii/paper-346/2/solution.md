<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A galaxy contains so many stars that its two-body relaxation time is generally much longer than its age. Individual encounters can therefore be neglected and each star moves in the smooth collective potential. Liouville conservation along these Hamiltonian trajectories gives the [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md)

$$
\frac{dF}{dt}=0.
$$

In spherical phase-space coordinates this is

$$
\boxed{
F_t+\dot rF_r+\dot\theta F_\theta+\dot\varphi F_\varphi
+\dot v_rF_{v_r}+\dot v_\theta F_{v_\theta}+\dot v_\varphi F_{v_\varphi}=0}.
$$

The spherical line element is $ds^2=dr^2+r^2d\theta^2+r^2\sin^2\theta\,d\varphi^2$, so

$$
\boxed{\dot r=v_r,\qquad \dot\theta=v_\theta/r,\qquad
\dot\varphi=v_\varphi/(r\sin\theta)}.
$$

For a unit-mass star in a spherical potential,

$$
L=\frac12(\dot r^2+r^2\dot\theta^2+r^2\sin^2\theta\,\dot\varphi^2)-\Phi(r).
$$

The Euler--Lagrange equations, followed by differentiating $v_\theta=r\dot\theta$ and $v_\varphi=r\sin\theta\,\dot\varphi$, give

$$
\boxed{\dot v_r=\frac{v_\theta^2+v_\varphi^2}{r}-\Phi'(r)},
$$



$$
\boxed{\dot v_\theta=\frac{v_\varphi^2\cot\theta-v_rv_\theta}{r}},
\qquad
\boxed{\dot v_\varphi=-\frac{v_\varphi v_r+v_\varphi v_\theta\cot\theta}{r}}.
$$

Integrating the Boltzmann equation over velocity space, with vanishing velocity-space boundary terms, gives spherical mass conservation:

$$
\boxed{\rho_t+\partial_r(\rho\langle v_r\rangle)
+\frac2r\rho\langle v_r\rangle=0}.
$$

Multiplication by $v_r$ and integration gives the radial [Jeans equation](../../../../../jeans-equation.md). With isotropic dispersion

$$
\langle v_r^2\rangle=\sigma^2+\langle v_r\rangle^2,\qquad
\langle v_\theta^2\rangle=\langle v_\varphi^2\rangle=\sigma^2,
$$

the geometric dispersion terms cancel, and use of continuity yields

$$
\boxed{
\partial_r(\rho\sigma^2)
+\rho\,\partial_t\langle v_r\rangle
+\rho\langle v_r\rangle\partial_r\langle v_r\rangle
=-\rho\,\Phi'(r)}.
$$

The factor $\rho$ on the right is required dimensionally.

In a Lambda-CDM background, the local excess mass contributes $GM(r)/r^2$, homogeneous matter inside radius $r$ contributes $4\pi G\rho_b r/3$, and the cosmological constant contributes outward acceleration $\Lambda r/3$. Hence

$$
\boxed{\Phi'(r)=\frac{GM(r)}{r^2}+\frac{4\pi G\rho_b}{3}r-\frac{\Lambda}{3}r}.
$$

Since $\Omega_m=8\pi G\rho_b/(3H^2)$, $\Omega_\Lambda=\Lambda/(3H^2)$, and $q=\Omega_m/2-\Omega_\Lambda$,

$$
\boxed{\Phi'(r)=\frac{GM(r)}{r^2}+qH^2r}.
$$

Write $\langle v_r\rangle=Hr+v_p$, where $v_p$ is the [peculiar velocity](../../../../../peculiar-velocity.md). Then

$$
\partial_t\langle v_r\rangle+\langle v_r\rangle\partial_r\langle v_r\rangle
=(\dot H+H^2)r+
v_{p,t}+Hv_p+Hrv_{p,r}+v_pv_{p,r}.
$$

The acceleration equation gives $\dot H+H^2=\ddot a/a=-qH^2$, which cancels the background term in $\Phi'$. Therefore

$$
\boxed{\partial_r(\rho\sigma^2)
=-\rho\left[\frac{GM(r)}{r^2}+S(r,t)\right]},
$$



$$
\boxed{S=v_pv_{p,r}+H(v_p+rv_{p,r})+v_{p,t}}.
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
