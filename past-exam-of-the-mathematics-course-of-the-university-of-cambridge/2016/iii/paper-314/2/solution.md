<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $e$ be [specific internal energy](../../../../../specific-internal-energy.md), $Q$ the [heat](../../../../../heat.md) supplied per unit volume per unit time, and $E=\rho(e+|\mathbf u|^2/2)$. For an inviscid [perfect gas](../../../../../ideal-gas.md) in a prescribed [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) $\Phi$, the [fluid total-energy equation](../../../../../fluid-total-energy-equation.md) is

$$
\partial_tE+\nabla\cdot[(E+p)\mathbf u]=-\rho\mathbf u\cdot\nabla\Phi+Q.
$$

There is no gravitational term if no external body is present. For a time-independent $\Phi$, adding [potential energy](../../../../../potential-energy.md) gives the equivalent conservative form $\partial_t(E+\rho\Phi)+\nabla\cdot[(E+p+\rho\Phi)\mathbf u]=Q$. Subtracting the kinetic-energy equation and using [mass conservation](../../../../../mass-conservation.md) gives

$$
\rho\frac{De}{Dt}=-p\nabla\cdot\mathbf u+Q.
$$

For a [perfect gas](../../../../../ideal-gas.md) with constant [specific-heat ratio](../../../../../heat-capacity-ratio.md) $\gamma$, $e=p/[(\gamma-1)\rho]$. The [isothermal equation of state](../../../../../globally-isothermal-equation-of-state.md) therefore makes $e=c_s^2/(\gamma-1)$ constant. Hence **the required [heat](../../../../../heat.md) supply and [heat](../../../../../heat.md) loss are**

$$
\boxed{Q=p\nabla\cdot\mathbf u,\qquad \mathcal L=-Q=-p\nabla\cdot\mathbf u.}
$$

Compression requires cooling; expansion requires heating. The [isothermal sound speed](../../../../../isothermal-sound-speed.md) $c_s$ differs from the [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) $\sqrt\gamma\,c_s$.

Define the isothermal [Mach numbers](../../../../../mach-number.md) by $\mathcal M_i=u_i/c_s$. Orient the normal to a stationary [isothermal shock](../../../../../isothermal-shock.md) along the flow, so the mass flux $j=\rho_1u_1=\rho_2u_2>0$. Tangential velocity is continuous for this planar hydrodynamic shock. Normal [momentum](../../../../../momentum.md) conservation gives

$$
\rho_1u_1^2+c_s^2\rho_1=\rho_2u_2^2+c_s^2\rho_2,
\qquad u_1+\frac{c_s^2}{u_1}=u_2+\frac{c_s^2}{u_2}.
$$

For a genuine discontinuity $u_1\ne u_2$, factorization gives $u_1u_2=c_s^2$. Thus **the [isothermal shock](../../../../../isothermal-shock.md) jump relations** are

$$
\boxed{\frac{\rho_2}{\rho_1}=\frac{u_1}{u_2}=\frac{u_1^2}{c_s^2}=\mathcal M_1^2=\frac1{\mathcal M_2^2},\qquad \mathcal M_1\mathcal M_2=1.}
$$

Across a thin shock, gravitational potential and tangential [kinetic energy](../../../../../kinetic-energy.md) are unchanged. The [specific enthalpy](../../../../../specific-enthalpy.md) $h=\gamma c_s^2/(\gamma-1)$ is the same on both sides, so the energy removed per unit area per unit time is

$$
F_{E,1}-F_{E,2}=\frac j2(u_1^2-u_2^2).
$$

Positive net cooling requires $u_1>u_2$, equivalently $\rho_2>\rho_1$ and $\mathcal M_1>1>\mathcal M_2$. **[Cooling across an isothermal shock](../../../../../cooling-across-an-isothermal-shock.md) permits only compression shocks**; the formal expansion discontinuity requires energy supplied by the surroundings. The continuous state $u_1=u_2$ is not a shock.

For steady radial flow, [mass conservation](../../../../../mass-conservation.md) gives $r^2\rho u_r=\text{constant}$. Differentiating it and eliminating the [mass density](../../../../../density.md) gradient from radial [momentum](../../../../../momentum.md) balance gives

$$
\left(u_r-\frac{c_s^2}{u_r}\right)\frac{du_r}{dr}=\frac{2c_s^2}{r}-\frac{GM}{r^2}.
$$

A regular [sonic point](../../../../../sonic-point.md) has $|u_r|=c_s$, so the right-hand side must vanish there as well. Therefore

$$
\boxed{r_s=\frac{GM}{2c_s^2}.}
$$

This is the [Bondi sonic point](../../../../../bondi-sonic-point.md) for accretion; the same critical radius appears in an isothermal [Parker wind](../../../../../parker-wind.md). A general steady solution need not pass through a [sonic point](../../../../../sonic-point.md), but a smooth transonic one must obey both critical conditions.

Put $x=r/r_s$ and $\mathcal M=|u_r|/c_s$ on a branch whose flow direction is fixed. The radial equation becomes

$$
\left(\mathcal M-\frac1{\mathcal M}\right)\frac{d\mathcal M}{dx}=\frac2x-\frac2{x^2}.
$$

Integrating yields **the [integrated isothermal Bondi flow relation](../../../../../integrated-isothermal-bondi-flow-relation.md)**:

$$
\boxed{\frac12\mathcal M^2-\ln\mathcal M=\frac2x+2\ln x+C.}
$$

For a [transonic branch](../../../../../transonic-branch.md), $x=\mathcal M=1$ gives $C=-3/2$. Expansion about the critical point gives $(\mathcal M-1)^2=(x-1)^2+O((x-1)^3)$, with slope $-1$ for inflow supplied by gas at rest at infinity and slope $+1$ for a transonic outflow.

For [Isothermal Bondi accretion](../../../../../isothermal-bondi-accretion.md), integrate radial [momentum](../../../../../momentum.md) balance once more, using $u_r\to0$ and $\rho\to\rho_\infty$ at infinity:

$$
\frac12u_r^2+c_s^2\ln\frac\rho{\rho_\infty}-\frac{GM}{r}=0.
$$

At the [Bondi sonic point](../../../../../bondi-sonic-point.md), $GM/r_s=2c_s^2$ and $u_r^2=c_s^2$, so $\rho_s=e^{3/2}\rho_\infty$. The positive inward [isothermal Bondi accretion rate](../../../../../isothermal-bondi-accretion-rate.md) is consequently

$$
\boxed{\dot M=-4\pi r^2\rho u_r=4\pi r_s^2\rho_s c_s=\pi e^{3/2}\frac{G^2M^2\rho_\infty}{c_s^3}.}
$$

The critical [mass density](../../../../../density.md) and rate are fixed by the regular transonic solution and the specified reservoir at infinity; an arbitrary subsonic solution does not share this accretion rate.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 314](../../paper-314-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
