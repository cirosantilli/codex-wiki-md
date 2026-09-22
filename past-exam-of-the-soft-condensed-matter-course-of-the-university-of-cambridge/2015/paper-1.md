# Paper 1

↑ **Parent:** [2015](../2015.md)

Original solutions to the nonbiology portions of the released paper. [Original public PDF, physical pages 364–367; dated 30 May 2015](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=364)

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

At fixed [temperature](../../temperature.md) and [solvent](../../mixture.md#solvent) [permittivity](../../permittivity.md), the [Debye–Hückel screening length](../../mathematical-biology.md#debye-huckel-screening-length) satisfies $\lambda_D^{-2}\propto\sum_i c_i z_i^2=2I$, where $I=\tfrac12\sum_i c_i z_i^2$ is [ionic strength](../../mixture.md#ionic-strength). Fully dissociated [sodium chloride](../../chemical-substance.md#sodium-chloride) has two monovalent [ion](../../chemistry.md#ion) species, giving $I_1=0.01$ M. Fully dissociated [magnesium sulfate](../../chemistry.md#magnesium-sulfate) has two divalent species, giving

$$
I_2=\tfrac12[0.1(2)^2+0.1(-2)^2]=0.40\,\mathrm M.
$$

The [multivalent-electrolyte screening-length ratio](../../mathematical-biology.md#multivalent-electrolyte-screening-length-ratio) is therefore

$$
\boxed{\lambda_{D,2}=3\,\mathrm{nm}\sqrt{\frac{0.01}{0.40}}=0.474\,\mathrm{nm}\simeq0.47\,\mathrm{nm}.}
$$

The squared valences are essential: counting only the total [ion](../../chemistry.md#ion) [concentration](../../mathematical-physics.md#concentration) misses a factor of four in the screening strength per formula unit. This is the comparable linear-screening estimate, assuming unchanged dielectric response and full dissociation. [ion pairs](../../ionic-bonding.md#ion-pair) and concentrated-electrolyte nonideality can make a real divalent-salt solution depart from it; no such correction is specified.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a long [ideal chain](../../mathematical-biology.md#ideal-chain) of $N$ statistical segments of [length](../../physics.md#length) $b$, $R_G^2=Nb^2/6$. At fixed repeat chemistry and statistical segment [length](../../physics.md#length), [molar mass](../../chemistry.md#molar-mass) is proportional to $N$. The [molecular-weight scaling of an ideal-chain gyration radius](../../polymer.md#molecular-weight-scaling-of-an-ideal-chain-gyration-radius) thus gives

$$
\boxed{R_G(10^6)=120\,\mathrm{nm}\sqrt{\frac{10^6}{10^5}}=379.5\,\mathrm{nm}\simeq3.8\times10^2\,\mathrm{nm}.}
$$

The supplied size and ideal statistics are used as stipulated; an independently tabulated coil size would not replace the given baseline.

[solvent quality](../../mixture.md#solvent-quality) changes the balance of segment–segment and segment–[solvent](../../mixture.md#solvent) contacts. In a [good solvent](../../mixture.md#good-solvent), excluded-volume repulsion swells a sufficiently long isolated chain, with $R_G\propto N^\nu$, $\nu\simeq0.588$ in three dimensions; the [Flory approximation](../../polymer.md#flory-approximation) gives $\nu=3/5$. At theta conditions the effective two-segment [excluded volume](../../statistical-physics.md#excluded-volume) vanishes and the ideal exponent $1/2$ is recovered for long chains. A [poor solvent](../../mixture.md#poor-solvent) favors a compact [polymer globule](../../mixture.md#polymer-globule), whose large-chain size scales approximately as $N^{1/3}$ at fixed internal [density](../../fluid-mechanics.md#density). [solvent](../../mixture.md#solvent) and [temperature](../../temperature.md) can also change local [persistence length](../../mathematical-biology.md#persistence-length) and hence the prefactor. These different conformations need not have the same radius at the same [molar mass](../../chemistry.md#molar-mass).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**TODO: user-deferred biology. The bacterium-specific numerical estimate and assumptions are deferred.**

The independent fluid-mechanical relation is

$$
\boxed{\mathrm{Re}=\frac{\rho UL}{\eta}=\frac{UL}{\nu},}
$$

where $\rho$ is [fluid](../../fluid-mechanics.md#fluid) [mass density](../../fluid-mechanics.md#density), $\eta$ [dynamic viscosity](../../dynamic-viscosity.md) and $\nu$ [kinematic viscosity](../../dynamic-viscosity.md#kinematic-viscosity). For a generic rigid [sphere](../../euclidean-geometry.md#sphere), the convention must specify whether $L$ is its diameter or radius; their [Reynolds numbers](../../dynamic-viscosity.md#reynolds-number) differ by a factor of two. The ratio compares advective [inertia](../../classical-mechanics.md#inertia) $\rho U^2/L$ with viscous [stress](../../continuum-mechanics.md#stress) gradients $\eta U/L^2$. Small [Reynolds number](../../dynamic-viscosity.md#reynolds-number) supports a creeping-flow approximation when unsteady [fluid](../../fluid-mechanics.md#fluid) [inertia](../../classical-mechanics.md#inertia) is also negligible. No organism-specific size, speed or propulsion calculation is made here.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Stokes–Einstein relation](../../stokes-flow.md#stokes-einstein-relation) connects thermal [diffusion](../../thermodynamics.md#diffusion) with dissipative [mobility](../../critical-phenomenon.md#order-parameter-mobility). For a dilute suspension of isolated rigid [spheres](../../euclidean-geometry.md#sphere) of [hydrodynamic radius](../../mixture.md#hydrodynamic-radius) $a$ in an unbounded [Newtonian fluid](../../viscous-fluid-flow.md#newtonian-fluid) of [viscosity](../../dynamic-viscosity.md) $\eta$,

$$
\boxed{D=\frac{k_BT}{\zeta}=\frac{k_BT}{6\pi\eta a},}
$$

where $\zeta$ is translational [drag coefficient](../../fluid-mechanics.md#drag-coefficient), $D$ [diffusion coefficient](../../brownian-motion.md#diffusion-coefficient) and $T$ absolute [temperature](../../temperature.md). [Stokes drag](../../stokes-flow.md#stokes-s-law) supplies $\zeta=6\pi\eta a$ under no-slip, continuum, low-Reynolds-number conditions. The [Einstein diffusion relation](../../thermodynamics.md#einstein-diffusion-relation) $D=k_BT/\zeta$ is more general than that particular spherical [drag](../../fluid-mechanics.md#drag-physics) law.

A short [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) argument explains the connection. Let a weak external potential $U$ exert [force](../../force.md) $\mathbf F=-\nabla U$, so drift [velocity](../../classical-mechanics.md#velocity) is $\mathbf F/\zeta$. The number [flux](../../mathematical-physics.md#flux) is $\mathbf j=n\mathbf F/\zeta-D\nabla n$. A [Boltzmann distribution](../../thermodynamics.md#boltzmann-distribution) $n\propto e^{-U/(k_BT)}$ has $\nabla n=n\mathbf F/(k_BT)$; requiring zero [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) [flux](../../mathematical-physics.md#flux) fixes $D=k_BT/\zeta$. [thermal fluctuations](../../statistical-physics.md#thermal-fluctuation) and viscous [dissipation](../../thermodynamics.md#dissipation) are therefore linked, rather than independent adjustable effects. The original theory also relates [diffusion](../../thermodynamics.md#diffusion) to measured random displacements.[Sections 3–5, printed pages 9–18 in the linked translation: equilibrium flux balance, spherical drag and displacement variance](../../physics-bibliography.md#on-the-movement-of-small-particles-suspended-in-a-stationary-liquid-demanded-by-the-molecular-kinetic-theory-of-heat-by-albert-einstein)

On times long compared with momentum relaxation, an isotropic diffusing [sphere](../../euclidean-geometry.md#sphere) has

$$
\langle[\Delta x(t)]^2\rangle=2Dt,\qquad
\langle|\Delta\mathbf r(t)|^2\rangle=6Dt.
$$

[single-particle tracking](../../biology.md#single-particle-tracking) can measure the slope. Alternatively, dilute single-scattering [dynamic light scattering](../../biology.md#dynamic-light-scattering) measures a field correlation $g_1(q,t)=e^{-Dq^2t}$; the corresponding intensity-correlation excess is proportional to $e^{-2Dq^2t}$. The scattering [wavenumber](../../wave-equation.md#wavenumber) and the distinction between field and intensity decay must be retained.

A [Stokes-Einstein experimental consistency test](../../stokes-flow.md#stokes-einstein-experimental-consistency-test) independently measures [temperature](../../temperature.md) and [solvent](../../mixture.md#solvent) [viscosity](../../dynamic-viscosity.md), uses a narrow distribution of inert [spheres](../../euclidean-geometry.md#sphere), checks decay rate proportional to $q^2$ or displacement variance proportional to time, and extrapolates toward infinite dilution. Subtract drift, account for wall-enhanced [drag](../../fluid-mechanics.md#drag-physics), and verify that aggregation is absent. Tracking additionally needs spatial calibration and correction for finite exposure and [localization precision](../../fluorescence.md#localization-precision). At finite [concentration](../../mathematical-physics.md#concentration), collective [diffusion](../../thermodynamics.md#diffusion) is not automatically the single-particle [self-diffusion](../../thermodynamics.md#self-diffusion) in the equation. A [hydrodynamic radius](../../mixture.md#hydrodynamic-radius) is not generally identical to a [polymer](../../polymer.md) [radius of gyration](../../polymer.md#radius-of-gyration); nonspherical particles, slip or viscoelastic [solvents](../../mixture.md#solvent) require a different [mobility](../../critical-phenomenon.md#order-parameter-mobility) model.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[polymers at interfaces](../../polymer.md#polymers-at-interfaces) balance favorable surface contacts against lost [conformational entropy](../../protein.md#conformational-entropy) and interactions among neighboring chains. At an attractive solid–liquid interface, an [adsorbed polymer train](../../polymer.md#adsorbed-polymer-train) consists of consecutive bound segments. An [adsorbed polymer loop](../../polymer.md#adsorbed-polymer-loop) leaves the surface and returns to it, while an [adsorbed polymer tail](../../polymer.md#adsorbed-polymer-tail) extends to a free chain end. A chain can contain all three, so [adsorption](../../physical-chemistry.md#adsorption) does not imply a completely flattened molecule. Surface affinity, [solvent quality](../../mixture.md#solvent-quality), [persistence length](../../mathematical-biology.md#persistence-length), chain [length](../../physics.md#length) and [concentration](../../mathematical-physics.md#concentration) control the balance and the resulting segment-density profile.

<a id="2/b/image-original-schematic-of-adsorbed-trains-loops-and-tails-and-the-crossover-from-isolated-grafted-mushrooms-to-an-overlapping-polymer-brush"></a>
![](../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1-polymer-interfaces.png)

**[Figure 1](#2/b/image-original-schematic-of-adsorbed-trains-loops-and-tails-and-the-crossover-from-isolated-grafted-mushrooms-to-an-overlapping-polymer-brush). Original schematic of adsorbed trains, loops and tails, and the crossover from isolated grafted mushrooms to an overlapping polymer brush**.

[adsorption](../../physical-chemistry.md#adsorption) gains [energy](../../energy.md) of order $\epsilon k_BT$ per bound segment but reduces the number of accessible chain configurations. Weak [adsorption](../../physical-chemistry.md#adsorption) can be described through [adsorption blobs](../../polymer.md#adsorption-blob) whose thickness exceeds the statistical segment [length](../../physics.md#length); each blob loses an [energy](../../energy.md) of order $k_BT$ through [confinement](../../standard-model.md#confinement). Stronger attraction generally creates more contacts and a more compact layer, while loops and tails can still dominate its outer extent. A measurement of adsorbed mass alone therefore does not determine layer thickness or conformation.

End-grafted chains are different: their attachment is fixed at one end. At [grafting density](../../polymer.md#grafting-density) $\sigma_g$, the mean lateral spacing is $D\sim\sigma_g^{-1/2}$. At low coverage the chains behave as isolated [polymer mushrooms](../../polymer.md#polymer-mushroom). The [polymer mushroom-to-brush crossover](../../polymer.md#polymer-mushroom-to-brush-crossover) occurs when $\sigma_gR_G^2\sim1$. At higher coverage in a [good solvent](../../mixture.md#good-solvent), crowding makes chains extend away from the surface. A free-energy balance per chain,

$$
\frac{F}{k_BT}\sim\frac{H^2}{Nb^2}+\frac{vN^2\sigma_g}{H},
$$

combines stretching [entropy](../../entropy.md) with repulsive [excluded volume](../../statistical-physics.md#excluded-volume) $v>0$. Minimization gives $H^3\sim vN^3b^2\sigma_g$, or

$$
\boxed{H\sim Nb(\sigma_gb^2)^{1/3}\quad\text{when }v\sim b^3.}
$$

This is a scaling result with an undetermined order-one coefficient, valid for overlapping chains stretched below their contour [length](../../physics.md#length). In a compact poor-solvent layer, a roughly fixed internal [polymer](../../polymer.md) [volume fraction](../../continuum-mechanics.md#volume-fraction) instead gives $H\propto N\sigma_g$.

Small-angle neutron scattering on end-grafted polydimethylsiloxane layers on porous silica has distinguished the good- and poor-solvent [density](../../fluid-mechanics.md#density) exponents. The chemical system and scattering contrast matter: changing [solvent quality](../../mixture.md#solvent-quality) should be separated from changing graft coverage, chain [molar mass](../../chemistry.md#molar-mass) or [adsorption](../../physical-chemistry.md#adsorption) strength.[Physical Review Letters 66, 719–722 (1991), abstract: actual polymer/substrate system, neutron-scattering method and the two thickness scalings](../../physics-bibliography.md#characterization-of-the-brush-regime-for-grafted-polymer-layers-at-the-solid-liquid-interface-by-p-auroy-and-others)

An interface can also localize chains of a [block copolymer](../../polymer.md#block-copolymer) when its blocks prefer different media. Such layers change [interfacial tension](../../critical-phenomenon.md#interfacial-tension) and can stabilize dispersed droplets or particles through [steric repulsion](../../mixture.md#steric-repulsion). Overlapping layers in a [good solvent](../../mixture.md#good-solvent) cost osmotic and conformational [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy); incomplete [adsorption](../../physical-chemistry.md#adsorption) can instead produce [polymer bridging](../../mixture.md#polymer-bridging) between particles. Nonadsorbing chains can cause depletion attraction. Thus the presence of a [polymer](../../polymer.md) does not by itself guarantee stabilization.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A viscoelastic material stores part of the [work](../../energy.md#work) of deformation and dissipates part. In the linear regime its [stress](../../continuum-mechanics.md#stress) depends on the [strain](../../continuum-mechanics.md#strain) history, not just the instantaneous [strain](../../continuum-mechanics.md#strain) or [shear strain rate](../../continuum-mechanics.md#shear-strain-rate). For simple shear, a causal [relaxation modulus](../../rheology.md#relaxation-modulus) $G(t)$ gives $\sigma(t)=\int_{-\infty}^tG(t-t')\dot\gamma(t')dt'$. A sudden [strain](../../continuum-mechanics.md#strain) then probes [stress relaxation](../../rheology.md#stress-relaxation), while a constant imposed [stress](../../continuum-mechanics.md#stress) probes [material creep](../../engineering.md#creep-deformation); these are different experiments.

For steady sinusoidal [strain](../../continuum-mechanics.md#strain) use the convention $\gamma(t)=\gamma_0\cos\omega t$ and $e^{i\omega t}$ complex amplitudes. The [complex viscoelastic modulus](../../rheology.md#dynamic-modulus) is

$$
\boxed{G^*(\omega)=\frac{\widetilde\sigma}{\widetilde\gamma}
=G'(\omega)+iG''(\omega),}
$$

so $\sigma(t)=\gamma_0[G'\cos\omega t-G''\sin\omega t]$. The [storage modulus](../../rheology.md#storage-modulus) $G'$ is the in-phase elastic component. The [loss modulus](../../rheology.md#loss-modulus) $G''$ multiplies the component in phase with [shear strain rate](../../continuum-mechanics.md#shear-strain-rate); [stress](../../continuum-mechanics.md#stress) leads [strain](../../continuum-mechanics.md#strain) by $\delta=\operatorname{atan2}(G'',G')$. The [loss tangent](../../rheology.md#loss-tangent) is $\tan\delta=G''/G'$ when $G'>0$.

Multiplying [stress](../../continuum-mechanics.md#stress) by [shear strain rate](../../continuum-mechanics.md#shear-strain-rate) and averaging gives $\langle P\rangle/V=\tfrac12\omega G''\gamma_0^2$. Hence the [dissipated energy per oscillatory shear cycle](../../rheology.md#dissipated-energy-per-oscillatory-shear-cycle) is

$$
\boxed{\frac{W_{\rm cycle}}{V}=\pi G''\gamma_0^2.}
$$

The elastic contribution returns its [work](../../energy.md#work) over the cycle. A passive material has nonnegative [dissipation](../../thermodynamics.md#dissipation), which fixes the sign of the loss term in the chosen Fourier convention. This [complex viscoelastic modulus](../../rheology.md#dynamic-modulus) is a response function, not the mathematical absolute value of a complex number.

A [Maxwell model](../../rheology.md#linear-maxwell-fluid) places a [spring](../../elasticity-physics.md#spring) of [shear modulus](../../elasticity-physics.md#shear-modulus) $G$ in series with a [dashpot](../../rheology.md#dashpot) of [viscosity](../../dynamic-viscosity.md) $\eta$, so the [strains](../../continuum-mechanics.md#strain) add at common [stress](../../continuum-mechanics.md#stress):

$$
\dot\gamma=\frac{\dot\sigma}{G}+\frac{\sigma}{\eta},
\qquad\tau=\frac{\eta}{G}.
$$

The [Maxwell fluid dynamic modulus](../../rheology.md#maxwell-fluid-dynamic-modulus) is

$$
G^*=\frac{G\,i\omega\tau}{1+i\omega\tau},\qquad
\boxed{G'=\frac{G(\omega\tau)^2}{1+(\omega\tau)^2},\quad
G''=\frac{G\omega\tau}{1+(\omega\tau)^2}.}
$$

At $\omega\tau\ll1$ the response is predominantly viscous, $G''\simeq\eta\omega$ and $G'\simeq G(\omega\tau)^2$. At $\omega\tau\gg1$ it approaches the elastic plateau $G'=G$. The two moduli cross, and $G''$ reaches its maximum, at $\omega\tau=1$. A [Kelvin-Voigt model](../../rheology.md#kelvin-voigt-model) instead has the [spring](../../elasticity-physics.md#spring) and [dashpot](../../rheology.md#dashpot) in parallel, giving $G^*=G+i\eta\omega$ and no fluid-like zero-frequency terminal flow. Real materials often need a spectrum of [relaxation times](../../markov-chain.md#relaxation-time) rather than one Maxwell time.

<a id="2/c/image-original-maxwell-storage-and-loss-moduli-with-a-stress-strain-cycle-whose-enclosed-area-measures-dissipated-work"></a>
![](../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1-viscoelasticity.png)

**[Figure 2](#2/c/image-original-maxwell-storage-and-loss-moduli-with-a-stress-strain-cycle-whose-enclosed-area-measures-dissipated-work). Original Maxwell storage and loss moduli, with a stress–strain cycle whose enclosed area measures dissipated work**.

Oscillatory [rheometry](../../rheology.md#rheometry) measures [stress](../../continuum-mechanics.md#stress) amplitude and phase while imposing a small [strain](../../continuum-mechanics.md#strain). An [oscillatory-shear amplitude sweep](../../rheology.md#oscillatory-shear-amplitude-sweep) first identifies a linear regime; an [oscillatory-shear frequency sweep](../../rheology.md#oscillatory-shear-frequency-sweep) then measures $G'$ and $G''$. Repeat at controlled [temperature](../../temperature.md), suppress evaporation, check [wall slip](../../fluid-mechanics.md#wall-slip) and sample aging, and correct instrument [inertia](../../classical-mechanics.md#inertia) at high [frequency](../../wave.md#frequency). Frequency-dependent structure and a nonlinear response cannot be inferred reliably by fitting one [spring](../../elasticity-physics.md#spring) and [dashpot](../../rheology.md#dashpot) to one point.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [amphiphile](../../physical-chemistry.md#amphiphile) has a solvent-affine part and a solvent-averse part within one molecule. In water these are commonly called [hydrophilic](../../physical-chemistry.md#hydrophilicity) head and [hydrophobic](../../physical-chemistry.md#hydrophobicity) tail. Two nonbiological examples are [sodium dodecyl sulfate](../../surface-tension.md#sodium-dodecyl-sulfate), with a twelve-carbon tail and an anionic sulfate head, and [cetyltrimethylammonium bromide](../../surface-tension.md#cetrimonium-bromide), with a sixteen-carbon tail and a cationic quaternary-ammonium head. Their [counterions](../../chemistry.md#counterion) balance the ionic head-group charge; the head and tail do not have interchangeable interactions with water.

Aggregation reduces unfavorable exposure of [hydrocarbon](../../chemical-substance.md#hydrocarbon) tails to water but loses molecular translational [entropy](../../entropy.md). Interfacial [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy), head-group [solvation](../../ionic-bonding.md#solvation) and electrostatic repulsion, chain packing and [conformational entropy](../../protein.md#conformational-entropy) determine the preferred aggregate. The [hydrophobic effect](../../physical-chemistry.md#hydrophobic-effect) is a solvent-mediated free-energy balance, rather than a literal attractive bond between tails.

The [amphiphile packing parameter](../../physical-chemistry.md#amphiphile-packing-parameter)

$$
P=\frac{v}{a_0\ell_c}
$$

compares tail [volume](../../geometry-and-topology.md#volume) $v$, effective head-group [area](../../differential-geometry.md#surface-area) $a_0$ and maximum tail [length](../../physics.md#length) $\ell_c$. A spherical core of radius $R$ obeys $v/a_0=R/3$, and a long cylindrical core obeys $v/a_0=R/2$. The condition $R\leq\ell_c$ gives the conventional spherical window $P\lesssim1/3$ and cylindrical window $1/3\lesssim P\lesssim1/2$. Less strongly curved bilayers become compatible for $1/2\lesssim P\lesssim1$, with planar packing near one; values above one can favor inverse [curvature](../../differential-geometry.md#curvature) in an appropriate nonpolar surrounding medium. These windows are geometric guides rather than exact phase boundaries.

A larger hydrated or electrostatically repelling head increases $a_0$ and favors positive [curvature](../../differential-geometry.md#curvature). Screening of charged heads or a smaller head can lower $a_0$ and favor rods or sheets. Multiple tails increase the tail [volume](../../geometry-and-topology.md#volume) relative to head [area](../../differential-geometry.md#surface-area) and can favor bilayers. Tail [length](../../physics.md#length), branching, [temperature](../../temperature.md) and [solvent](../../mixture.md#solvent) selectivity alter both geometry and interaction [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy), so one cannot predict a unique aggregate from hydrophobicity alone.[1976, pp. 1525–1568: coupled thermodynamics, molecular packing constraints and globular, cylindrical and bilayer aggregates](../../chemistry-bibliography.md#theory-of-self-assembly-of-hydrocarbon-amphiphiles-by-jacob-n-israelachvili-and-others)

In the supplied chemical-potential expression, $\mu$ is the [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) [chemical potential](../../chemical-potential.md) per [amphiphile](../../physical-chemistry.md#amphiphile), $\mu_\alpha^0$ the standard [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy) per [amphiphile](../../physical-chemistry.md#amphiphile) within an aggregate of size $\alpha$, and $x_\alpha$ the dimensionless molecular fraction belonging to that size class. The [aggregate molecular fraction versus aggregate number fraction](../../physical-chemistry.md#aggregate-molecular-fraction-versus-aggregate-number-fraction) distinction explains the logarithm: the aggregate count fraction is $x_\alpha/\alpha$, and dividing its translational [chemical potential](../../chemical-potential.md) by $\alpha$ gives a per-molecule value. Thus

$$
\alpha\frac{\mu-\mu_\alpha^0}{k_BT}=\ln(x_\alpha/\alpha),
\qquad
\boxed{x_\alpha=\alpha\exp\!\left[\frac{\alpha(\mu-\mu_\alpha^0)}{k_BT}\right].}
$$

Here $k_B$ is the [Boltzmann constant](../../thermodynamics.md#boltzmann-constant), $T$ absolute [temperature](../../temperature.md), and $\alpha$ a positive integer. The logarithm acts on a dimensionless ideal activity; a concentrated nonideal solution would require [activity coefficients](../../chemical-potential.md#activity-coefficient).

[equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) exchange of [amphiphiles](../../physical-chemistry.md#amphiphile) gives the same per-molecule $\mu$ for every size. For monomers, $\mu=\mu_1^0+k_BT\ln x_1$. Substitution yields the [finite-micelle aggregation-number distribution](../../physical-chemistry.md#finite-micelle-aggregation-number-distribution)

$$
\boxed{x_\alpha=\alpha x_1^\alpha
\exp\!\left[\frac{\alpha(\mu_1^0-\mu_\alpha^0)}{k_BT}\right],\qquad
x_{\rm tot}=\sum_{\alpha\ge1}x_\alpha.}
$$

This formula by itself does not prescribe a preferred [micelle](../../physical-chemistry.md#micelle) size: the size dependence of $\mu_\alpha^0$ must include the competing packing and interaction terms. If their balance favors a finite size $\alpha_*$, a monomer population and a peak around that size can coexist. Dividing by $\alpha$ would instead plot the distribution of aggregate counts.

At very low $x_{\rm tot}$, the factors $x_1^\alpha$ suppress large aggregates and most molecules remain monomers. As $x_1$ rises, a favorable aggregate class grows extremely rapidly because of this high [power](../../energy.md#power). The [critical micelle concentration from standard chemical potentials](../../physical-chemistry.md#critical-micelle-concentration-from-standard-chemical-potentials) has the large-size estimate

$$
x_{1,*}\simeq\exp\!\left[\frac{\mu_{\alpha_*}^0-\mu_1^0}{k_BT}\right].
$$

More precisely, the illustrative crossover condition $x_{\alpha_*}=x_1$ gives

$$
\ln x_{1,*}=
\frac{\alpha_*(\mu_{\alpha_*}^0-\mu_1^0)/(k_BT)-\ln\alpha_*}{\alpha_*-1}.
$$

Added material above the crossover enters aggregates predominantly. Monomer [concentration](../../mathematical-physics.md#concentration) then increases slowly rather than being exactly pinned: its logarithm enters $\mu$, while aggregate populations respond with a large factor $\alpha_*$. For finite [micelles](../../physical-chemistry.md#micelle) this is a sharp association crossover, not an absolute prohibition on aggregates below one exact [concentration](../../mathematical-physics.md#concentration).

<a id="3/image-original-illustrative-molecular-fraction-distributions-over-aggregation-number-below-and-above-a-micellization-crossover"></a>
![](../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1-aggregate-distribution.png)

**[Figure 3](#3/image-original-illustrative-molecular-fraction-distributions-over-aggregation-number-below-and-above-a-micellization-crossover). Original illustrative molecular-fraction distributions over aggregation number below and above a micellization crossover**.

The drawing uses a declared illustrative standard-free-energy model favoring aggregates near $\alpha=40$. It is not an inferred distribution or critical [concentration](../../mathematical-physics.md#concentration) for either named [surfactant](../../surface-tension.md#surfactant). The separate monomer peak is at $\alpha=1$; a distribution of molecular fractions weights each aggregate by its number of molecules.

For the general physics of a nearly planar [fluid](../../fluid-mechanics.md#fluid) sheet, let $h(x,y)$ be a small-slope displacement, $\kappa$ [membrane bending rigidity](../../mathematical-biology.md#membrane-bending-rigidity) and $\sigma$ mechanical tension. At fixed topology and symmetric reference [curvature](../../differential-geometry.md#curvature), the quadratic [Helfrich energy](../../mathematical-biology.md#helfrich-energy) is

$$
F[h]=\frac12\int d^2x\,[\kappa(\nabla^2h)^2+\sigma|\nabla h|^2].
$$

The bending term is the small-slope curvature-elastic [energy](../../energy.md); additional spontaneous-curvature or boundary terms require extra information.[Section II.C, p. 695, equation (12): curvature-elastic energy and coefficients with units of energy](../../physics-bibliography.md#elastic-properties-of-lipid-bilayers-theory-and-possible-experiments-by-wolfgang-helfrich)

For Fourier amplitudes $h_{\mathbf q}=A^{-1}\int_Ah(\mathbf x)e^{-i\mathbf q\cdot\mathbf x}d^2x$, equipartition gives the [membrane fluctuation spectrum under tension](../../mathematical-biology.md#membrane-fluctuation-spectrum-under-tension),

$$
\boxed{\langle|h_{\mathbf q}|^2\rangle=
\frac{k_BT}{A(\kappa q^4+\sigma q^2)}.}
$$

Higher [temperature](../../temperature.md) increases fluctuations, while greater [membrane bending rigidity](../../mathematical-biology.md#membrane-bending-rigidity) or tension suppresses them. Short-wavelength modes are predominantly bending-controlled; longer wavelengths can be tension-controlled. Finite sheet size, supports, [confinement](../../standard-model.md#confinement) and imposed [area](../../differential-geometry.md#surface-area) set [boundary conditions](../../differential-equation.md#boundary-condition) and [infrared cutoffs](../../fourier-analysis.md#infrared-cutoff); continuum elasticity also needs a short-distance cutoff. [solvent](../../mixture.md#solvent) [viscosity](../../dynamic-viscosity.md) affects relaxation rates, although it does not enter this [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) amplitude at fixed elastic parameters.

**TODO: user-deferred biology. The requested importance of these fluctuations for bodily function is deferred.** The preceding result covers only the independent continuum and thermal physics.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In a [regular solution](../../mixture.md#regular-solution), ideal combinatorial [entropy](../../entropy.md) competes with a nonzero unlike-contact [energy](../../energy.md). For equal molecular [volumes](../../geometry-and-topology.md#volume) and [mole fraction](../../mathematical-biology.md#mole-fraction) $\phi$ of species A, write mixing [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy) per site as

$$
\frac{f(\phi)}{k_BT}
=\phi\ln\phi+(1-\phi)\ln(1-\phi)+\chi\phi(1-\phi),
$$

where

$$
\chi=\frac{z}{k_BT}\left[\epsilon_{AB}-\frac{\epsilon_{AA}+\epsilon_{BB}}2\right].
$$

Here $z$ is the [coordination number](../../ionic-bonding.md#coordination-number) and $\epsilon_{ij}$ a pair-contact [energy](../../energy.md) counted consistently in the lattice model. A positive $\chi$ penalizes unlike contacts; a negative value favors them. The logarithmic terms lower [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy) on mixing. The sign of the [enthalpy of mixing](../../enthalpy.md#enthalpy-of-mixing) alone therefore does not determine miscibility.

At fixed [temperature](../../temperature.md) and composition, a homogeneous phase is globally stable only if no division into two compositions lowers its [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy). The [common-tangent construction](../../critical-phenomenon.md#common-tangent-construction) selects coexisting compositions $\phi_a,\phi_b$, equivalent to equality of both species' [chemical potentials](../../chemical-potential.md). Local stability to infinitesimal fluctuations instead requires

$$
\frac{f''}{k_BT}=\frac1\phi+\frac1{1-\phi}-2\chi>0.
$$

Zero [curvature](../../differential-geometry.md#curvature) gives the [spinodal](../../critical-phenomenon.md#spinodal), while the coexistence boundary is the [binodal](../../critical-phenomenon.md#binodal). Between them a homogeneous state can be metastable and require [nucleation](../../critical-phenomenon.md#nucleation); inside the [spinodal](../../critical-phenomenon.md#spinodal) its small composition fluctuations grow. The symmetric [regular solution](../../mixture.md#regular-solution) has

$$
\boxed{\phi_c=\tfrac12,\qquad\chi_c=2.}
$$

Below this contact penalty, the [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy) is convex at every composition. Above it a miscibility gap is possible around the central composition. If $\chi=A/T$ with $A>0$, heating promotes mixing, but specific interactions or temperature-dependent noncombinatorial terms can produce other trends.

For two [polymers](../../polymer.md), let $N_A,N_B$ count equal-volume segments per chain, and now let $\phi$ be the segment [volume fraction](../../continuum-mechanics.md#volume-fraction) of A. Connecting segments into chains reduces their independent translational [entropy](../../entropy.md). The [binary Flory-Huggins polymer blend](../../mixture.md#binary-flory-huggins-polymer-blend) has

$$
\frac{f}{k_BT}=\frac{\phi}{N_A}\ln\phi
+\frac{1-\phi}{N_B}\ln(1-\phi)+\chi\phi(1-\phi).
$$

The energetic contact term remains extensive in the number of segments, while the favorable [entropy](../../entropy.md) per segment is reduced by $1/N_A$ and $1/N_B$. This is the key [long-chain limit of polymer-blend miscibility](../../mixture.md#long-chain-limit-of-polymer-blend-miscibility): a small positive incompatibility can overcome the mixing [entropy](../../entropy.md). The lattice treatment is a controlled model for this argument, rather than a claim that every real blend has composition-independent $\chi$.[1942, pp. 51–55: chain-connected lattice configurations and combinatorial mixing entropy; later sections add the energetic contribution](../../chemistry-bibliography.md#thermodynamics-of-high-polymer-solutions-by-paul-j-flory)

The local stability condition and critical interaction parameter become

$$
\frac1{N_A\phi}+\frac1{N_B(1-\phi)}-2\chi>0,\qquad
\boxed{\chi_c=\frac12\left(N_A^{-1/2}+N_B^{-1/2}\right)^2.}
$$

For equal chain [lengths](../../physics.md#length), $\chi_c=2/N$. Similar segment chemistry and matched cohesive interactions can reduce the unlike-contact penalty; favorable specific interactions, such as complementary [hydrogen bonding](../../chemical-bond.md#hydrogen-bonding), can make mixing favorable even for long chains. Lower [molar mass](../../chemistry.md#molar-mass) increases mixing [entropy](../../entropy.md). [temperature](../../temperature.md) can help when it lowers the effective $\chi$, but heating is not universally sufficient. A suitable common [solvent](../../mixture.md#solvent) can facilitate processing or ternary mixing, and a block-copolymer compatibilizer can stabilize fine domains; neither guarantees that the final solvent-free binary material is one [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) molecular phase.

An oil–water [emulsion](../../mixture.md#emulsion) illustrates [emulsion stability versus molecular miscibility](../../mixture.md#emulsion-stability-versus-molecular-miscibility). A [surfactant](../../surface-tension.md#surfactant) adsorbs with its water-affine head toward water and its oil-affine tail toward oil, lowering [interfacial tension](../../critical-phenomenon.md#interfacial-tension) and the [work](../../energy.md#work) $\gamma\,dA$ needed to make additional interface. Breaking a fixed oil [volume](../../geometry-and-topology.md#volume) $V_o$ into spherical droplets of radius $R$ gives total [area](../../differential-geometry.md#surface-area) $3V_o/R$, so creating small droplets still requires substantial [area](../../differential-geometry.md#surface-area) and usually mechanical [work](../../energy.md#work).

Adsorbed [surfactants](../../surface-tension.md#surfactant) can oppose [droplet coalescence](../../mixture.md#droplet-coalescence) through charged double-layer repulsion, hydrated-head interactions or [steric repulsion](../../mixture.md#steric-repulsion) from sufficiently extended groups. Adequate coverage, [adsorption](../../physical-chemistry.md#adsorption) time, ionic conditions and [film drainage](../../engineering.md#film-drainage) affect the lifetime. A lower [interfacial tension](../../critical-phenomenon.md#interfacial-tension) does not itself remove the bulk miscibility gap, and a protected [emulsion](../../mixture.md#emulsion) is commonly kinetically stabilized. A thermodynamically stable [microemulsion](../../critical-phenomenon.md#microemulsion) is a distinct situation requiring an appropriate composition and free-energy balance. The two liquids must not be called molecularly miscible simply because droplets disperse visibly.

For the capillary, balance upward contact-line [force](../../force.md) against hydrostatic column weight, neglecting meniscus [volume](../../geometry-and-topology.md#volume) and gas [density](../../fluid-mechanics.md#density). For inner radius $r$,

$$
2\pi r\gamma\cos\theta=\rho g\pi r^2h,
\qquad h=\frac{2\gamma\cos\theta}{\rho gr}.
$$

The [contact angle](../../surface-tension.md#contact-angle) is measured through the liquid. [complete wetting](../../surface-tension.md#complete-wetting) means $\theta_2=0$, so the [contact-angle change of capillary rise](../../surface-tension.md#contact-angle-change-of-capillary-rise) gives

$$
\boxed{h_2=\frac{0.050}{\cos35^\circ}=0.06104\,\mathrm m\simeq6.10\,\mathrm{cm}.}
$$

This follows from the stipulated [wetting](../../surface-tension.md#wetting) change, holding radius, bulk liquid [surface tension](../../surface-tension.md) and [density](../../fluid-mechanics.md#density) fixed. One should not replace that premise with a general claim that grease always improves glass [wetting](../../surface-tension.md#wetting); if contamination also changes the liquid [surface tension](../../surface-tension.md), the original height and new angle alone would not determine the new height.

For two wide vertical plates separated by gap $d$, use unit width. There are two upward contact-line contributions and liquid cross-sectional [area](../../differential-geometry.md#surface-area) $d$, giving the [capillary rise between parallel plates](../../surface-tension.md#capillary-rise-between-parallel-plates):

$$
2\gamma\cos\theta=\rho gdh_{\rm plates},
\qquad\boxed{h_{\rm plates}=\frac{2\gamma\cos\theta}{\rho gd}.}
$$

Only one principal meniscus [curvature](../../differential-geometry.md#curvature) contributes between wide plates, whereas a circular tube has two. For the same [fluid](../../fluid-mechanics.md#fluid) and angle,

$$
\boxed{\frac{h_{\rm plates}}{h_{\rm tube}}=\frac rd.}
$$

If the plate gap equals the tube diameter, $d=2r$, the rise is half as large: the initial and completely [wetting](../../surface-tension.md#wetting) heights would be $2.50$ cm and $3.05$ cm. If instead $d=r$, the heights are equal. In either geometry, changing only the angle from $35^\circ$ to zero multiplies the height by $1/\cos35^\circ$. Since the question specifies no plate spacing, the general gap-dependent relation is the unambiguous result; the half-height answer requires the equal-gap-to-diameter convention.

## ↑ Ancestors (11)

1. [2015](../2015.md)
2. [Past exam of the soft condensed matter course of the University of Cambridge](../../past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge.md)
3. [Soft Condensed Matter course of the University of Cambridge](../../university-of-cambridge.md#soft-condensed-matter-course-of-the-university-of-cambridge)
4. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
