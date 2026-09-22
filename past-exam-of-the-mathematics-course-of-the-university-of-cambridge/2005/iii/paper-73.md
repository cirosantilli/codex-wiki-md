# Paper 73

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper73.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper73.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The first equation is vertical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium): the upward [pressure gradient](../../../fluid-mechanics.md#pressure-gradient) balances the central [mass](../../../classical-mechanics.md#mass)'s vertical gravitational force. For $|z|\ll r$, the point-mass acceleration is $-GMz/(r^2+z^2)^{3/2}\simeq-\Omega_K^2z$, where [Keplerian rotation](../../../astrophysics.md#keplerian-disk) gives $\Omega_K^2=GM/r^3$. The disc's [self-gravity](../../../classical-mechanics.md#self-gravity) and vertical inertia are neglected.

The second equation is local thermal balance. The divergence of the vertical [radiative flux](../../../astrophysics.md#radiative-flux) equals [viscous dissipation](../../../stokes-flow.md#viscous-dissipation). In the convention of this [alpha disk](../../../astrophysics.md#alpha-disk), $\nu=\alpha p/(\rho\Omega)$, and the dominant [Keplerian shear](../../../planetary-science.md#keplerian-shear) has $r\,d\Omega/dr=-3\Omega/2$. Therefore

$$
q^+=\rho\nu\left(r\frac{d\Omega}{dr}\right)^2=\frac94\alpha\Omega p=\frac{\partial F}{\partial z}.
$$

The [radiative flux](../../../astrophysics.md#radiative-flux) increases from zero at the symmetric midplane to a positive outgoing value at the upper surface. Radial heat transport, thermal [advection](../../../fluid-mechanics.md#advection) and rapid storage of thermal [energy](../../../classical-mechanics.md#energy) are excluded from this local balance.

The third equation is [radiative diffusion](../../../astrophysics.md#radiative-diffusion), equivalently

$$
F=-\frac{16\sigma T^3}{3\kappa\rho}\frac{\partial T}{\partial z}.
$$

It applies to optically thick material, with $\kappa$ the opacity per unit [mass](../../../classical-mechanics.md#mass) and $\sigma$ the [Stefan-Boltzmann constant](../../../thermodynamics.md#stefan-boltzmann-constant). Here constant [electron-scattering opacity](../../../stellar-structure.md#electron-scattering-opacity) represents [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering); the formula uses a diffusive, nearly thermal radiation field. Positive upward [flux](../../../physics.md#flux) requires [temperature](../../../thermodynamics.md#temperature) to decrease upwards.

The final equation is the [ideal gas](../../../thermodynamics.md#ideal-gas) [pressure](../../../thermodynamics.md#pressure) law, with [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight) $\mu_m$ in proton-mass units. Writing $\mathcal R=k/(\mu_m m_p)$ gives $p=\mathcal R\rho T$. The [pressure](../../../thermodynamics.md#pressure) is [gas pressure](../../../thermodynamics.md#gas-pressure) because [radiation pressure](../../../thermodynamics.md#radiation-pressure) is assumed negligible. **The four equations express vertical support, local heating balance, diffusive cooling and the gas equation of state.**

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Work at one radius and write $\mathcal R=k/(\mu_m m_p)$. Use the [surface density](../../../astrophysics.md#surface-density-of-a-disk) to fix the [mass density](../../../fluid-mechanics.md#density) normalization and introduce the height scale

$$
h^6=\frac{3\alpha\kappa\Sigma^2\mathcal R^4}{16\sigma\Omega^5}.
$$

Choose the dimensionless variables

$$
z=h\zeta,\qquad \rho=\frac\Sigma h D,\qquad p=\Sigma\Omega^2hP,\qquad T=\frac{\Omega^2h^2}{\mathcal R}\Theta,\qquad F=\alpha\Sigma\Omega^3h^2Q.
$$

The [pressure](../../../thermodynamics.md#pressure) and [temperature](../../../thermodynamics.md#temperature) scales make the hydrostatic and [ideal gas](../../../thermodynamics.md#ideal-gas) equations parameter-free. The [flux](../../../physics.md#flux) scale fixes the heating coefficient at $9/4$, and the choice of $h$ makes the diffusion coefficient unity. Direct substitution gives the universal [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation)

$$
\boxed{\frac{dP}{d\zeta}=-D\zeta,\qquad \frac{dQ}{d\zeta}=\frac94P,\qquad \frac{d\Theta}{d\zeta}=-\frac{DQ}{\Theta^3},\qquad P=D\Theta.}
$$

For example, the dimensionless coefficient in the [temperature](../../../thermodynamics.md#temperature) equation is $3\alpha\kappa\Sigma^2\mathcal R^4/(16\sigma\Omega^5h^6)=1$.

Let the upper free surface be at $\zeta=\zeta_s$, so its physical semithickness is $H=h\zeta_s$. Midplane [symmetry](../../../physics.md#symmetry-physics) and the [radiative-zero disk surface](../../../astrophysics.md#radiative-zero-disk-surface) conditions give

$$
\boxed{Q(0)=0,\qquad P(\zeta_s)=\Theta(\zeta_s)=0,\qquad 2\int_0^{\zeta_s}D\,d\zeta=1.}
$$

The last condition is precisely $\Sigma=\int_{-H}^H\rho\,dz$. The unknown surface position and the two positive midplane values $P(0),\Theta(0)$ are determined as part of the normalized [boundary value problem](../../../differential-equation.md#boundary-value-problem). [Symmetry](../../../physics.md#symmetry-physics) makes $P,D,\Theta$ even and $Q$ odd; $P'(0)=\Theta'(0)=0$ already follow from the equations and are not additional independent [boundary conditions](../../../differential-equation.md#boundary-condition).

The zero conditions do not mean zero surface [flux](../../../physics.md#flux). Integrating the heating equation gives $Q(\zeta_s)=(9/4)\int_0^{\zeta_s}P\,d\zeta>0$. Near a regular surface with finite outgoing [flux](../../../physics.md#flux), dividing the hydrostatic equation by the [temperature](../../../thermodynamics.md#temperature) equation yields $dP/d\Theta\simeq\zeta_s\Theta^3/Q_s$. Thus $P\propto\Theta^4$, $D\propto\Theta^3$ and $\Theta\propto\zeta_s-\zeta$, so [mass density](../../../fluid-mechanics.md#density) also vanishes. The apparent singular quotient in the diffusion equation has a finite regular limit. All [boundary conditions](../../../differential-equation.md#boundary-condition) and equations are independent of the physical parameters: this is [homologous vertical structure of a constant-opacity alpha disk](../../../astrophysics.md#homologous-vertical-structure-of-a-constant-opacity-alpha-disk).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The [density-weighted mean kinematic viscosity](../../../fluid-mechanics.md#density-weighted-mean-kinematic-viscosity) is

$$
\bar\nu=\frac1\Sigma\int_{-H}^H\rho\nu\,dz=\frac\alpha{\Sigma\Omega}\int_{-H}^H p\,dz,
$$

using $\nu=\alpha p/(\rho\Omega)$. Under the preceding rescaling, let

$$
I_P=\int_{-\zeta_s}^{\zeta_s}P(\zeta)\,d\zeta.
$$

Uniqueness of the universal dimensionless solution makes $I_P$ a positive numerical constant independent of $\alpha,\Omega,\kappa,\Sigma,\mathcal R$. Hence

$$
\bar\nu=\alpha\Omega h^2 I_P=\left(\frac3{16}\right)^{1/3}I_P\,\alpha^{4/3}\left(\frac\kappa\sigma\right)^{1/3}\mathcal R^{4/3}\Sigma^{2/3}\Omega^{-2/3}.
$$

For [Keplerian rotation](../../../astrophysics.md#keplerian-disk), $\Omega^{-2/3}=(GM)^{-1/3}r$. The [constant-opacity gas-pressure disk viscosity law](../../../astrophysics.md#constant-opacity-gas-pressure-disk-viscosity-law) is therefore

$$
\boxed{\bar\nu=C\alpha^{4/3}(GM)^{-1/3}\left(\frac\kappa\sigma\right)^{1/3}\left(\frac{\mu_m m_p}{k}\right)^{-4/3}r\Sigma^{2/3},\qquad C=\left(\frac3{16}\right)^{1/3}I_P.}
$$

The particular scaling convention changes the representation of $I_P$ but not this physical law. Its nontrivial powers come from balancing viscous heating, diffusive cooling and vertical support together, rather than assuming a fixed [temperature](../../../thermodynamics.md#temperature) or thickness.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Estimate characteristic bulk terms. Put $\epsilon=H/r\ll1$ and assume smooth radial variation on scale $r$, secular evolution, and $\alpha\lesssim1$. Vertical support gives $c_s^2\sim p/\rho\sim\Omega^2H^2$, while the [alpha disk](../../../astrophysics.md#alpha-disk) prescription and slow accretion imply

$$
\nu\sim\alpha\Omega H^2,\qquad u_r\sim\frac\nu r,\qquad u_z\sim\frac Hr u_r.
$$

These velocity estimates follow from the viscous radial evolution scale and [mass conservation](../../../continuum-mechanics.md#mass-conservation). They are estimates for a slowly evolving thin disc, not a claim that geometric thinness excludes independently forced rapid vertical motion.

For vertical balance, the exact central force expands as

$$
\frac{GMz}{(r^2+z^2)^{3/2}}=\Omega_K^2z\left[1-\frac32\frac{z^2}{r^2}+O\!\left(\frac{z^4}{r^4}\right)\right].
$$

At $z\sim H$, the neglected correction has magnitude $\rho\Omega^2H\epsilon^2$, compared with the retained force $\rho\Omega^2H$. Radial [pressure](../../../thermodynamics.md#pressure) support similarly changes the rotation from its Keplerian value by

$$
\frac{\delta\Omega^2}{\Omega_K^2}\sim\frac{c_s^2}{r^2\Omega_K^2}=O(\epsilon^2).
$$

Vertical meridional inertia scales as $u_r u_z/r$ or $u_z^2/H$, both $O(\alpha^2\epsilon^4\Omega^2H)$. Meridional viscous accelerations can scale as $\nu u_z/H^2$ or $\nu u_r/(rH)$, both $O(\alpha^2\epsilon^2\Omega^2H)$. Thus the gravity correction and possible viscous correction give

$$
\boxed{\frac{\text{neglected vertical-force terms}}{\rho\Omega^2H}=O(\epsilon^2).}
$$

Some omitted terms are smaller than this leading order.

For the heating equation, the retained dissipation is $q_0^+\sim\rho\nu\Omega^2\sim\alpha p\Omega$. Radial [pressure](../../../thermodynamics.md#pressure) support and the finite-height correction change the dominant shear by a relative $O(\epsilon^2)$. Smooth vertical variation of the rotation gives $\partial_z(r\Omega)=O(\epsilon\Omega)$, whose additional squared shear contributes $O(\epsilon^2q_0^+)$. Meridional shear of order $u_r/H$ gives an additional relative $O(\alpha^2\epsilon^2)$ contribution.

Thermal [advection](../../../fluid-mechanics.md#advection) and compressional work are of order $\rho u_r c_s^2/r$ and $p u_r/r$, respectively. Relative to $\alpha p\Omega$ they are $O(\epsilon^2)$. Thermal storage on the viscous evolution timescale $t_\nu\sim r^2/\nu$ has the same order, since $p/t_\nu\sim\alpha p\Omega\epsilon^2$. For [radiative diffusion](../../../astrophysics.md#radiative-diffusion) with the same local diffusivity in different directions, smooth gradients give $F_r/F_z\sim H/r$, so

$$
\frac{r^{-1}\partial_r(rF_r)}{\partial_zF_z}\sim\frac{F_r/r}{F_z/H}=O(\epsilon^2).
$$

Consequently

$$
\boxed{\frac{\text{neglected local-energy terms}}{(9/4)\alpha\Omega p}=O\!\left((H/r)^2\right).}
$$

This is the [thin-accretion-disk truncation error](../../../astrophysics.md#thin-accretion-disk-truncation-error) for the secular, radially smooth approximation. Neglect of disc [self-gravity](../../../classical-mechanics.md#self-gravity) and [radiation pressure](../../../thermodynamics.md#radiation-pressure), optical thickness, the opacity model and the idealized zero surface boundary have their own validity conditions; their errors do not become small solely because $H/r$ does. Near a sharp radial [boundary layer](../../../continuum-mechanics.md#boundary-layer) or during thermal evolution on the heating timescale, the above estimates need not apply.

## 2

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The variable $\psi$ is a [rotating-flow pressure potential](../../../physics.md#rotating-flow-pressure-potential) including the conservative body-force and centrifugal potentials. For constant [mass density](../../../fluid-mechanics.md#density),

$$
\boxed{\psi=\frac p\rho+\Phi-\frac12|\boldsymbol\Omega\times\mathbf r|^2,}
$$

up to an additive function of time, where $\Phi$ is any imposed conservative potential. The last term is the [centrifugal potential](../../../physics.md#centrifugal-potential); its negative gradient is the centrifugal acceleration. The [Coriolis force](../../../physics.md#coriolis-force) remains explicit in the equation because it is velocity-dependent and cannot be absorbed into a scalar position potential.

The further constraint is [incompressible flow](../../../fluid-mechanics.md#incompressible-flow):

$$
\boxed{\nabla\cdot\mathbf u=0.}
$$

For the specified shear, $\mathbf u_0\cdot\nabla\mathbf u_0=0$ and $\nabla^2\mathbf u_0=0$. Its [Coriolis acceleration](../../../physics.md#coriolis-acceleration) is $4\Omega Ax\mathbf e_x$, so the corresponding total basic [pressure](../../../thermodynamics.md#pressure) potential can be chosen as $\psi_0=-2\Omega Ax^2$. This supplies the force balance required for the basic state used below.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let the perturbation phase be $\vartheta=\mathbf k(t)\cdot\mathbf r$ and write $\psi=\psi_0+\operatorname{Re}[\Pi(t)e^{i\vartheta}]$. [Incompressible flow](../../../fluid-mechanics.md#incompressible-flow) imposes $\mathbf k\cdot\mathbf v=0$. Applying the background advective derivative to the phase gives

$$
(\partial_t+\mathbf u_0\cdot\nabla)\vartheta=\dot{\mathbf k}\cdot\mathbf r-2Axk_y.
$$

Cancel this position-dependent phase by choosing

$$
\boxed{\dot k_x=2Ak_y,\qquad \dot k_y=\dot k_z=0,\qquad k_x(t)=k_x(t_0)+2Ak_y(t-t_0).}
$$

The perturbation acting on the basic flow gives $(\mathbf u'\cdot\nabla)\mathbf u_0=-2Au_x'\mathbf e_y$. Its self-advection vanishes exactly: the physical velocity $\mathbf u'$ is perpendicular to $\mathbf k$, while every spatial derivative of $\mathbf u'$ is proportional to a component of $\mathbf k$. Thus $\mathbf u'\cdot\nabla\mathbf u'=0$, including the products between the complex mode and its conjugate. Substituting into the full [Navier-Stokes equation](../../../viscous-fluid-flow.md#navier-stokes-equation) therefore gives an [exact incompressible shearing wave](../../../gravitational-instability-of-an-astrophysical-disk.md#exact-incompressible-shearing-wave), with no small-amplitude approximation:

$$
\boxed{\dot{\mathbf v}-2Av_x\mathbf e_y+2\Omega\mathbf e_z\times\mathbf v=-i\mathbf k\Pi-\nu k^2\mathbf v,\qquad \mathbf k\cdot\mathbf v=0.}
$$

In components these equations are

$$
\begin{aligned}
\dot v_x-2\Omega v_y&=-ik_x\Pi-\nu k^2v_x,\\
\dot v_y+2(\Omega-A)v_x&=-ik_y\Pi-\nu k^2v_y,\\
\dot v_z&=-ik_z\Pi-\nu k^2v_z.
\end{aligned}
$$

Differentiating the transversality constraint closes the [pressure](../../../thermodynamics.md#pressure):

$$
\boxed{ik^2\Pi=2\Omega k_xv_y+(4A-2\Omega)k_yv_x.}
$$

The coefficient $4A$ includes both the shear term in the momentum equation and $\dot{\mathbf k}\cdot\mathbf v$; treating the [wavevector](../../../continuum-mechanics.md#wavevector) as fixed would miss one contribution. Initial data with $\mathbf k(t_0)\cdot\mathbf v(t_0)=0$ remain transverse under this closed evolution. These [shearing waves](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-wave) are exact in an unbounded local shear flow or with compatible shearing-periodic boundaries; arbitrary rigid [boundary conditions](../../../differential-equation.md#boundary-condition) need not admit a single such wave.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For $k_z=v_z=0$, define the complex vertical [vorticity](../../../fluid-mechanics.md#vorticity) [amplitude](../../../physics.md#wave-amplitude)

$$
Z=i(k_xv_y-k_yv_x).
$$

Take the curl of the [amplitude](../../../physics.md#wave-amplitude) equations, including $\dot k_x=2Ak_y$. Incompressibility cancels the [pressure](../../../thermodynamics.md#pressure) and rotation terms, giving

$$
\dot Z=-\nu k^2Z.
$$

Equivalently, the uniform basic absolute [vorticity](../../../fluid-mechanics.md#vorticity) has no gradient for the perturbation to advect. The general [two-dimensional viscous shearing wave](../../../gravitational-instability-of-an-astrophysical-disk.md#two-dimensional-viscous-shearing-wave) solution is

$$
\boxed{Z(t)=Z_0\exp\!\left[-\nu\int_{t_0}^t(k_x(s)^2+k_y^2)\,ds\right],\qquad v_x=\frac{ik_yZ}{k^2},\qquad v_y=-\frac{ik_xZ}{k^2},}
$$

where $Z_0$ is an arbitrary complex constant and $k_x(t_0)$ is an arbitrary real initial radial [wavenumber](../../../wave-equation.md#wavenumber). The perturbation [pressure](../../../thermodynamics.md#pressure) follows from part (ii), or explicitly $\Pi=(4Ak_y^2-2\Omega k^2)Z/k^4$.

For $A\ne0$, shift the time origin to the swing $k_x=0$ and put $T=k_x/k_y=2At$, $T_0=2At_0$ and $\mathrm{Re}=A/(\nu k_y^2)$. Then

$$
k^2=k_y^2(1+T^2),\qquad Z(T)=Z_0\exp\!\left[-\frac{g(T)-g(T_0)}{2\mathrm{Re}}\right],\qquad g(T)=T+\frac{T^3}{3}.
$$

The spatially averaged perturbation kinetic-energy [mass density](../../../fluid-mechanics.md#density) is $E=\rho\langle|\mathbf u'|^2\rangle/2=\rho|\mathbf v|^2/4$, and $|\mathbf v|^2=|Z|^2/k^2$. Consequently

$$
\boxed{\frac{E(T)}{E(T_0)}=\frac{1+T_0^2}{1+T^2}\exp\!\left[-\frac{g(T)-g(T_0)}{\mathrm{Re}}\right],\qquad E(T)\propto\frac{e^{-(T+T^3/3)/\mathrm{Re}}}{1+T^2}.}
$$

The proportionality constant depends on the initial data; the exponential profile is not a claim of infinite physical growth from the remote past. For $A>0$, leading waves with $T<0$ can gain velocity [amplitude](../../../physics.md#wave-amplitude) as their [wavevector](../../../continuum-mechanics.md#wavevector) magnitude decreases, before [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) and later winding damp them. This is the [Orr mechanism](../../../hydrodynamic-stability.md#orr-mechanism), and it is independent of uniform rotation for these two-dimensional disturbances.

If $A=0$, the [wavevector](../../../continuum-mechanics.md#wavevector) is constant and $\mathbf v(t)=\mathbf v(t_0)e^{-\nu k^2(t-t_0)}$, so there is no shear amplification. The formulas with the physical-time integral remain valid, although $T=2At$ is no longer a useful coordinate. The high-positive-Reynolds-number case in the next part takes $A>0$.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For a fixed $\mathrm{Re}\gg1$, optimize the gain over the initial wave tilt and a later observation time. From the [energy](../../../classical-mechanics.md#energy) profile,

$$
\frac{d\log E}{dT}=-\frac{2T}{1+T^2}-\frac{1+T^2}{\mathrm{Re}}.
$$

Its stationary points satisfy

$$
-2\mathrm{Re}\,T=(1+T^2)^2.
$$

There are two negative roots in the high-Reynolds-number regime: an early [energy](../../../classical-mechanics.md#energy) minimum and a later maximum. Write them as $T_-$ and $T_+$. Balancing the large-$|T|$ terms for the early root and the small-$|T|$ terms for the late root gives

$$
T_-=-(2\mathrm{Re})^{1/3}\bigl[1+O(\mathrm{Re}^{-2/3})\bigr],\qquad T_+=-\frac1{2\mathrm{Re}}+O(\mathrm{Re}^{-3}).
$$

Thus the optimum disturbance starts as a sufficiently tightly wound leading wave and reaches its peak slightly before $k_x=0$; finite [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) shifts the peak away from the inviscid swing.

Normalize its initial [energy](../../../classical-mechanics.md#energy) at $T_-$. The exact maximum ratio is

$$
G_{\max}=\frac{1+T_-^2}{1+T_+^2}\exp\!\left[\frac{g(T_-)-g(T_+)}{\mathrm{Re}}\right].
$$

The prefactor is asymptotic to $(2\mathrm{Re})^{2/3}$, while $g(T_-)/\mathrm{Re}\to-2/3$ and $g(T_+)/\mathrm{Re}\to0$. Therefore [optimal transient amplification of a viscous shearing wave](../../../gravitational-instability-of-an-astrophysical-disk.md#optimal-transient-amplification-of-a-viscous-shearing-wave) gives

$$
\boxed{G_{\max}\sim\left(\frac{2\mathrm{Re}}e\right)^{2/3},\qquad \mathrm{Re}=\frac A{\nu k_y^2}.}
$$

The time between the optimum initial tilt and the peak is approximately $(2\mathrm{Re})^{1/3}/(2A)$. Without [viscosity](../../../fluid-mechanics.md#dynamic-viscosity), ever larger initial tilts would allow unbounded gain; [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) damps them before they can swing, selecting the finite optimum. The coefficient above uses the paper's [Reynolds number](../../../fluid-mechanics.md#reynolds-number) based on $A$, not one based on the full shear rate $2A$.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

For axisymmetric disturbances, $k_y=0$, the [wavevector](../../../continuum-mechanics.md#wavevector) is fixed, so there is no winding/swing mechanism. Take $k_z\ne0$ and set $\chi=k_z^2/k^2$. Eliminating [pressure](../../../thermodynamics.md#pressure) with incompressibility gives

$$
\dot v_x=2\Omega\chi v_y-\nu k^2v_x,\qquad\dot v_y=-2(\Omega-A)v_x-\nu k^2v_y,\qquad v_z=-\frac{k_x}{k_z}v_x.
$$

The [axisymmetric incompressible epicyclic wave](../../../astrophysics.md#axisymmetric-incompressible-epicyclic-wave) has inviscid frequency

$$
\omega^2=\kappa_r^2\chi,\qquad\kappa_r^2=4\Omega(\Omega-A),
$$

where $\kappa_r$ is the [radial epicyclic frequency](../../../astrophysics.md#radial-epicyclic-frequency).

In a Keplerian flow $A=3\Omega/4$ and $\kappa_r=\Omega$. The axisymmetric disturbances therefore execute stable inertial/epicyclic oscillations, with viscous [amplitude](../../../physics.md#wave-amplitude) decay $e^{-\nu k^2t}$. Rotation opposes sustained radial displacement through angular-momentum conservation. There can be bounded exchanges of [kinetic energy](../../../classical-mechanics.md#kinetic-energy) between components, but no large Reynolds-number-dependent amplification of this axisymmetric family. Indeed, with $w=v_x/\sqrt\chi$, inviscid motion conserves

$$
(\Omega-A)|w|^2+\Omega|v_y|^2.
$$

Since the physical velocity norm is $|w|^2+|v_y|^2$, Keplerian [energy](../../../classical-mechanics.md#energy) amplification is at most $\Omega/(\Omega-A)=4$; [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) can only reduce that bound. A pure initial azimuthal disturbance can attain the inviscid factor four after a quarter epicyclic period. By contrast, the two-dimensional nonaxisymmetric [Orr mechanism](../../../hydrodynamic-stability.md#orr-mechanism) remains available in a Keplerian flow and has the $\mathrm{Re}^{2/3}$ gain derived above.

In non-rotating shear, $\Omega=0$ while $A$ remains nonzero. The axisymmetric solution is

$$
v_x=C_xe^{-\nu k^2\tau},\qquad v_y=(C_y+2A\tau C_x)e^{-\nu k^2\tau},\qquad\tau=t-t_0.
$$

Cross-stream motion transports the basic shear and generates an azimuthal streak: this is the [lift-up effect](../../../hydrodynamic-stability.md#lift-up-effect). Inviscid azimuthal velocity grows linearly and its [energy](../../../classical-mechanics.md#energy) quadratically, rather than oscillating. With [viscosity](../../../fluid-mechanics.md#dynamic-viscosity), the gain for a suitable initial cross-stream disturbance scales as $[A/(\nu k^2)]^2$ at large [Reynolds number](../../../fluid-mechanics.md#reynolds-number), appreciably stronger than the two-dimensional $\mathrm{Re}^{2/3}$ scaling. For instance, $C_y=0$ and fixed $\chi>0$ give the leading optimized gain $4\chi A^2/(e^2\nu^2k^4)$ at $\tau\simeq1/(\nu k^2)$. Neither mechanism is an exponentially growing hydrodynamic [normal mode](../../../wave-equation.md#normal-mode). **Rotation bounds axisymmetric lift-up in [Keplerian shear](../../../planetary-science.md#keplerian-shear); without rotation, lift-up gives strong algebraic transient growth.** If $k_z=0$ as well as $k_y=0$, incompressibility forces $v_x=0$ and removes this coupling altogether.

## 3

↑ **Parent:** [Paper 73](paper-73.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Consider a local [shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet) centered at a circular orbit. Take uniform [mass density](../../../fluid-mechanics.md#density), background velocity $\mathbf u_0=-2Ax\mathbf e_y$, rotation $\boldsymbol\Omega=\Omega\mathbf e_z$ and a weak uniform vertical [magnetic field](../../../electromagnetism.md#magnetic-field) $\mathbf B_0=B_0\mathbf e_z$. Here

$$
A=-\frac12r\frac{d\Omega}{dr},\qquad \kappa_r^2=4\Omega(\Omega-A).
$$

Use [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics), neglect [viscosity](../../../fluid-mechanics.md#dynamic-viscosity), [magnetic diffusion](../../../astrophysical-fluid-dynamics.md#magnetic-diffusion) and vertical stratification, and take incompressible axisymmetric disturbances proportional to $e^{ikz-i\omega t}$. They have horizontal velocity and field perturbations. Let $\mathbf b=\delta\mathbf B/\sqrt{\mu_0\rho}$ be the magnetic perturbation in velocity units, $v_A=B_0/\sqrt{\mu_0\rho}$ the [Alfvén speed](../../../astrophysical-fluid-dynamics.md#alfven-speed) and $\omega_A=kv_A$ the [Alfvén frequency](../../../astrophysical-fluid-dynamics.md#alfven-frequency). Magnetic [pressure](../../../thermodynamics.md#pressure) can be included in the perturbation's total [pressure](../../../thermodynamics.md#pressure); the horizontal Lorentz force for this mode is the [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension) term $i\omega_A\mathbf b$.

Linearizing momentum and induction gives

$$
\begin{aligned}
-i\omega u_x-2\Omega u_y&=i\omega_A b_x,\\
-i\omega u_y+2(\Omega-A)u_x&=i\omega_A b_y,\\
-i\omega b_x&=i\omega_Au_x,\\
-i\omega b_y&=-2Ab_x+i\omega_Au_y.
\end{aligned}
$$

The term $-2Ab_x$ winds a radial magnetic perturbation into an azimuthal one. Omitting it would remove the shear's magnetic [energy](../../../classical-mechanics.md#energy) source and give the wrong stability criterion.

A useful elimination that also covers neutral modes introduces the fluid displacement $\boldsymbol\xi$. Frozen-in [flux](../../../physics.md#flux) gives $\mathbf b=i\omega_A\boldsymbol\xi$, while the Eulerian perturbation velocity is $u_x=\dot\xi_x$, $u_y=\dot\xi_y+2A\xi_x$, because the displacement samples the gradient of the basic flow. The equations become the [spring model of magnetorotational instability](../../../astrophysics.md#spring-model-of-magnetorotational-instability):

$$
\ddot\xi_x-2\Omega\dot\xi_y-4\Omega A\xi_x=-\omega_A^2\xi_x,\qquad \ddot\xi_y+2\Omega\dot\xi_x=-\omega_A^2\xi_y.
$$

For the stated time dependence, their [determinant](../../../linear-algebra.md#determinant) is

$$
\det\begin{pmatrix}\omega_A^2-\omega^2-4\Omega A&2i\Omega\omega\\-2i\Omega\omega&\omega_A^2-\omega^2\end{pmatrix}=0.
$$

Thus the [ideal magnetorotational dispersion relation](../../../astrophysics.md#ideal-magnetorotational-dispersion-relation) is

$$
\boxed{(\omega^2-\omega_A^2)^2-4\Omega(\Omega-A)\omega^2-4\Omega A\omega_A^2=0.}
$$

It follows without dividing by $\omega$, so the neutral stability boundary is included.

To analyze it, put $a=\omega_A^2$ and $Y=\omega^2$. Then

$$
Y^2-(\kappa_r^2+2a)Y+a(a-4\Omega A)=0,\qquad Y_\pm=a+\frac{\kappa_r^2}{2}\pm\frac12\sqrt{\kappa_r^4+16\Omega^2a}.
$$

For a hydrodynamically stable rotation law, $\kappa_r^2>0$, the sum of the two roots is positive. Their product is negative precisely when $0<a<4\Omega A$. One squared frequency is then negative, giving an exponentially growing mode $\omega=i\gamma$ and its decaying partner. Therefore the [magnetorotational instability](../../../astrophysics.md#magnetorotational-instability), or [MRI](../../../astrophysics.md#magnetorotational-instability), has criterion

$$
\boxed{\frac{d\Omega^2}{d\ln r}=-4\Omega A<0,\qquad 0<\omega_A^2<4\Omega A.}
$$

Angular velocity must decrease outwards, although [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) may increase outwards and satisfy [Rayleigh's circulation criterion](../../../hydrodynamic-stability.md#rayleigh-s-circulation-criterion). This is why a Keplerian disc can be stable to the axisymmetric hydrodynamic disturbances of Question 2 yet unstable once magnetic coupling is introduced. At zero magnetic frequency the unstable root becomes neutral, while sufficiently large magnetic frequency restores stability. For increasing angular velocity, $A<0$ with $\Omega>0$, this ideal vertical-field instability is absent.

The [growth rate](../../../wave-equation.md#growth-rate) is

$$
\gamma^2=\frac12\left[\sqrt{\kappa_r^4+16\Omega^2a}-\kappa_r^2-2a\right].
$$

For $0<A<\Omega$, differentiation with respect to $a$ sets $\sqrt{\kappa_r^4+16\Omega^2a}=4\Omega^2$, yielding the [maximum growth rate of ideal magnetorotational instability](../../../astrophysics.md#maximum-growth-rate-of-ideal-magnetorotational-instability):

$$
\boxed{\omega_{A,\max}^2=A(2\Omega-A),\qquad \gamma_{\max}=A.}
$$

For [Keplerian rotation](../../../astrophysics.md#keplerian-disk), $A=3\Omega/4$, so

$$
\boxed{0<\omega_A^2<3\Omega^2,\qquad \omega_{A,\max}^2=\frac{15}{16}\Omega^2,\qquad \gamma_{\max}=\frac34\Omega.}
$$

Thus the fastest growth is on an orbital timescale. The field strength selects its wavelength, $k_{\max}\propto1/v_A$, rather than the maximum ideal [growth rate](../../../wave-equation.md#growth-rate). At fixed $k$, growth does approach zero as $B_0\to0$; retaining the finite maximum in that limit requires shorter wavelengths, which [magnetic diffusion](../../../astrophysical-fluid-dynamics.md#magnetic-diffusion) can eventually exclude. Unstable wavelengths satisfy $\lambda>2\pi v_A/\sqrt{4\Omega A}$ in this local model. A finite disc must accommodate such a wavelength, so a sufficiently strong field can suppress the available vertical modes through excessive tension.

Physically, a bent field line acts like a spring joining neighboring fluid elements. The inner element rotates faster and pulls the outer element forward, transferring [angular momentum](../../../classical-mechanics.md#angular-momentum) outward. The inner element loses [angular momentum](../../../classical-mechanics.md#angular-momentum) and moves inward; the outer element gains it and moves outward. In a rotation law with outward-decreasing angular velocity, these motions increase their angular-velocity difference and the magnetic coupling produces further separation. A weak restoring spring therefore creates a feedback instability by enabling angular-momentum exchange. Without that exchange, each displaced element keeps its [angular momentum](../../../classical-mechanics.md#angular-momentum) and a positive epicyclic frequency restores its orbit. Strong [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension) instead prevents the separation. The free [energy](../../../classical-mechanics.md#energy) is the [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation), not the initial magnetic [energy](../../../classical-mechanics.md#energy).

The instability provides an important route to turbulence and [angular momentum transport](../../../classical-mechanics.md#angular-momentum-transport) in sufficiently conducting [accretion discs](../../../astrophysics.md#accretion-disk). The radial [flux](../../../physics.md#flux) of azimuthal momentum includes the stress

$$
T_{xy}=\rho\langle u_xu_y\rangle-\frac{\langle\delta B_x\delta B_y\rangle}{\mu_0}.
$$

The first term is a [Reynolds stress](../../../turbulence.md#reynolds-stress) and the second is the magnetic contribution from the [Maxwell stress tensor](../../../electromagnetism.md#maxwell-stress-tensor), with the sign appropriate to momentum [flux](../../../physics.md#flux). For the growing branch, take $u_x$ real and positive. The linear equations give $u_y/u_x=(\gamma^2+a)/(2\Omega\gamma)>0$ and $b_y/b_x=(\gamma^2+a-4\Omega A)/(2\Omega\gamma)<0$. The last sign follows from $(\gamma^2+a)(\gamma^2+a-4\Omega A)+4\Omega^2\gamma^2=0$. Thus both the velocity and magnetic contributions carry [angular momentum](../../../classical-mechanics.md#angular-momentum) outward. The associated [energy](../../../classical-mechanics.md#energy) extraction is $-T_{xy}\,r\,d\Omega/dr=2AT_{xy}>0$. Inward accretion can then accompany outward angular-momentum transport, and dissipation of the resulting fluctuations heats the disc. This gives a physical mechanism behind an effective turbulent-viscosity description such as an [alpha disk](../../../astrophysics.md#alpha-disk), whereas microscopic [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) alone is generally too weak for rapid accretion.

<a id="3/image-finite-hydrodynamic-swing-amplification-compared-with-the-growing-mri-branch-in-a-keplerian-disc"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-73-shear-instabilities.png)

**[Figure 1](#3/image-finite-hydrodynamic-swing-amplification-compared-with-the-growing-mri-branch-in-a-keplerian-disc). Finite hydrodynamic swing amplification compared with the growing MRI branch in a Keplerian disc**.

**[MRI](../../../astrophysics.md#magnetorotational-instability) is an exponentially growing magnetic instability of outward-decreasing angular velocity; hydrodynamic shearing-wave amplification is transient and does not by itself establish sustained turbulence.** Nonlinear saturation, field regeneration and transport efficiency depend on field geometry, boundaries and thermodynamics. Poor conductivity or important nonideal magnetic effects can suppress or modify the ideal instability, so the local dispersion relation is a mechanism and growth criterion rather than a universal prescription for the saturated stress.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
