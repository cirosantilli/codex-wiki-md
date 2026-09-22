<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

Take the sphere to move in the positive $z$-direction and use spherical coordinates centred on it. An axisymmetric harmonic potential that decays at infinity has the dipole form $A\cos\theta/r^2$. The no-penetration condition in the laboratory frame is

$$
\left.\frac{\partial\phi}{\partial r}\right|_{r=a}
=U\cos\theta.
$$

It fixes $A=-Ua^3/2$, so the [potential flow around a translating sphere](../../../../../potential-flow-around-a-translating-sphere.md) is

$$
\boxed{
\phi(r,\theta)=-\frac{Ua^3}{2r^2}\cos\theta}.
$$

The laboratory-frame [velocity](../../../../../velocity.md) components are

$$
\boxed{
u_r=\frac{Ua^3}{r^3}\cos\theta,
\qquad
u_\theta=\frac{Ua^3}{2r^3}\sin\theta,
\qquad
u_\varphi=0}.
$$

The fluid [kinetic energy](../../../../../kinetic-energy.md) is

$$
\begin{aligned}
K_f
&=\frac\rho2\int_a^\infty\int_{S^2}
\frac{U^2a^6}{r^6}
\left(\cos^2\theta+\frac14\sin^2\theta\right)
r^2\,d\Omega\,dr\\
&=\boxed{\frac{\pi}{3}\rho a^3U^2}
=\frac12\left(\frac12\rho V\right)U^2,
\end{aligned}
$$

where $V=4\pi a^3/3$. Thus the [added mass of a sphere](../../../../../added-mass-of-a-sphere.md) is $\rho V/2$.

When the sphere falls, replacing fluid of density $\rho$ by material of density $\rho_s$ lowers the gravitational [potential energy](../../../../../potential-energy.md) at rate

$$
\boxed{\dot P=-(\rho_s-\rho)VgU}.
$$

The total [kinetic energy](../../../../../kinetic-energy.md) of sphere and fluid is

$$
K=\frac12\left(\rho_s+\frac\rho2\right)VU^2.
$$

Conservation of total energy gives

$$
\left(\rho_s+\frac\rho2\right)VU\frac{dU}{dt}
-(\rho_s-\rho)VgU=0.
$$

For $U\ne0$, the [acceleration of a freely falling sphere with added mass](../../../../../acceleration-of-a-freely-falling-sphere-with-added-mass.md) is

$$
\boxed{
\frac{dU}{dt}=\frac{\rho_s-\rho}{\rho_s+\rho/2}\,g}.
$$

The same formula holds at release by continuity.

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
