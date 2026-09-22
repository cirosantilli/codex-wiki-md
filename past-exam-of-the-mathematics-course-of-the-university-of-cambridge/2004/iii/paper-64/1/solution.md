<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $u<0$ for inward radial [velocity](../../../../../velocity.md), and assume a constant [specific-heat ratio](../../../../../heat-capacity-ratio.md) $\gamma>1$. The [isentropic flow](../../../../../isentropic-flow.md) has $p=K\rho^\gamma$ and [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) $c^2=\gamma K\rho^{\gamma-1}$. Steady spherical [mass conservation](../../../../../mass-conservation.md) and the radial [Euler equation for fluid motion](../../../../../euler-equations-for-an-inviscid-fluid.md) give

$$
4\pi r^2\rho u=-\dot M,\qquad
\frac{\rho'}\rho=-\frac2r-\frac{u'}u,\qquad
uu'=-c^2\frac{\rho'}\rho-\frac{GM}{r^2}.
$$

Eliminating the [mass density](../../../../../density.md) [derivative](../../../../../derivative.md) gives $(u-c^2/u)u'=2c^2/r-GM/r^2$, or

$$
\boxed{\frac{u'}u=\frac1r\frac{GM/r-2c^2}{c^2-u^2}.}
$$

Differentiating $c^2\propto\rho^{\gamma-1}$ gives the corresponding [sound speed](../../../../../speed-of-sound.md) equation:

$$
\boxed{\frac{c'}c=-\frac{\gamma-1}{2}\left(\frac2r+\frac{u'}u\right)
=-\frac{\gamma-1}{2r}\frac{GM/r-2u^2}{c^2-u^2}.}
$$

At a smooth [sonic point](../../../../../sonic-point.md), $u_s^2=c_s^2$. A finite [derivative](../../../../../derivative.md) requires the numerator of the flow equation to vanish too. Thus

$$
\boxed{u_s^2=c_s^2=\frac{GM}{2r_s}.}
$$

This regularity requirement concerns a smooth [transonic branch](../../../../../transonic-branch.md), rather than an arbitrary singular solution reaching unit [Mach number](../../../../../mach-number.md).

Integrating the momentum equation using the [specific enthalpy](../../../../../specific-enthalpy.md) $c^2/(\gamma-1)$ yields the [Bernoulli equation](../../../../../bernoulli-equation.md)

$$
\frac{u^2}{2}+\frac{c^2}{\gamma-1}-\frac{GM}{r}
=\frac{c_\infty^2}{\gamma-1},\qquad
c_\infty^2=\gamma K\rho_\infty^{\gamma-1}.
$$

For a finite positive [mass accretion rate](../../../../../mass-accretion-rate.md), its large-radius solution has

$$
u=-\frac{\dot M}{4\pi\rho_\infty r^2}[1+O(r^{-1})],\qquad
c^2=c_\infty^2+\frac{(\gamma-1)GM}{r}+O(r^{-4}),
$$



$$
\rho=\rho_\infty\left[1+\frac{GM}{c_\infty^2r}+O(r^{-2})\right].
$$

These expressions satisfy both the flow equations asymptotically and show **$u\to0$ and $\rho\to\rho_\infty$**. In particular $u'/u\sim-2/r$ agrees with the first boxed equation. Combining the [Bernoulli equation](../../../../../bernoulli-equation.md) with sonic regularity additionally gives $c_s^2=2c_\infty^2/(5-3\gamma)$, so a finite positive [sonic point](../../../../../sonic-point.md) occurs in the range identified below.

For the small-radius inward [free fall](../../../../../free-fall.md) branch, neglecting enthalpy against $GM/r$ in the [Bernoulli equation](../../../../../bernoulli-equation.md) predicts $u^2\sim2GM/r$. The [continuity equation](../../../../../continuity-equation.md) then fixes $\rho\propto r^{-3/2}$, and consequently $c^2\propto r^{-3(\gamma-1)/2}$. The neglected-to-leading ratio is

$$
\frac{c^2}{u^2}\propto r^{(5-3\gamma)/2}.
$$

It tends to zero precisely when

$$
\boxed{\gamma<\gamma_{\mathrm{crit}}=\frac53.}
$$

This makes the assumed [supersonic flow](../../../../../supersonic-flow.md) and leading [free fall](../../../../../free-fall.md) self-consistent. At equality, the ratio is of constant order rather than vanishing; above it, the proposed asymptotic balance fails. The isothermal limit $\gamma=1$ also permits free fall, with logarithmic rather than power-law enthalpy.

For the stellar funnel, write the magnetic scalar potential as $\psi=\mu\cos\theta/r^2$, where $R=r\sin\theta$ and $z=r\cos\theta$. Its [magnetic dipole field](../../../../../magnetic-dipole-field.md) has $B_r=-2\mu\cos\theta/r^3$ and $B_\theta=-\mu\sin\theta/r^3$, so a [magnetic-field-line equation](../../../../../magnetic-field-line-equation.md) is

$$
\frac{dr}{r\,d\theta}=\frac{B_r}{B_\theta}=2\cot\theta,
\qquad r=\ell\sin^2\theta.
$$

The edge of the polar [flux tube](../../../../../flux-tube.md) meets the stellar surface at $\theta_*\simeq a/R_*$. Thus, near the pole, $\theta^2\simeq\theta_*^2r/R_*$, and its transverse radius is $R\simeq r\theta$. This proves the [dipolar flux-tube area](../../../../../dipolar-flux-tube-area.md) law

$$
\boxed{A(r)\simeq\pi r^2\theta^2=\pi a^2\left(\frac r{R_*}\right)^3.}
$$

Equivalently [magnetic flux](../../../../../magnetic-flux.md) conservation gives $A|\mathbf B|=\mathrm{constant}$ and $|\mathbf B|\propto r^{-3}$. The stipulated small cross section keeps the tube close to the polar axis, where its direction is approximately radial; the approximation is not valid all the way to arbitrarily large $r$.

Outside the star the prescribed field is a gradient, hence $\nabla\times\mathbf B=0$ and $\mathbf j=0$. Its [Lorentz force density](../../../../../lorentz-force-density.md) is therefore **$\mathbf j\times\mathbf B=0$**. The magnetic-[pressure](../../../../../pressure.md) and magnetic-tension parts cancel in this exact current-free dipole. Field-aligned [velocity](../../../../../velocity.md) also has $\mathbf u\times\mathbf B=0$, consistent with a steady prescribed field. The following calculation uses the narrow polar funnel approximation.

Now steady [mass conservation](../../../../../mass-conservation.md) reads $\rho u A=\mathrm{constant}$. With $A\propto r^3$, replace the spherical factor 2 by 3:

$$
\left(u-\frac{c^2}{u}\right)u'=\frac{3c^2}{r}-\frac{GM}{r^2}.
$$

The [Bernoulli equation](../../../../../bernoulli-equation.md) is unchanged because the magnetic field supplies no work or force. On a gravity-dominated [free fall](../../../../../free-fall.md) branch, $u^2\sim2GM/r$, but $\rho\propto r^{-5/2}$ and $c^2\propto r^{-5(\gamma-1)/2}$. Hence

$$
\frac{c^2}{u^2}\propto r^{(7-5\gamma)/2},\qquad
\boxed{\gamma_{\mathrm{crit}}=\frac75\quad\text{for the dipolar funnel}.}
$$

The same bound follows from regular [transonic accretion in a power-law tube](../../../../../transonic-accretion-in-a-power-law-tube.md): $u_s^2=c_s^2=GM/(3r_s)$ and the reservoir-matched [Bernoulli equation](../../../../../bernoulli-equation.md) gives $c_s^2=2c_\infty^2/(7-5\gamma)$. The stellar surface cuts off the mathematical small-$r$ limit; the criterion refers to a funnel that becomes gravity dominated and crosses its [sonic point](../../../../../sonic-point.md) before reaching that surface.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
