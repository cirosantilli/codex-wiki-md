# Paper 46

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper46.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper46.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write the [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass) with [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry) as $\Phi(r)$ and let $\mathbf n$ be the unit [vector](../../../vector-space.md#vector) normal to a [circular orbit](../../../classical-mechanics.md#circular-orbit), oriented in the direction of its [angular velocity](../../../classical-mechanics.md#angular-velocity). Put $\boldsymbol\Omega=\Omega\mathbf n$ and denote the [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) by $\mathbf h=h\mathbf n$. Circular force balance and the [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy) give

$$
\Phi'(r)=r\Omega^2,\qquad h=r^2\Omega,\qquad \varepsilon=\Phi(r)+\frac12r^2\Omega^2.
$$

Differentiating along the family of [circular orbits](../../../classical-mechanics.md#circular-orbit),

$$
\frac{d\varepsilon}{dr}=2r\Omega^2+r^2\Omega\Omega'=\Omega\frac{dh}{dr}.
$$

A change in orbital orientation contributes $h\,d\mathbf n$ to $d\mathbf h$, but $\mathbf n\cdot d\mathbf n=0$. Consequently

$$
\boxed{d\varepsilon=\Omega\,dh=\boldsymbol\Omega\cdot d\mathbf h.}
$$

This [circular-orbit energy gradient](../../../classical-mechanics.md#circular-orbit-energy-gradient) accounts for radial and inclination changes together; [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry) makes the orbital [energy](../../../classical-mechanics.md#energy) independent of the plane.

For either variable-mass particle, $\mathbf H=M\mathbf h$ and $E=M\varepsilon$. Thus $d\mathbf H=M\,d\mathbf h+\mathbf h\,dM$, so

$$
dE=\varepsilon\,dM+M\boldsymbol\Omega\cdot d\mathbf h=(\varepsilon-\Omega h)dM+\boldsymbol\Omega\cdot d\mathbf H.
$$

[Conservation of mass](../../../continuum-mechanics.md#mass-conservation) and [conservation of angular momentum](../../../classical-mechanics.md#conservation-of-angular-momentum) impose $dM_2=-dM_1$, $d\mathbf H_2=-d\mathbf H_1$. Adding the two particle contributions proves

$$
\boxed{dE=\{(\varepsilon_1-\Omega_1h_1)-(\varepsilon_2-\Omega_2h_2)\}\,dM_1+(\boldsymbol\Omega_1-\boldsymbol\Omega_2)\cdot d\mathbf H_1.}
$$

To interpret the signs, label the inner orbit 1 and the outer orbit 2. For $f(r)=\varepsilon-\Omega h$ the first identity gives $f'=-h\Omega'$. The assumed outward decrease of [angular velocity](../../../classical-mechanics.md#angular-velocity) therefore makes $f_1<f_2$, so the mass-exchange part lowers the [energy](../../../classical-mechanics.md#energy) when $dM_1>0$: [mass](../../../classical-mechanics.md#mass) is transferred inward. In a coplanar, co-rotating pair, $\Omega_1>\Omega_2$ and an outward [angular momentum](../../../classical-mechanics.md#angular-momentum) transfer has $d\mathbf H_1=-dH\mathbf n$ with $dH>0$. Its contribution is $-(\Omega_1-\Omega_2)dH<0$.

The [vector](../../../vector-space.md#vector) difference also identifies the inclination-reducing exchange. For a fixed small magnitude of admissible [angular momentum](../../../classical-mechanics.md#angular-momentum) exchange, its [energy](../../../classical-mechanics.md#energy) contribution is most negative when

$$
d\mathbf H_1=-s(\boldsymbol\Omega_1-\boldsymbol\Omega_2),\qquad s>0,
$$

by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). This gives $dE_{\rm angular}=-s|\boldsymbol\Omega_1-\boldsymbol\Omega_2|^2$. Let $q=\mathbf n_1\cdot\mathbf n_2=\cos\iota$ and $H_i=|\mathbf H_i|$, taking fixed particle masses for this exchange. Projecting $d\mathbf H_i$ perpendicular to its own direction gives

$$
d\mathbf n_1=\frac{s\Omega_2}{H_1}(\mathbf n_2-q\mathbf n_1),\qquad d\mathbf n_2=\frac{s\Omega_1}{H_2}(\mathbf n_1-q\mathbf n_2).
$$

Therefore

$$
dq=s(1-q^2)\left(\frac{\Omega_2}{H_1}+\frac{\Omega_1}{H_2}\right)>0\qquad(0<\iota<\pi).
$$

The downhill exchange reduces the relative [orbital inclination](../../../classical-mechanics.md#orbital-inclination). Its inner [angular momentum](../../../classical-mechanics.md#angular-momentum) component is $\mathbf n_1\cdot d\mathbf H_1=-s(\Omega_1-\Omega_2q)<0$; in the aligned limit the outer orbit receives that [angular momentum](../../../classical-mechanics.md#angular-momentum) directly. For strongly inclined orbits, part of the exchange instead cancels differently directed angular momenta as the planes align. Together these gradients explain the tendencies toward inward [mass](../../../classical-mechanics.md#mass) transfer, outward [angular momentum](../../../classical-mechanics.md#angular-momentum) transport and coplanarity.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $M_*$ be the central [mass](../../../classical-mechanics.md#mass), so $\Omega^2=GM_*/r^3$ and the [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy) is $\varepsilon=-GM_*/(2r)$. Define the inward [accretion rate](../../../astrophysics.md#accretion-rate) $\dot M>0$. The rate at which the gas acquires binding [energy](../../../classical-mechanics.md#energy) in moving from $b$ to $a$ is

$$
\boxed{B_{a,b}=\dot M\{\varepsilon(b)-\varepsilon(a)\}=\frac{GM_*\dot M}{2}\left(\frac1a-\frac1b\right).}
$$

The vertically integrated viscous heating per unit horizontal area, including the entire column, is $\bar\nu\Sigma(r\Omega')^2$. Since $r\Omega'=-3\Omega/2$, the dissipated power in the annulus is

$$
D_{a,b}=\int_a^b2\pi r\,\bar\nu\Sigma\frac94\Omega^2\,dr=\frac{3GM_*\dot M}{2}\int_a^b\frac1{r^2}\left(1-\sqrt{\frac{r_{\rm in}}r}\right)dr.
$$

Here the column [integral](../../../calculus.md#integral) already includes dissipation associated with both disk faces; adding another factor of two would double-count it. Performing the elementary [integrals](../../../calculus.md#integral) gives

$$
\boxed{D_{a,b}=GM_*\dot M\left[\frac32\left(\frac1a-\frac1b\right)-\sqrt{r_{\rm in}}\left(a^{-3/2}-b^{-3/2}\right)\right].}
$$

For the whole disk, take $a=r_{\rm in}$ and $b\to\infty$. Both expressions give

$$
\boxed{D_{\rm disk}=B_{\rm disk}=\frac{GM_*\dot M}{2r_{\rm in}}.}
$$

If $a\gg r_{\rm in}$, the bracket $1-\sqrt{r_{\rm in}/r}$ is uniformly close to one throughout the annulus. Comparing the positive [integrals](../../../calculus.md#integral) shows

$$
\frac{D_{a,b}}{B_{a,b}}=3\left[1+O\left(\sqrt{\frac{r_{\rm in}}a}\right)\right],
$$

with the correction negative. Thus **far from the inner edge the [viscous dissipation](../../../stokes-flow.md#viscous-dissipation) is approximately three times the local binding-energy acquisition**.

There is no violation of [conservation of energy](../../../physics.md#conservation-of-energy) because the [viscous torque in an accretion disk](../../../astrophysics.md#viscous-torque-in-an-accretion-disk) also transports mechanical [energy](../../../classical-mechanics.md#energy). The outward [viscous torque in an accretion disk](../../../astrophysics.md#viscous-torque-in-an-accretion-disk) is

$$
\mathcal G=-2\pi\bar\nu\Sigma r^3\Omega'=\dot M\big(\sqrt{GM_*r}-\sqrt{GM_*r_{\rm in}}\big),
$$

and its outward [energy](../../../classical-mechanics.md#energy) flux is $\Omega\mathcal G=GM_*\dot M[r^{-1}-\sqrt{r_{\rm in}}r^{-3/2}]$. The explicit expressions satisfy

$$
\boxed{D_{a,b}=B_{a,b}+\Omega(a)\mathcal G(a)-\Omega(b)\mathcal G(b).}
$$

[Energy](../../../classical-mechanics.md#energy) transported from the inner disk supplies the extra dissipation at larger radii. The torque power vanishes at the [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition) and tends to zero at infinity, leaving global balance. This is [torque transport of energy in a steady accretion disk](../../../astrophysics.md#torque-transport-of-energy-in-a-steady-accretion-disk).

## 2

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The vertical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) equation balances the gradient of the total [pressure](../../../thermodynamics.md#pressure) against gravity. In a [thin disk](../../../astrophysics.md#thin-disk) with [Keplerian rotation](../../../astrophysics.md#keplerian-disk), expanding the central gravitational field about the midplane gives vertical acceleration $-\Omega^2z$, so $p_z=-\rho\Omega^2z$. Disk self-gravity is neglected in this approximation.

The flux-gradient equation is local thermal balance: the upward [radiative flux](../../../astrophysics.md#radiative-flux) increases with height because [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation) dissipates [energy](../../../classical-mechanics.md#energy). For a Newtonian effective [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $\mu$, the volumetric heating rate is $\mu(r\Omega')^2$, which becomes $9\mu\Omega^2/4$ for [Keplerian rotation](../../../astrophysics.md#keplerian-disk). The symbol $\mu$ here is [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity), not [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity); the latter is $\nu=\mu/\rho$.

The [radiative diffusion](../../../astrophysics.md#radiative-diffusion) equation applies to an [optically thick medium](../../../astrophysics.md#optically-thick-medium) in [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium). Its [diffusion](../../../thermodynamics.md#diffusion) coefficient is $c/(3\kappa\rho)$, and the equilibrium radiation [energy density](../../../statistical-physics.md#energy-density) is $u_{\rm rad}=4\sigma T^4/c$. Hence

$$
F=-\frac{c}{3\kappa\rho}\frac{du_{\rm rad}}{dz}=-\frac{16\sigma T^3}{3\kappa\rho}\frac{dT}{dz}.
$$

The minus sign means [energy](../../../classical-mechanics.md#energy) flows down the [temperature](../../../thermodynamics.md#temperature) gradient. Here $\sigma$ is the [Stefan-Boltzmann constant](../../../thermodynamics.md#stefan-boltzmann-constant), $\kappa$ the [opacity](../../../stellar-structure.md#opacity) per unit [mass](../../../classical-mechanics.md#mass), and $c$ the [speed of light](../../../special-relativity.md#speed-of-light). Constant [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) [opacity](../../../stellar-structure.md#opacity) is the adopted transport approximation; [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium) is an additional assumption behind the radiation [equation of state](../../../thermodynamics.md#equation-of-state).

Finally the [equation of state](../../../thermodynamics.md#equation-of-state) adds [ideal gas](../../../thermodynamics.md#ideal-gas) [gas pressure](../../../thermodynamics.md#gas-pressure) $p_g=\rho kT/(\mu_m m_H)$ and isotropic [radiation pressure](../../../thermodynamics.md#radiation-pressure) $p_r=u_{\rm rad}/3=4\sigma T^4/(3c)$. The [Boltzmann constant](../../../thermodynamics.md#boltzmann-constant) is $k$, and $\mu_m m_H$ is the mean [mass](../../../classical-mechanics.md#mass) per gas particle. Both contributions supply the total [pressure](../../../thermodynamics.md#pressure) entering vertical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

In the limiting model with negligible [gas pressure](../../../thermodynamics.md#gas-pressure), $p=p_r=4\sigma T^4/(3c)$. Its gradient is $p_z=16\sigma T^3T_z/(3c)$. Combining [radiative diffusion](../../../astrophysics.md#radiative-diffusion) and [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives

$$
F=-\frac{c}{\kappa\rho}p_z=\frac{c\Omega^2}{\kappa}z.
$$

Because $\kappa$ and $\Omega$ are constant with height at the fixed disk radius,

$$
\frac{dF}{dz}=\frac{c\Omega^2}{\kappa}.
$$

Equating this to the viscous heating rate $9\mu\Omega^2/4$ forces

$$
\boxed{\mu=\frac{4c}{9\kappa}.}
$$

This proves [constant viscosity in radiation-supported vertical balance](../../../astrophysics.md#constant-viscosity-in-radiation-supported-vertical-balance). It fixes the local effective [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) uniquely, independent of height, [surface density](../../../astrophysics.md#surface-density-of-a-disk) and radius within this ideal limiting model. It does not fix a height-independent [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity): $\nu(z)=4c/(9\kappa\rho(z))$ still depends on the local [mass density](../../../fluid-mechanics.md#density).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Set $\mathcal R=k/(\mu_m m_H)$, so $p_g=\mathcal R\rho T$ and the prescribed [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) is $\mu=\alpha\mathcal R\rho T/\Omega$. Keplerian shear and [radiative diffusion](../../../astrophysics.md#radiative-diffusion) then give

$$
F_z=\frac94\alpha\mathcal R\Omega\rho T,\qquad F=-\frac{4\sigma}{3\kappa\rho}(T^4)_z.
$$

Differentiating the second expression, equating it to the first and dividing by $\rho$ gives

$$
\boxed{\frac1\rho\frac{d}{dz}\left(\frac1\rho\frac{dT^4}{dz}\right)+A\Omega T=0,\qquad A=\frac{27\alpha\kappa\mathcal R}{16\sigma}=\frac{27\alpha\kappa k}{16\sigma\mu_m m_H}.}
$$

This reduction uses the gas-pressure [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) closure, not an assumption that [gas pressure](../../../thermodynamics.md#gas-pressure) dominates the hydrostatic support.

For $z\ge0$, introduce the [vertical mass coordinate of a disk](../../../astrophysics.md#vertical-mass-coordinate-of-a-disk)

$$
m(z)=\int_0^z\rho(z')\,dz',\qquad \frac{d}{dm}=\frac1\rho\frac{d}{dz}.
$$

Let $\Sigma=\int_{-z_s}^{z_s}\rho\,dz$ be the full [surface density](../../../astrophysics.md#surface-density-of-a-disk) of a reflection-symmetric disk. The upper surface is at $m_s=\Sigma/2$. With $\zeta=2m/\Sigma$, the [temperature](../../../thermodynamics.md#temperature) equation becomes

$$
\frac4{\Sigma^2}\frac{d^2T^4}{d\zeta^2}+A\Omega T=0.
$$

Write $T=T_*t(\zeta)$ and choose

$$
\boxed{T_*^3=\frac{A\Omega\Sigma^2}4=\frac{27\alpha\kappa\mathcal R\Omega\Sigma^2}{64\sigma}.}
$$

The equation reduces exactly to $(t^4)''+t=0$. Midplane symmetry gives $t'(0)=0$, and the zero surface [temperature](../../../thermodynamics.md#temperature) gives $t(1)=0$. The stipulated unique positive nontrivial dimensionless solution therefore applies at every radius and [surface density](../../../astrophysics.md#surface-density-of-a-disk), with all physical dependence contained in $T_*$ and the mass-coordinate scaling. A zero [temperature](../../../thermodynamics.md#temperature) at the ideal surface does not mean zero escaping flux: $F=-(4\sigma/(3\kappa))\partial_mT^4$ can have a finite nonzero surface value.

The required [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) is the [density-weighted mean kinematic viscosity](../../../fluid-mechanics.md#density-weighted-mean-kinematic-viscosity), not an unweighted vertical mean. Since $\rho\nu=\mu$,

$$
\bar\nu=\frac1\Sigma\int_{-z_s}^{z_s}\mu\,dz=\frac{2\alpha\mathcal R}{\Omega\Sigma}\int_0^{\Sigma/2}T(m)\,dm.
$$

Substituting the dimensionless solution gives, with $I_t=\int_0^1t(\zeta)\,d\zeta$,

$$
\boxed{\bar\nu=\frac{\alpha\mathcal R}{\Omega}\left(\frac{A\Omega\Sigma^2}4\right)^{1/3}I_t=\frac{3I_t}{4}\left(\frac{\alpha^4\kappa\mathcal R^4}{\sigma}\right)^{1/3}\Sigma^{2/3}\Omega^{-2/3}.}
$$

For central [mass](../../../classical-mechanics.md#mass) $M_*$, $\Omega=(GM_*/r^3)^{1/2}$, so the requested explicit radius and surface-density dependence is

$$
\boxed{\bar\nu(r,\Sigma)=\frac{3I_t}{4}\left(\frac{\alpha^4\kappa k^4}{\sigma(\mu_m m_H)^4GM_*}\right)^{1/3}r\Sigma^{2/3}.}
$$

The universal [integral](../../../calculus.md#integral) need not be evaluated. No separate solution for $\rho(z)$ is needed to find this mean: the mass-coordinate transformation removes it from both the [temperature](../../../thermodynamics.md#temperature) equation and the [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) [integral](../../../calculus.md#integral). The result is the [gas-pressure viscosity closure with mixed pressure support](../../../astrophysics.md#gas-pressure-viscosity-closure-with-mixed-pressure-support).

## 3

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Choose a reference [circular orbit](../../../classical-mechanics.md#circular-orbit) at radius $r_0$, rotate the frame with $\boldsymbol\Omega=\Omega(r_0)\mathbf e_z$, and introduce local Cartesian coordinates $x=r-r_0$, $y=r_0(\phi-\Omega t)$ and vertical coordinate $z$. On scales small compared with $r_0$, neglect curvature of the coordinate directions but retain the leading [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation). The background [velocity](../../../classical-mechanics.md#velocity) relative to the rotating frame is

$$
\mathbf u_0=r_0\Omega'(r_0)x\mathbf e_y=-2Ax\mathbf e_y,\qquad A=-\frac12r_0\Omega'(r_0).
$$

Thus $A=3\Omega/4$ for a [Keplerian disk](../../../astrophysics.md#keplerian-disk). The [shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet) retains [Coriolis acceleration](../../../physics.md#coriolis-acceleration) and the linear tidal acceleration. The radial [shearing-sheet tidal potential](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet-tidal-potential) is $-2\Omega Ax^2$, whose force $4\Omega Ax\mathbf e_x$ balances the background [Coriolis acceleration](../../../physics.md#coriolis-acceleration). If vertical tidal gravity is included, its equilibrium contribution is balanced by a background [pressure](../../../thermodynamics.md#pressure) $p_0(z)$ and disappears when that equilibrium is subtracted.

Write the total [velocity](../../../classical-mechanics.md#velocity) as $\mathbf u=\mathbf u_0+\mathbf v$. In the rotating-frame [magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation), background advection is $(\mathbf u_0\cdot\nabla)\mathbf v=-2Ax\partial_y\mathbf v$ and advection of the background by the perturbation is $(\mathbf v\cdot\nabla)\mathbf u_0=-2Av_x\mathbf e_y$. The uniform-viscosity [diffusion](../../../thermodynamics.md#diffusion) of the linear background shear is zero. For a solenoidal [magnetic field](../../../electromagnetism.md#magnetic-field) the [Lorentz force](../../../electromagnetism.md#lorentz-force) per unit [mass](../../../classical-mechanics.md#mass) is

$$
\frac{(\nabla\times\mathbf B)\times\mathbf B}{\mu_0\rho}=\frac{\mathbf B\cdot\nabla\mathbf B}{\mu_0\rho}-\nabla\frac{B^2}{2\mu_0\rho}.
$$

At constant [density](../../../fluid-mechanics.md#density), absorb the magnetic-pressure gradient into $\psi=(p-p_0)/\rho+B^2/(2\mu_0\rho)$. Subtracting the background force balance then gives the stated momentum equation, with the remaining nonlinear advection $\mathbf v\cdot\nabla\mathbf v$, [Coriolis acceleration](../../../physics.md#coriolis-acceleration) $2\boldsymbol\Omega\times\mathbf v$, [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension) and viscous [diffusion](../../../thermodynamics.md#diffusion).

For constant finite [electrical conductivity](../../../electromagnetism.md#electrical-conductivity) $\sigma_e$, put $\eta=(\mu_0\sigma_e)^{-1}$. The [resistive induction equation](../../../astrophysical-fluid-dynamics.md#resistive-induction-equation) with uniform [magnetic diffusivity](../../../astrophysical-fluid-dynamics.md#magnetic-diffusivity) is $\partial_t\mathbf B+\mathbf u\cdot\nabla\mathbf B=\mathbf B\cdot\nabla\mathbf u+\eta\nabla^2\mathbf B$. Substituting the background shear supplies the term $-2AB_x\mathbf e_y$ and the same background-advection operator as in the momentum equation. The two further conditions are

$$
\boxed{\nabla\cdot\mathbf v=0,\qquad\nabla\cdot\mathbf B=0.}
$$

They express [incompressibility](../../../fluid-mechanics.md#incompressible-flow) and the absence of [magnetic monopoles](../../../physics.md#magnetic-monopole), respectively.

Now take real [plane waves](../../../quantum-mechanics.md#plane-wave) with common phase $\vartheta=\mathbf k(t)\cdot\mathbf x$ and real [wavevector](../../../continuum-mechanics.md#wavevector). The solenoidal conditions become

$$
\mathbf k\cdot\widetilde{\mathbf v}=0,\qquad \mathbf k\cdot\widetilde{\mathbf B}=0.
$$

Every field depends on position only through $\vartheta$. Hence for either transverse [vector](../../../vector-space.md#vector) field $\mathbf P$ and either wave field $\mathbf Q$, $(\mathbf P\cdot\nabla)\mathbf Q=(\mathbf P\cdot\mathbf k)\partial_\vartheta\mathbf Q=0$. This proves that all the displayed quadratic advection and tension terms vanish pointwise, including products involving conjugate [amplitudes](../../../physics.md#wave-amplitude). These waves are therefore exact solutions at finite [amplitude](../../../physics.md#wave-amplitude), not merely a [linearization](../../../algebra.md#linearization).

Acting with $D_0=\partial_t-2Ax\partial_y$ on the phase yields

$$
D_0\vartheta=(\dot k_x-2Ak_y)x+\dot k_y y+\dot k_z z.
$$

Canceling its position-dependent part requires

$$
\boxed{\dot k_x=2Ak_y,\qquad\dot k_y=\dot k_z=0,\qquad k_x(t)=k_{x0}+2Ak_yt.}
$$

The remaining [amplitude](../../../physics.md#wave-amplitude) equations are

$$
\boxed{\dot{\widetilde{\mathbf v}}-2A\widetilde v_x\mathbf e_y+2\boldsymbol\Omega\times\widetilde{\mathbf v}=-i\mathbf k\widetilde\psi-\nu k^2\widetilde{\mathbf v},\qquad\dot{\widetilde{\mathbf B}}=-2A\widetilde B_x\mathbf e_y-\eta k^2\widetilde{\mathbf B}.}
$$

Differentiating the [velocity](../../../classical-mechanics.md#velocity) constraint determines the [pressure](../../../thermodynamics.md#pressure) [amplitude](../../../physics.md#wave-amplitude):

$$
i k^2\widetilde\psi=4Ak_y\widetilde v_x-2\mathbf k\cdot(\boldsymbol\Omega\times\widetilde{\mathbf v}).
$$

The [resistive induction equation](../../../astrophysical-fluid-dynamics.md#resistive-induction-equation) preserves its constraint because $\dot{\mathbf k}\cdot\widetilde{\mathbf B}=2Ak_y\widetilde B_x$ cancels the corresponding shear term in $\mathbf k\cdot\dot{\widetilde{\mathbf B}}$. The specified [magnetic field](../../../electromagnetism.md#magnetic-field) has no spatially uniform part. Thus there is no background [magnetic field](../../../electromagnetism.md#magnetic-field) producing an additional linear magnetic-tension coupling. The scalar $\psi$ is the modified [pressure](../../../thermodynamics.md#pressure); the physical [pressure](../../../thermodynamics.md#pressure) can include a constant and a second spatial harmonic from $-B^2/(2\mu_0)$ while $\psi$ retains the stipulated plane-wave form. This is an exact [zero-mean magnetic shearing wave](../../../gravitational-instability-of-an-astrophysical-disk.md#zero-mean-magnetic-shearing-wave).

For decay, take the real part of the [scalar product](../../../linear-algebra.md#dot-product) of the velocity-amplitude equation with its [complex conjugate](../../../complex-analysis.md#complex-conjugate). [Pressure](../../../thermodynamics.md#pressure) does no work because $\mathbf k\cdot\widetilde{\mathbf v}=0$, and the real part of Coriolis work is zero. Therefore

$$
\frac{d}{dt}|\widetilde{\mathbf v}|^2=4A\operatorname{Re}(\widetilde v_x\widetilde v_y^*)-2\nu k^2|\widetilde{\mathbf v}|^2\le(2|A|-2\nu k^2)|\widetilde{\mathbf v}|^2.
$$

The [resistive induction equation](../../../astrophysical-fluid-dynamics.md#resistive-induction-equation) similarly gives

$$
\frac{d}{dt}|\widetilde{\mathbf B}|^2=-4A\operatorname{Re}(\widetilde B_x\widetilde B_y^*)-2\eta k^2|\widetilde{\mathbf B}|^2\le(2|A|-2\eta k^2)|\widetilde{\mathbf B}|^2,
$$

using $2|u_xu_y|\le|\mathbf u|^2$. Integrating these differential inequalities, define

$$
J(t)=\int_0^t k(s)^2\,ds=(k_{x0}^2+k_y^2+k_z^2)t+2Ak_{x0}k_yt^2+\frac43A^2k_y^2t^3.
$$

Then

$$
|\widetilde{\mathbf v}(t)|^2\le|\widetilde{\mathbf v}(0)|^2e^{2|A|t-2\nu J(t)},\qquad |\widetilde{\mathbf B}(t)|^2\le|\widetilde{\mathbf B}(0)|^2e^{2|A|t-2\eta J(t)}.
$$

A non-axisymmetric wave has $k_y\ne0$. For nonzero differential shear and positive $\nu,\eta$, the negative cubic terms dominate the linear upper bound on shear work. Consequently

$$
\boxed{\widetilde{\mathbf v}(t)\longrightarrow0,\qquad\widetilde{\mathbf B}(t)\longrightarrow0\quad(t\to\infty).}
$$

This [cubic-exponent decay of a nonaxisymmetric shearing wave](../../../gravitational-instability-of-an-astrophysical-disk.md#cubic-exponent-decay-of-a-nonaxisymmetric-shearing-wave) allows transient [energy](../../../classical-mechanics.md#energy) growth before the winding to short radial wavelengths makes [diffusion](../../../thermodynamics.md#diffusion) dominant. The magnetic [amplitudes](../../../physics.md#wave-amplitude) can also be written explicitly as

$$
\widetilde{\mathbf B}(t)=e^{-\eta J(t)}\big(\widetilde B_x(0),\ \widetilde B_y(0)-2At\widetilde B_x(0),\ \widetilde B_z(0)\big),
$$

which confirms the damping independently. Positivity of the dissipative coefficients is necessary: with $k_z=0$, an inviscid vertical [velocity](../../../classical-mechanics.md#velocity) [amplitude](../../../physics.md#wave-amplitude) can remain constant, and an ideal vertical magnetic [amplitude](../../../physics.md#wave-amplitude) can remain constant when $\eta=0$. The asserted decay applies to the viscous, finitely conducting model; taking an ideal limit before the long-time limit changes the conclusion.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
