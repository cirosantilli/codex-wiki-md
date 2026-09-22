<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\sigma_0^2=\langle v_z^2\rangle=v_{\rm rms}^2/3$ for the one-dimensional thermal [velocity dispersion](../../../../../velocity-dispersion.md) of an isotropic monatomic [ideal gas](../../../../../ideal-gas.md). An [isothermal process](../../../../../isothermal-process.md) keeps $\sigma_0$ fixed, and the vertical [pressure](../../../../../pressure.md) is $P=\rho\sigma_0^2$. [Hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) in the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) $\Phi(z)$ gives

$$
\sigma_0^2\frac{d\log\rho}{dz}=-\frac{d\Phi}{dz}.
$$

Planar symmetry reduces the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) to $\Phi''=4\pi G\rho$. Combining the two equations yields

$$
\boxed{\sigma_0^2\frac{d^2\log\rho}{dz^2}=-4\pi G\rho.}
$$

The velocity factor here is a velocity second moment, not the square of a particular particle's instantaneous vertical velocity.

Set $H^2=\sigma_0^2/(2\pi G\rho_0)$ and try the symmetric [self-gravitating isothermal slab](../../../../../self-gravitating-isothermal-slab.md) profile $\rho=\rho_0\operatorname{sech}^2(z/H)$. Its logarithmic derivatives are

$$
\frac{d\log\rho}{dz}=-\frac2H\tanh(z/H),\qquad
\frac{d^2\log\rho}{dz^2}=-\frac2{H^2}\operatorname{sech}^2(z/H).
$$

The chosen $H$ makes the second expression satisfy the required equation. The central conditions $\rho(0)=\rho_0$ and $\rho'(0)=0$ fix the smooth even solution uniquely. In the scale-height convention used here,

$$
\boxed{\rho(z)=\rho_0\operatorname{sech}^2\!\left(\frac z{2z_0}\right),\qquad z_0=\frac{\sigma_0}{\sqrt{8\pi G\rho_0}},\qquad H=2z_0.}
$$

The undefined constant printed as $a$ in the scale-height denominator must be $G$; this follows both from substitution and dimensions.

Integrating [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md), with the additive potential constant chosen so that $\Phi(0)=0$, gives

$$
\boxed{\Phi(z)=2\sigma_0^2\log\cosh(z/H),\qquad \ddot z=-\frac{2\sigma_0^2}{H}\tanh(z/H).}
$$

The [orbits in a self-gravitating isothermal slab](../../../../../orbits-in-a-self-gravitating-isothermal-slab.md) separate into horizontal and vertical motions. There is no horizontal force, so $x=x_i+v_xt$ and $y=y_i+v_yt$, with constant horizontal velocities. For collisionless test particles, or between gas collisions, [conservation of energy](../../../../../conservation-of-energy.md) fixes the vertical energy

$$
E_z=\frac12\dot z^2+\Phi(z).
$$

Every finite $E_z>0$ has two turning points $\pm A$, where

$$
A=H\operatorname{arcosh}\!\left(e^{E_z/(2\sigma_0^2)}\right),\qquad
T_z=4\int_0^A\frac{dz}{\sqrt{2[E_z-\Phi(z)]}}.
$$

Thus the general orbit drifts uniformly in the plane while oscillating periodically across it. A particle with $E_z=0$ stays in the midplane; an orbit with nonzero horizontal velocity is generally not closed.

Near the plane, $\Phi(z)=\sigma_0^2z^2/H^2+O(z^4)$, so the vertical motion is a [harmonic oscillator](../../../../../simple-harmonic-motion.md) with $\nu^2=2\sigma_0^2/H^2=4\pi G\rho_0$. Far from the plane, $\Phi\sim2\sigma_0^2|z|/H$ and the force tends to a constant magnitude. Indeed the [surface density](../../../../../surface-density-of-a-disk.md) is $\Sigma=\int\rho\,dz=2\rho_0H$, and that magnitude is $2\pi G\Sigma$. Large-amplitude vertical motion is therefore approximately uniformly accelerated on each side, rather than sinusoidal. Because this ideal slab extends infinitely in the horizontal directions and its potential grows without bound as $|z|\to\infty$, no finite-energy particle escapes vertically.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
