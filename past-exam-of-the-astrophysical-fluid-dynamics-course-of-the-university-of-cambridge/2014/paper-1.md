# Paper 1

↑ **Parent:** [2014](../2014.md)

Original public paper: [Physical PDF pages 303–306](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=303). All optional notes and both long questions are covered. The cloud-mass conventions, magnetic-collapse assumptions and [entropy](../../entropy.md) normalization are distinguished explicitly.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For an [ideal gas](../../ideal-gas.md) of fixed composition, the central [temperature](../../temperature.md) satisfies $T_c\propto p_c/\rho_c=K\rho_c^{1/n}$. Keeping $T_c$ fixed therefore requires $K\propto\rho_c^{-1/n}$, rather than keeping the [polytropic constant](../../astrophysical-fluid-dynamics.md#polytropic-constant) fixed. Substitution in the [Lane-Emden equation](../../nonlinear-analysis.md#lane-emden-equation) scalings gives

$$
M\propto\rho_c^{(3/n-1)/2}\rho_c^{-3/(2n)}=\rho_c^{-1/2},\qquad
R\propto\rho_c^{(1/n-1)/2}\rho_c^{-1/(2n)}=\rho_c^{-1/2}.
$$

Consequently the [homologous polytropes at fixed central temperature](../../stellar-structure.md#homologous-polytropes-at-fixed-central-temperature) obey

$$
\boxed{M\propto R.}
$$

The [polytropic index](../../stellar-structure.md#polytropic-index) and mean particle [mass](../../classical-mechanics.md#mass) must be common to this homologous sequence: varying either changes the dimensionless structural coefficient. The fixed-central-temperature assumption is the idealization being used here, rather than a universal property of real [stars](../../stellar-astrophysics.md#star).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In an adiabatic outflow without additional heating, the reservoir's [specific enthalpy](../../enthalpy.md#specific-enthalpy) supplies both escaping [kinetic energy](../../energy.md#kinetic-energy) and the work against [gravity](../../physics.md#gravity). For a monatomic [ideal gas](../../ideal-gas.md), $\gamma=5/3$ and $h=c_s^2/(\gamma-1)=3c_s^2/2$, where $c_s$ is the reservoir's [adiabatic sound speed](../../compressible-flow.md#adiabatic-sound-speed). The [Bernoulli equation](../../euler-equations-for-an-inviscid-fluid.md#bernoulli-equation), measured from a reservoir initially at rest at radius $r$, gives

$$
\frac{v_\infty^2}{2}+h_\infty
=\frac{c_s^2}{\gamma-1}-\frac{GM}{r}.
$$

The maximum terminal speed uses all available [specific enthalpy](../../enthalpy.md#specific-enthalpy), so $h_\infty\to0$ and

$$
\boxed{v_{\infty,\max}=\sqrt{3c_s^2-\frac{2GM}{r}}.}
$$

A freely escaping adiabatic flow needs a nonnegative radicand; equality is marginal escape. If the radicand is negative, this reservoir cannot supply an unheated escaping outflow. The initial rest condition is a stagnation-reservoir approximation: an exactly stationary finite-density surface cannot simultaneously carry a nonzero steady [mass flow rate](../../fluid-mechanics.md#mass-flow-rate). Further heating, radiation [forces](../../force.md) or an imposed confining [pressure](../../pressure.md) would change the terminal-energy budget.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Once swept-up matter dominates the ejecta and [radiative cooling](../../heat.md#radiative-cooling) is negligible, the [Sedov-Taylor blast wave](../../galaxy.md#sedov-taylor-blast-wave) has its [shock](../../transport-equation.md#shock-wave) radius fixed by [dimensional analysis](../../mathematical-physics.md#dimensional-analysis):

$$
R_s=\xi\left(\frac{Et^2}{\rho_0}\right)^{1/5}.
$$

Here $\xi$ is a dimensionless constant of order unity fixed by the [adiabatic index](../../ideal-gas.md#heat-capacity-ratio). Treating the ambient matter as [hydrogen](../../chemical-substance.md#hydrogen) gives $\rho_0\simeq10^6m_H\simeq1.67\times10^{-21}\,\mathrm{kg\,m^{-3}}$, while $t\simeq3.16\times10^{10}\,\mathrm s$. Thus

$$
\boxed{R_s\simeq1.43\times10^{17}\,\mathrm m\simeq4.6\,\mathrm{pc}\quad(\xi\simeq1).}
$$

For a monatomic gas, the usual similarity normalization $\xi\simeq1.15$ instead gives about $5.3\,\mathrm{pc}$. An estimate of a few [parsecs](../../astrophysics.md#parsec) is therefore appropriate. Negligible ejecta [mass](../../classical-mechanics.md#mass) does not by itself guarantee this energy-conserving stage: substantial radiation losses or a strongly nonuniform ambient [mass density](../../fluid-mechanics.md#density) would invalidate the assumed similarity law.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [stellar wind](../../stellar-astrophysics.md#stellar-wind) carries matter away from a [star](../../stellar-astrophysics.md#star), altering its [mass](../../classical-mechanics.md#mass), [angular momentum](../../momentum.md#angular-momentum) and surroundings. Hot coronal gas can escape through pressure-driven expansion; radiation transfers [momentum](../../momentum.md) to gas through continuum or [spectral line](../../stellar-astrophysics.md#spectral-line) absorption, or to dust that then drags gas. A [magnetic field](../../magnetic-field.md) can transfer rotational [energy](../../energy.md) and [angular momentum](../../momentum.md#angular-momentum) to an outflow. These mechanisms need not give the same terminal speed or [mass loss rate](../../mathematical-physics.md#mass-loss-rate).

For a steady spherical pressure-driven model, [conservation of mass](../../continuum-mechanics.md#mass-conservation) gives $\dot M=4\pi r^2\rho u$. Combining the radial [Euler equation](../../euler-equations-for-an-inviscid-fluid.md) with an [isothermal equation of state](../../compressible-flow.md#globally-isothermal-equation-of-state) $p=\rho a^2$ gives the [Parker wind equation](../../astrophysical-fluid-dynamics.md#parker-wind-equation)

$$
\left(u-\frac{a^2}{u}\right)\frac{du}{dr}
=\frac{2a^2}{r}-\frac{GM}{r^2}.
$$

A smooth [transonic branch](../../compressible-flow.md#transonic-branch) passes through $u=a$ at $r_s=GM/(2a^2)$, connecting a subsonic inner atmosphere to an escaping supersonic wind. The [isothermal Parker wind](../../astrophysical-fluid-dynamics.md#isothermal-parker-wind) requires continuing heat input as the gas expands; a [polytropic stellar wind](../../stellar-astrophysics.md#polytropic-stellar-wind) instead tracks a changing [temperature](../../temperature.md) and must satisfy its own terminal-energy condition. A [subsonic isothermal breeze](../../astrophysical-fluid-dynamics.md#subsonic-isothermal-breeze) generally tends to a nonzero external [pressure](../../pressure.md), so outward velocity alone does not select the escaping solution.

<a id="2/a/image-transonic-isothermal-parker-wind-and-a-pressure-confined-breeze"></a>
![](../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1-parker-wind.png)

**[Figure 1](#2/a/image-transonic-isothermal-parker-wind-and-a-pressure-confined-breeze). Transonic isothermal Parker wind and a pressure-confined breeze**.

The [solar wind](../../astrophysics.md#solar-wind) supplies a nearby example of an outward [plasma](../../physics.md#plasma-physics) flow carrying a [magnetic field](../../magnetic-field.md). Profiles of [spectral lines](../../stellar-astrophysics.md#spectral-line), especially absorption shifted by the [Doppler effect](../../wave.md#doppler-effect) together with emission, diagnose more distant [stellar winds](../../stellar-astrophysics.md#stellar-wind). The critical-point condition and boundary heating constrain $\dot M$; it is not determined by an escape-speed estimate alone.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

An [accretion disk](../../astrophysical-disk.md#accretion-disk) forms when inward-moving gas retains enough [angular momentum](../../momentum.md#angular-momentum) to orbit a compact object. In a geometrically thin [Keplerian disk](../../astrophysical-disk.md#keplerian-disk), radial [force](../../force.md) balance gives $\Omega\simeq\sqrt{GM/r^3}$ and vertical [hydrostatic equilibrium](../../statistical-physics.md#hydrostatic-equilibrium) gives a thickness $H\sim c_s/\Omega\ll r$. Matter cannot fall far inward while keeping its original [specific angular momentum](../../celestial-mechanics.md#specific-angular-momentum) $r^2\Omega\propto r^{1/2}$: stresses must transport [angular momentum](../../momentum.md#angular-momentum) outward.

The [viscous torque in an accretion disk](../../astrophysical-disk.md#viscous-torque-in-an-accretion-disk) has outward magnitude

$$
\mathcal G=-2\pi r^3\nu\Sigma\frac{d\Omega}{dr}
=3\pi\nu\Sigma\sqrt{GMr},
$$

where $\nu$ is the effective [kinematic viscosity](../../dynamic-viscosity.md#kinematic-viscosity) and $\Sigma$ the [surface density](../../astrophysical-disk.md#surface-density-of-a-disk). With constant inward [accretion rate](../../astrophysical-disk.md#accretion-rate) $\dot M>0$ and zero inner torque at $r_{\rm in}$, [conservation of angular momentum](../../momentum.md#conservation-of-angular-momentum) gives

$$
\nu\Sigma=\frac{\dot M}{3\pi}\left(1-\sqrt{\frac{r_{\rm in}}r}\right).
$$

The associated [standard thin-disk dissipation flux](../../astrophysical-disk.md#standard-thin-disk-dissipation-flux) from each face is

$$
F(r)=\frac{3GM\dot M}{8\pi r^3}\left(1-\sqrt{\frac{r_{\rm in}}r}\right).
$$

Orbital [gravitational potential energy](../../energy.md#gravitational-energy) becomes [heat](../../heat.md) and, in a radiatively efficient disk, escaping radiation. Integrating both faces gives the [standard thin-disk luminosity](../../astrophysical-disk.md#standard-thin-disk-luminosity) $L=GM\dot M/(2r_{\rm in})$ under this boundary condition. A central stellar surface or an inner torque can release or redistribute additional [energy](../../energy.md).

The [alpha disk](../../astrophysical-disk.md#alpha-disk) prescription $\nu\sim\alpha c_sH$ summarizes an effective stress rather than a claim that molecular [viscosity](../../dynamic-viscosity.md) alone explains observed rates. In an ionized disk, [magnetorotational instability](../../astrophysical-disk.md#magnetorotational-instability) can produce magnetic and fluid stresses. The inward evolution occurs on the [viscous timescale](../../astrophysical-disk.md#viscous-timescale) $t_\nu\sim r^2/\nu$, much longer than an orbit for a thin disk with $\alpha\lesssim1$. Hot inner annuli and cooler outer annuli naturally give a range of emitted [temperatures](../../temperature.md); the [blackbody](../../astrophysics.md#blackbody) approximation additionally requires sufficient [optical depth](../../astrophysics.md#optical-depth).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A local thermal imbalance can amplify a gas perturbation even without an initial displacement of an interface. Let $\mathcal L(\rho,T)$ denote net cooling per unit [mass](../../classical-mechanics.md#mass), including heating with a negative sign, and suppose $\mathcal L(\rho_0,T_0)=0$. When the [sound-crossing time](../../compressible-flow.md#sound-crossing-time) is short compared with the thermal evolution time, [pressure](../../pressure.md) equilibrates and an [ideal gas](../../ideal-gas.md) perturbation is approximately isobaric. The linearized thermal equation is

$$
c_p\frac{d\delta T}{dt}
=-\left(\frac{\partial\mathcal L}{\partial T}\right)_p\delta T.
$$

Thus a negative constant-pressure derivative produces [isobaric thermal instability](../../astrophysical-fluid-dynamics.md#isobaric-thermal-instability): a cooler parcel experiences a net loss that cools it further, while a warmer parcel heats further. For example, [isobaric thermal stability of a heated ideal gas](../../astrophysical-fluid-dynamics.md#isobaric-thermal-stability-of-a-heated-ideal-gas) with $\mathcal L=A\rho T^\alpha-H$ gives $\sigma=(1-\alpha)H/(c_pT_0)$ and instability for $\alpha<1$. Different heating laws and fixed-density perturbations give different criteria; [thermal conduction](../../heat.md#thermal-conduction) damps sufficiently short-scale [temperature](../../temperature.md) contrasts. Such feedback helps a gas separate into denser cool and rarer warm regions when stable thermal branches exist.

The [Rayleigh-Taylor instability](../../continuum-mechanics.md#rayleigh-taylor-instability) instead releases [gravitational potential energy](../../energy.md#gravitational-energy) when a heavier fluid lies above a lighter fluid in a downward gravitational field. For two inviscid incompressible half-spaces with no [surface tension](../../surface-tension.md) or [magnetic field](../../magnetic-field.md), a horizontal perturbation of [wavenumber](../../wave-equation.md#wavenumber) $k$ has

$$
\sigma^2=\mathcal A gk,\qquad
\mathcal A=\frac{\rho_h-\rho_l}{\rho_h+\rho_l}>0.
$$

The [Atwood number](../../continuum-mechanics.md#atwood-number) measures the density contrast. A descending heavy-fluid finger and an ascending light-fluid bubble both lower the total [gravitational potential energy](../../energy.md#gravitational-energy), increasing the original displacement. Interchanging the layers gives an oscillatory stable interface. An accelerating or decelerating astrophysical shell has an analogous effective acceleration, allowing mixing at suitable ejecta interfaces in a [supernova remnant](../../galaxy.md#supernova-remnant). Finite interface width, [viscosity](../../dynamic-viscosity.md), [surface tension](../../surface-tension.md) and [magnetic tension](../../magnetohydrodynamics.md#magnetic-tension) modify the short-wavelength behavior; the ideal sharp-interface formula does not select a finite fastest-growing wavelength.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For small isentropic perturbations of a fixed-composition [gas](../../thermodynamics.md#gas), linearizing its [equation of state](../../pressure.md#equation-of-state) gives $p_1=(\partial p/\partial\rho)_s\rho_1=c_s^2\rho_1$. The [adiabatic sound speed](../../compressible-flow.md#adiabatic-sound-speed) is evaluated at the uniform background, so it is spatially constant at this order. If fast heat exchange instead enforces constant [temperature](../../temperature.md), use the [isothermal sound speed](../../compressible-flow.md#isothermal-sound-speed) consistently. A completely arbitrary [entropy](../../entropy.md) perturbation would require an additional thermodynamic variable.

The uniform static infinite medium requires the [Jeans swindle](../../linear-cosmological-density-perturbation.md#jeans-swindle): its background gravitational field is subtracted or externally balanced, and only the perturbation sources the [Poisson equation for Newtonian gravity](../../newton-s-law-of-universal-gravitation.md#poisson-equation-for-newtonian-gravity). Linearizing the [continuity equation](../../mathematical-physics.md#continuity-equation), [Euler equation](../../euler-equations-for-an-inviscid-fluid.md) and gravitational equation then gives

$$
\partial_t\rho_1+\rho_0\nabla\cdot\mathbf u_1=0,\qquad
\partial_t\mathbf u_1=-\frac{c_s^2}{\rho_0}\nabla\rho_1-\nabla\Psi_1,\qquad
\nabla^2\Psi_1=4\pi G\rho_1.
$$

Taking one more time derivative of the first equation and substituting the other two yields

$$
\partial_t^2\rho_1=c_s^2\nabla^2\rho_1+4\pi G\rho_0\rho_1.
$$

A [Fourier mode](../../fourier-analysis.md#fourier-mode) proportional to $e^{i(\mathbf k\cdot\mathbf x-\omega t)}$ therefore obeys the [Jeans instability](../../linear-cosmological-density-perturbation.md#jeans-instability) relation

$$
\boxed{\omega^2=c_s^2k^2-4\pi G\rho_0
=c_s^2(k^2-k_J^2),\qquad k_J=\frac{\sqrt{4\pi G\rho_0}}{c_s}.}
$$

For $k>k_J$, the mode oscillates as a [sound wave](../../fluid-mechanics.md#acoustic-wave). For $0<k<k_J$, $\omega=\pm i\sqrt{4\pi G\rho_0-c_s^2k^2}$ gives a growing and a decaying mode; the [static Jeans growth-rate spectrum](../../linear-cosmological-density-perturbation.md#static-jeans-growth-rate-spectrum) has no preferred finite fastest-growing wavelength in the infinite-medium approximation. The threshold $k=k_J$ is marginal at linear order. The [Jeans length](../../linear-cosmological-density-perturbation.md#jeans-length) is $\lambda_J=2\pi/k_J=c_s\sqrt{\pi/(G\rho_0)}$. Defining the [Jeans mass](../../stellar-astrophysics.md#jeans-mass) as a sphere whose diameter is this wavelength gives

$$
\boxed{M_J=\frac{4\pi}{3}\rho_0\left(\frac{\lambda_J}{2}\right)^3
=\frac{\pi^{5/2}}6\frac{c_s^3}{G^{3/2}\rho_0^{1/2}}.}
$$

Other radius conventions alter its numerical coefficient; the [mass](../../classical-mechanics.md#mass) scale compares [self-gravity](../../newton-s-law-of-universal-gravitation.md#self-gravity) with [pressure](../../pressure.md) communication.

For the pressureless finite cloud, the [shell theorem](../../mathematical-physics.md#spherical-shell-theorem) gives an edge acceleration $\ddot r=-GM/r^2$, with fixed enclosed $M=4\pi r_0^3\rho_0/3$. Multiplication by $\dot r$ and integration from rest gives

$$
\frac{\dot r^2}{2}=GM\left(\frac1r-\frac1{r_0}\right),\qquad
\dot r=-\sqrt{2GM}\left(\frac1r-\frac1{r_0}\right)^{1/2}.
$$

The negative root describes collapse. Substituting $r=r_0\sin^2\theta$ gives the [free-fall time of a uniform sphere](../../astrophysics.md#free-fall-time-of-a-uniform-sphere)

$$
t_{\rm ff}=\frac{2r_0^{3/2}}{\sqrt{2GM}}\int_0^{\pi/2}\sin^2\theta\,d\theta
=\frac{\pi r_0^{3/2}}{2\sqrt{2GM}}
=\boxed{\sqrt{\frac{3\pi}{32G\rho_0}}}.
$$

The surface and inner shells reach the origin together in [pressureless homologous spherical collapse](../../astrophysics.md#pressureless-homologous-spherical-collapse); [pressure](../../pressure.md), rotation or shell crossing would change this ideal solution.

Equating this time to the specified radius-based [sound-crossing time](../../compressible-flow.md#sound-crossing-time) $r_0/c_s$ gives $r_0=c_s\sqrt{3\pi/(32G\rho_0)}$. The resulting [crossing-time cloud support mass](../../stellar-astrophysics.md#crossing-time-cloud-support-mass) is

$$
\boxed{M_{\rm cross}=C_{\rm cross}\frac{c_s^3}{G^{3/2}\rho_0^{1/2}},\qquad
C_{\rm cross}=\frac{4\pi}{3}\left(\frac{3\pi}{32}\right)^{3/2}.}
$$

This is the same dimensional [mass](../../classical-mechanics.md#mass) scale as $M_J$, with a different coefficient because the adopted length and time criteria differ. In particular, $t_{\rm ff}=r_0/c_s$ is not the exact marginal dispersion-relation condition.

With the requested isotropic support approximation, replace $c_s$ by the [Alfvén speed](../../ideal-magnetohydrodynamics.md#alfven-speed) $v_A=B/\sqrt{\mu_0\rho_0}$. In the crossing-time convention the [Magnetic Jeans mass](../../stellar-astrophysics.md#magnetic-jeans-mass) is

$$
\boxed{M_{B,{\rm cross}}=C_{\rm cross}\frac{v_A^3}{G^{3/2}\rho_0^{1/2}}
=C_{\rm cross}\frac{B^3}{(\mu_0G)^{3/2}\rho_0^2}.}
$$

Using the wavelength-based [Jeans mass](../../stellar-astrophysics.md#jeans-mass) convention instead replaces $C_{\rm cross}$ by $\pi^{5/2}/6$. The scaling, rather than a convention-independent coefficient, is the shared prediction.

For a fixed cloud [mass](../../classical-mechanics.md#mass) undergoing isothermal homologous contraction, $\rho/\rho_0=(r_0/r)^3$ and $c_s$ is constant. Its number of thermal [Jeans masses](../../stellar-astrophysics.md#jeans-mass) therefore grows as

$$
\boxed{N_J(\rho)=N_{J,0}\left(\frac{\rho}{\rho_0}\right)^{1/2}
=N_{J,0}\left(\frac{r_0}{r}\right)^{3/2}.}
$$

A cloud initially close to the support threshold has $N_{J,0}$ of order one, so smaller pieces can subsequently become independently unstable: this is [isothermal fragmentation](../../stellar-astrophysics.md#isothermal-fragmentation).

For approximately isotropic contraction with [magnetic flux freezing](../../ideal-magnetohydrodynamics.md#magnetic-flux-freezing), $Br^2$ stays constant, so $B\propto\rho^{2/3}$. Hence $M_B\propto B^3/\rho^2$ stays constant and

$$
\boxed{N_B(\rho)=N_{B,0}.}
$$

This ideal magnetic support therefore does not create progressively more unstable masses in the way thermal isothermal support does. The same conclusion follows from the conserved [mass-to-flux ratio](../../ideal-magnetohydrodynamics.md#mass-to-flux-ratio). A magnetically subcritical cloud cannot initiate unrestricted cross-field collapse under ideal flux freezing alone; flux loss or initially supercritical conditions are needed. A real [magnetic field](../../magnetic-field.md) also gives anisotropic support: motion and fragmentation along its field lines are not excluded by this scalar-speed estimate.

<a id="3/image-jeans-dispersion-relation-and-the-changing-number-of-support-masses-during-idealized-collapse"></a>
![](../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1-jeans-instability.png)

**[Figure 2](#3/image-jeans-dispersion-relation-and-the-changing-number-of-support-masses-during-idealized-collapse). Jeans dispersion relation and the changing number of support masses during idealized collapse**.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Mach number](../../compressible-flow.md#mach-number) is $\mathcal M=u/c_s$, comparing the flow speed relative to a disturbance with the local [sound speed](../../compressible-flow.md#speed-of-sound). For a body moving supersonically, spherical acoustic disturbances emitted earlier have a tangent envelope with [Mach cone](../../compressible-flow.md#mach-cone) half-angle $\sin\theta=1/\mathcal M$. Signals cannot propagate arbitrarily far upstream. Compressive characteristics can converge and steepen into a [shock wave](../../transport-equation.md#shock-wave), within which microscopic dissipation prevents a multivalued fluid state; supersonic motion alone does not require every flow to contain a shock.

Work in the [shock frame](../../compressible-flow.md#shock-frame) with steady normal velocities $u_1,u_2>0$. Integrating [conservation of mass](../../continuum-mechanics.md#mass-conservation), normal [momentum](../../momentum.md) and total [energy](../../energy.md) over a thin pillbox, neglecting gravity across the thin layer, gives the [Rankine-Hugoniot conditions for a perfect gas](../../compressible-flow.md#rankine-hugoniot-conditions-for-a-perfect-gas):

$$
j=\rho_1u_1=\rho_2u_2,\qquad
p_1+\rho_1u_1^2=p_2+\rho_2u_2^2,
$$



$$
j\left(h_1+\frac{u_1^2}{2}\right)
=j\left(h_2+\frac{u_2^2}{2}\right),\qquad
h=\frac{\gamma p}{(\gamma-1)\rho}.
$$

The [energy](../../energy.md) equation includes [pressure](../../pressure.md) work through [specific enthalpy](../../enthalpy.md#specific-enthalpy). The shock is adiabatic if negligible [heat](../../heat.md) escapes the layer, but its irreversible dissipation means it is not isentropic.

Put $\chi=\rho_2/\rho_1=u_1/u_2$ and $\mathcal M_1=u_1/\sqrt{\gamma p_1/\rho_1}$. [Momentum](../../momentum.md) conservation gives $p_2=p_1+\rho_1u_1^2(1-1/\chi)$. Substitution in the [energy](../../energy.md) equation produces the unshocked root $\chi=1$ and the compressive root

$$
\chi=\frac{(\gamma+1)\mathcal M_1^2}{(\gamma-1)\mathcal M_1^2+2},\qquad
\frac{p_2}{p_1}=\frac{2\gamma\mathcal M_1^2-(\gamma-1)}{\gamma+1}.
$$

Since $\rho_1u_1^2/p_1=\gamma\mathcal M_1^2$, the strong-shock limit has negligible upstream thermal [pressure](../../pressure.md) compared with ram [pressure](../../pressure.md). The [Strong-shock Rankine-Hugoniot conditions](../../compressible-flow.md#strong-shock-rankine-hugoniot-conditions) give

$$
\boxed{\frac{\rho_2}{\rho_1}=\frac{u_1}{u_2}\longrightarrow\frac{\gamma+1}{\gamma-1},\qquad
\frac{p_2}{p_1}\simeq\frac{2\gamma}{\gamma+1}\mathcal M_1^2.}
$$

For unchanged composition, the [ideal gas law](../../ideal-gas.md#ideal-gas-law) implies $T_2/T_1=(p_2/p_1)/\chi$, so

$$
\boxed{\frac{T_2}{T_1}\simeq\frac{2\gamma(\gamma-1)}{(\gamma+1)^2}\mathcal M_1^2.}
$$

For $\gamma=5/3$, the compression tends to four and $T_2\simeq3\bar m u_1^2/(16k_B)$, where $\bar m$ is mean particle [mass](../../classical-mechanics.md#mass).

With constant specific heat $c_v$, [entropy production in a perfect-gas shock](../../compressible-flow.md#entropy-production-in-a-perfect-gas-shock) is measured by the change in [specific entropy](../../entropy.md#specific-entropy)

$$
\Delta s=c_v\ln\left[\frac{p_2}{p_1}\left(\frac{\rho_1}{\rho_2}\right)^\gamma\right].
$$

The strong-shock expression is therefore

$$
\boxed{\Delta s\simeq c_v\ln\left[\frac{2\gamma\mathcal M_1^2}{\gamma+1}
\left(\frac{\gamma-1}{\gamma+1}\right)^\gamma\right].}
$$

The exact jump is positive for every compressive shock with $\mathcal M_1>1$, in accordance with the [Second law of thermodynamics](../../second-law-of-thermodynamics.md); the asymptotic expression is only for $\mathcal M_1\gg1$. There is a normalization issue in the printed description: this logarithmic formula with constant $c_v$ describes [entropy](../../entropy.md) per unit [mass](../../classical-mechanics.md#mass). The true [entropy density](../../entropy.md#entropy-density) is $\rho s$, so its difference is $\rho_2s_2-\rho_1s_1$, rather than the same logarithmic jump with a constant [heat capacity](../../heat.md#heat-capacity) per unit [volume](../../geometry-and-topology.md#volume). A material parcel's irreversible [entropy](../../entropy.md) increase should be assessed using $\Delta s$.

Downstream gas is denser and hotter. For optically thin collisional emission the loss per unit [volume](../../geometry-and-topology.md#volume) is typically $n_en_i\Lambda(T)$, whereas stored thermal [energy](../../energy.md) scales approximately as $nT$. Compression can therefore reduce the [radiative gas cooling time](../../heat.md#optically-thin-gas-cooling-time); excitation and ionization at the higher [temperature](../../temperature.md) can open additional cooling channels. The actual efficiency still depends on the [astrophysical cooling function](../../heat.md#astrophysical-cooling-function), composition and [optical depth](../../astrophysics.md#optical-depth). In a radiative shock with separated scales, the [temperature](../../temperature.md) first rises across a narrow dissipative layer, then decreases through a much broader cooling region of characteristic length $\ell_{\rm cool}\sim u_2t_{\rm cool}$. Subsonic cooling usually brings further compression with approximately constant [pressure](../../pressure.md). The immediate microscopic shock thickness and the macroscopic cooling length are distinct.

Let state $f$ be the fully cooled gas, with $T_f=T_1$ and the same composition. Set $a^2=p_1/\rho_1$, the [isothermal sound speed](../../compressible-flow.md#isothermal-sound-speed) squared. Across the entire shock plus cooling layer, [mass](../../classical-mechanics.md#mass) and [momentum](../../momentum.md) are still conserved, but gas [energy](../../energy.md) alone is not. With $\chi_f=\rho_f/\rho_1$,

$$
a^2+u_1^2=a^2\chi_f+\frac{u_1^2}{\chi_f},\qquad
(\chi_f-1)(a^2\chi_f-u_1^2)=0.
$$

The nontrivial [isothermal shock](../../compressible-flow.md#isothermal-shock) therefore has

$$
\boxed{\rho_f=\rho_1\frac{u_1^2}{a^2}
=\gamma\mathcal M_1^2\rho_1.}
$$

If the upstream Mach number were defined with $a$ instead, this would be $\rho_f/\rho_1=\mathcal M_{\rm iso}^2$. Retaining the distinction avoids losing the factor $\gamma$.

The gas's [specific entropy](../../entropy.md#specific-entropy) rises irreversibly at the hot shock and then decreases as escaping radiation removes heat. Since the final [temperature](../../temperature.md) equals the initial [temperature](../../temperature.md),

$$
\boxed{s_f-s_1=-(\gamma-1)c_v\ln\chi_f<0.}
$$

This decrease for the gas is consistent with the [Second law of thermodynamics](../../second-law-of-thermodynamics.md): the emitted radiation and its eventual surroundings carry [entropy](../../entropy.md) away. It does not make the microscopic compressive shock reversible. The figure illustrates both the hot [entropy](../../entropy.md) jump and the subsequent cooling; its spatial cooling profile is schematic because no cooling law has been specified.

<a id="4/image-temperature-and-specific-entropy-across-an-adiabatic-shock-followed-by-radiative-cooling"></a>
![](../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1-radiative-shock.png)

**[Figure 3](#4/image-temperature-and-specific-entropy-across-an-adiabatic-shock-followed-by-radiative-cooling). Temperature and specific entropy across an adiabatic shock followed by radiative cooling**.

## ↑ Ancestors (11)

1. [2014](../2014.md)
2. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
3. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../university-of-cambridge.md#astrophysical-fluid-dynamics-course-of-the-university-of-cambridge)
4. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
