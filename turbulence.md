# Turbulence

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turbulence)

Turbulence is irregular fluid motion with interacting velocity fluctuations over a range of scales. It can mix a [particle suspension](fluid-mechanics.md#suspension-chemistry) and promote [fluid entrainment](fluid-mechanics.md#fluid-entrainment) into a [turbulent plume](turbulent-plume.md).

**Table of contents**

- [Reynolds averaging](#reynolds-averaging)
- [External intermittency](#external-intermittency)
- [Wave turbulence](#wave-turbulence)
  - [Weak wave cascade](#weak-wave-cascade)
- [Magnetohydrodynamic turbulence](#magnetohydrodynamic-turbulence)
  - [Dimensional freedom of an MHD spectrum](#dimensional-freedom-of-an-mhd-spectrum)
  - [Electron-magnetohydrodynamic cascade](#electron-magnetohydrodynamic-cascade)
    - [Critically balanced electron-magnetohydrodynamic cascade](#critically-balanced-electron-magnetohydrodynamic-cascade)
    - [Weak electron-magnetohydrodynamic cascade](#weak-electron-magnetohydrodynamic-cascade)
  - [Critical balance](#critical-balance)
  - [Alfvénic turbulence](#alfvenic-turbulence)
    - [Weak Alfvénic cascade](#weak-alfvenic-cascade)
      - [Weak-to-strong transition of an Alfvénic cascade](#weak-to-strong-transition-of-an-alfvenic-cascade)
    - [Iroshnikov-Kraichnan spectrum](#iroshnikov-kraichnan-spectrum)
    - [Goldreich–Sridhar turbulence](#goldreich-sridhar-turbulence)
- [Turbulence closure](#turbulence-closure)
  - [Constant-skewness turbulence closure](#constant-skewness-turbulence-closure)
    - [Normalized constant-skewness structure-function equation](#normalized-constant-skewness-structure-function-equation)
  - [Eddy-damped quasi-normal Markovian closure](#eddy-damped-quasi-normal-markovian-closure)
- [K-epsilon turbulence model](#k-epsilon-turbulence-model)
  - [K-epsilon turbulence front](#k-epsilon-turbulence-front)
  - [Log-layer solution of the k-epsilon model](#log-layer-solution-of-the-k-epsilon-model)
- [Turbulent mixing](#turbulent-mixing)
  - [Richardson pair dispersion](#richardson-pair-dispersion)
    - [Three-regime turbulent pair-separation model](#three-regime-turbulent-pair-separation-model)
    - [Diffusive large-scale pair dispersion](#diffusive-large-scale-pair-dispersion)
    - [Richardson constant](#richardson-constant)
  - [Taylor turbulent dispersion](#taylor-turbulent-dispersion)
    - [Power-law velocity-correlation dispersion](#power-law-velocity-correlation-dispersion)
    - [Lagrangian velocity autocorrelation](#lagrangian-velocity-autocorrelation)
    - [Lagrangian integral time](#lagrangian-integral-time)
  - [Forced stratified mixing with square-root power input](#forced-stratified-mixing-with-square-root-power-input)
  - [Stratified mixing energy budget](#stratified-mixing-energy-budget)
    - [Instantaneous mixing efficiency](#instantaneous-mixing-efficiency)
      - [Cumulative mixing efficiency](#cumulative-mixing-efficiency)
- [Turbulent plane jet similarity](#turbulent-plane-jet-similarity)
  - [Finite-edge stress condition for a mixing-length jet](#finite-edge-stress-condition-for-a-mixing-length-jet)
- [Mixing length](#mixing-length)
  - [Mixing-length closure](#mixing-length-closure)
- [Turbulent kinetic energy](#turbulent-kinetic-energy)
  - [Mean-shear production of turbulent kinetic energy](#mean-shear-production-of-turbulent-kinetic-energy)
  - [Local turbulent kinetic energy balance](#local-turbulent-kinetic-energy-balance)
    - [Fixed-correlation equilibrium model for stratified turbulence](#fixed-correlation-equilibrium-model-for-stratified-turbulence)
- [Reynolds stress](#reynolds-stress)
  - [Nondiffusive convective angular momentum transport](#nondiffusive-convective-angular-momentum-transport)
  - [Reynolds-stress energy production in a shearing sheet](#reynolds-stress-energy-production-in-a-shearing-sheet)
  - [Constant-stress Reynolds-averaged wall flow](#constant-stress-reynolds-averaged-wall-flow)
  - [Eddy viscosity](#eddy-viscosity)
  - [Reynolds-averaged momentum equation](#reynolds-averaged-momentum-equation)
- [Internal intermittency](#internal-intermittency)
  - [Kolmogorov refined similarity hypothesis](#kolmogorov-refined-similarity-hypothesis)
    - [Lognormal intermittency model](#lognormal-intermittency-model)
  - [Coarse-grained energy dissipation](#coarse-grained-energy-dissipation)
  - [Integral-scale intermittency](#integral-scale-intermittency)
    - [Landau intermittency counterexample](#landau-intermittency-counterexample)
- [Energy cascade](#energy-cascade)
  - [Spectral triad interaction](#spectral-triad-interaction)
  - [Zeroth law of turbulence](#zeroth-law-of-turbulence)
    - [Turbulent dissipation anomaly](#turbulent-dissipation-anomaly)
  - [Eddy turnover time](#eddy-turnover-time)
  - [Two-dimensional enstrophy cascade](#two-dimensional-enstrophy-cascade)
    - [Logarithmic structure function in an enstrophy cascade](#logarithmic-structure-function-in-an-enstrophy-cascade)
  - [Townsend-Betchov cascade cartoon](#townsend-betchov-cascade-cartoon)
  - [Kolmogorov 1941 theory](#kolmogorov-1941-theory)
    - [Kolmogorov second similarity hypothesis](#kolmogorov-second-similarity-hypothesis)
      - [Kolmogorov two-thirds law](#kolmogorov-two-thirds-law)
    - [Kolmogorov first similarity hypothesis](#kolmogorov-first-similarity-hypothesis)
  - [Equilibrium range](#equilibrium-range)
  - [Dissipation range](#dissipation-range)
    - [Kolmogorov microscales](#kolmogorov-microscales)
      - [Kolmogorov length scale](#kolmogorov-length-scale)
  - [Inertial range](#inertial-range)
- [Homogeneous turbulence](#homogeneous-turbulence)
  - [Integral scale of turbulence](#integral-scale-of-turbulence)
  - [Betchov relation](#betchov-relation)
  - [Isotropic turbulence](#isotropic-turbulence)
    - [Local isotropy of turbulence](#local-isotropy-of-turbulence)
    - [Loitsyansky integral](#loitsyansky-integral)
      - [Landau angular-momentum argument for turbulent decay](#landau-angular-momentum-argument-for-turbulent-decay)
      - [Kolmogorov decay law](#kolmogorov-decay-law)
    - [Saffman integral](#saffman-integral)
      - [Saffman decay law](#saffman-decay-law)
      - [Small-wavenumber spectrum with nonzero Saffman integral](#small-wavenumber-spectrum-with-nonzero-saffman-integral)
    - [Velocity correlation tensor](#velocity-correlation-tensor)
      - [Kármán-Howarth equation](#karman-howarth-equation)
        - [Kolmogorov equation for structure functions](#kolmogorov-equation-for-structure-functions)
          - [Kolmogorov four-fifths law](#kolmogorov-four-fifths-law)
      - [Longitudinal velocity correlation](#longitudinal-velocity-correlation)
        - [Longitudinal velocity structure function](#longitudinal-velocity-structure-function)
          - [Velocity increment](#velocity-increment)
          - [Large-scale contributions to structure functions](#large-scale-contributions-to-structure-functions)
          - [Structure-function spectral filter](#structure-function-spectral-filter)
    - [Turbulent energy spectrum](#turbulent-energy-spectrum)
    - [Longitudinal velocity-gradient skewness](#longitudinal-velocity-gradient-skewness)
- [Eddy diffusion](#eddy-diffusion)
  - [Buoyancy-driven turbulent density diffusion](#buoyancy-driven-turbulent-density-diffusion)
    - [Quintic density-profile similarity in an unstable tube](#quintic-density-profile-similarity-in-an-unstable-tube)
  - [Density-variance dissipation rate](#density-variance-dissipation-rate)
  - [Turbulent Prandtl number](#turbulent-prandtl-number)
    - [Reynolds analogy](#reynolds-analogy)
  - [Vertical turbulent buoyancy flux](#vertical-turbulent-buoyancy-flux)
  - [Buoyancy-gradient mixing-length closure](#buoyancy-gradient-mixing-length-closure)
    - [Arrested cubic buoyancy profile](#arrested-cubic-buoyancy-profile)
    - [Flux convergence in turbulent buoyancy mixing](#flux-convergence-in-turbulent-buoyancy-mixing)
- [Eddy diffusivity](#eddy-diffusivity)
  - [Turbulent Schmidt number](#turbulent-schmidt-number)
- [Turbulent round jet](#turbulent-round-jet)

## Reynolds averaging

↑ **Parent:** [Turbulence](turbulence.md)

[Reynolds averaging](#reynolds-averaging) separates a resolved mean from zero-mean fluctuations. The idealized averaging operation is linear and idempotent, commutes with the [derivatives](calculus.md#derivative) under consideration and treats resolved mean factors as constant inside its averaging scale. Products then satisfy $\overline{fg}=\overline f\,\overline g+\overline{f'g'}$. Actual finite spatial filters need scale separation or corrections when these rules are only approximate.

## External intermittency

↑ **Parent:** [Turbulence](turbulence.md)

A fixed observation point alternates between turbulent and non-turbulent fluid because a fluctuating interface passes it. This is distinct from [internal intermittency](#internal-intermittency), which concerns variations within fluid that remains turbulent.

## Wave turbulence

↑ **Parent:** [Turbulence](turbulence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_turbulence)

Wave turbulence describes the statistical transfer of energy between interacting [waves](physics.md#wave). The [wave period](physics.md#wave-period), nonlinear interaction time, phase correlations and resonances determine the transfer rate. A [weak wave cascade](#weak-wave-cascade) treats the change in one interaction as small; [critical balance](#critical-balance) instead makes the nonlinear interaction rate comparable to the linear wave frequency.

### Weak wave cascade

↑ **Parent:** [Wave turbulence](#wave-turbulence)

If a wave packet experiences a fractional nonlinear change $\chi=\tau_w/\tau_{\mathrm{nl}}\ll1$ per interaction, and successive interaction phases are decorrelated, $N$ changes add as a [random walk](markov-process.md#random-walk) of size $\sqrt N\chi$. Order-one transfer needs $N\sim\chi^{-2}$ interactions, giving the displayed cascade time. Phase coherence or resonant constraints can alter this estimate; weakness alone does not justify random addition.

## Magnetohydrodynamic turbulence

↑ **Parent:** [Turbulence](turbulence.md)

[Magnetohydrodynamic turbulence](#magnetohydrodynamic-turbulence) is irregular nonlinear motion of an electrically conducting fluid coupled to a [magnetic field](electromagnetism.md#magnetic-field). [Alfvén waves](astrophysical-fluid-dynamics.md#alfven-wave) and [magnetosonic waves](astrophysical-fluid-dynamics.md#magnetosonic-wave) give propagation times in addition to the nonlinear mixing time. A strong guide field distinguishes directions parallel and perpendicular to it, so the resulting cascades need not be isotropic.

### Dimensional freedom of an MHD spectrum

↑ **Parent:** [Magnetohydrodynamic turbulence](#magnetohydrodynamic-turbulence)

In a local isotropic hydrodynamic inertial-range model with only $\epsilon$ and $k$, dimensional analysis fixes the [Kolmogorov 1941 theory](#kolmogorov-1941-theory) spectrum. A mean [magnetic field](electromagnetism.md#magnetic-field) supplies the independent [Alfvén speed](astrophysical-fluid-dynamics.md#alfven-speed), permitting the arbitrary dimensionless function in the displayed formula even before anisotropy adds parallel scales. Cascade-time assumptions such as weak decorrelated interactions or [critical balance](#critical-balance) are therefore necessary to select an MHD spectrum.

### Electron-magnetohydrodynamic cascade

↑ **Parent:** [Magnetohydrodynamic turbulence](#magnetohydrodynamic-turbulence)

An electron-magnetohydrodynamic cascade transfers magnetic fluctuations through the nonlinear [electron magnetohydrodynamics](astrophysical-fluid-dynamics.md#electron-magnetohydrodynamics) induction equation. Writing $b_l=\delta B_l/B_0$, its perpendicular nonlinear interaction time is $\tau_{\mathrm{nl}}\sim l_\perp^2/(v_Ad_i b_l)$. The anisotropic [whistler wave](astrophysical-fluid-dynamics.md#whistler-wave) time is $\tau_w\sim l_\parallel l_\perp/(v_Ad_i)$. Scaling predictions depend on locality, phase decorrelation and the assumed balance of these times.

#### Critically balanced electron-magnetohydrodynamic cascade

↑ **Parent:** [Electron-magnetohydrodynamic cascade](#electron-magnetohydrodynamic-cascade)

[Critical balance](#critical-balance) sets $\tau_{\mathrm{nl}}\sim\tau_w$, hence $l_\parallel\sim l_\perp/b_l$. A local strong cascade with constant [energy flux](physics.md#energy-flux) has $\epsilon\sim v_A^3d_i b_l^3/l_\perp^2$, giving the displayed exponents and perpendicular [magnetic energy spectrum](electromagnetism.md#magnetic-energy-spectrum) $E_B(k_\perp)\propto k_\perp^{-7/3}$. The anisotropy becomes stronger towards small perpendicular scales.

#### Weak electron-magnetohydrodynamic cascade

↑ **Parent:** [Electron-magnetohydrodynamic cascade](#electron-magnetohydrodynamic-cascade)

For $b_ll_\parallel/l_\perp\ll1$, the [weak wave cascade](#weak-wave-cascade) estimate gives $\tau_{\mathrm{cas}}\sim l_\perp^3/(v_Ad_i b_l^2l_\parallel)$. Constant [energy flux](physics.md#energy-flux) $\epsilon\sim v_A^2b_l^2/\tau_{\mathrm{cas}}$ yields the displayed amplitude. An additionally isotropic local cascade has $b_l\propto l^{1/2}$ and shell-integrated [magnetic energy spectrum](electromagnetism.md#magnetic-energy-spectrum) $E_B(k)\propto k^{-2}$. These statements are phenomenological consequences of the chosen locality and decorrelation assumptions.

### Critical balance

↑ **Parent:** [Magnetohydrodynamic turbulence](#magnetohydrodynamic-turbulence)

[Critical balance](#critical-balance) is a scale-dependent ordering in which the wave-propagation time and nonlinear interaction time are comparable. For strong [Alfvénic turbulence](#alfvenic-turbulence), $k_\parallel v_A\sim k_\perp\delta u_\perp$. For [electron magnetohydrodynamics](astrophysical-fluid-dynamics.md#electron-magnetohydrodynamics), the linear rate is $v_Ad_i k_\parallel k_\perp$ and the nonlinear rate is $v_Ad_i k_\perp^2\delta B/B_0$, so [critical balance](#critical-balance) instead gives $\delta B/B_0\sim k_\parallel/k_\perp$. This assumption is an estimate of decorrelation dynamics, not an exact equality at every point.

<h3 id="alfvenic-turbulence">Alfvénic turbulence</h3>

↑ **Parent:** [Magnetohydrodynamic turbulence](#magnetohydrodynamic-turbulence)

[Alfvénic turbulence](#alfvenic-turbulence) is the turbulent interaction of fluctuations polarized primarily as [Alfvén waves](astrophysical-fluid-dynamics.md#alfven-wave). In [Elsässer variables](astrophysical-fluid-dynamics.md#elsasser-variable) $\mathbf z^\pm=\mathbf u_\perp\pm\delta\mathbf B_\perp/\sqrt{4\pi\rho_0}$, each [wave](physics.md#wave) population is nonlinearly distorted by the oppositely propagating population. Equal populations give a balanced cascade; unequal populations give an imbalanced cascade. The absence of one population removes the leading nonlinear interaction in ideal [reduced magnetohydrodynamics](astrophysical-fluid-dynamics.md#reduced-magnetohydrodynamics).

<h4 id="weak-alfvenic-cascade">Weak Alfvénic cascade</h4>

↑ **Parent:** [Alfvénic turbulence](#alfvenic-turbulence)

For balanced anisotropic [Alfvénic turbulence](#alfvenic-turbulence), suppose $\tau_A=l_\parallel/v_A\ll\tau_{\rm nl}=l_\perp/\delta z$ and resonant interactions preserve the parallel scale during the perpendicular cascade. Random encounter accumulation gives $\tau_{\rm cas}=v_Al_\perp^2/(\delta z^2l_\parallel)$. Constant [energy flux](physics.md#energy-flux) then gives $\delta z\propto l_\perp^{1/2}$ and the displayed perpendicular [turbulent energy spectrum](#turbulent-energy-spectrum). Unlike isotropic phenomenology, the fixed parallel scale is independent of the decreasing perpendicular scale.

<h5 id="weak-to-strong-transition-of-an-alfvenic-cascade">Weak-to-strong transition of an Alfvénic cascade</h5>

↑ **Parent:** [Weak Alfvénic cascade](#weak-alfvenic-cascade)

In a [weak Alfvénic cascade](#weak-alfvenic-cascade) at fixed $l_\parallel$, $\chi=\tau_A/\tau_{\rm nl}\propto l_\perp^{-1/2}$ grows as the perpendicular scale shrinks. If its outer value is $\chi_0\ll1$ at $L_\perp$, it reaches order one at the displayed scale. Beyond it the weak-interaction ordering fails and a [critical balance](#critical-balance) model may become appropriate.

#### Iroshnikov-Kraichnan spectrum

↑ **Parent:** [Alfvénic turbulence](#alfvenic-turbulence)

The [Iroshnikov-Kraichnan spectrum](#iroshnikov-kraichnan-spectrum) phenomenology assumes balanced, isotropic local [Alfvénic turbulence](#alfvenic-turbulence) with $\delta z_l\ll v_A$, decorrelated counterpropagating encounters, $\tau_A=l/v_A$ and $\tau_{\rm nl}=l/\delta z_l$. A [weak wave cascade](#weak-wave-cascade) takes $\tau_{\rm cas}\sim\tau_{\rm nl}^2/\tau_A=v_Al/\delta z_l^2$. Constant [energy flux](physics.md#energy-flux) gives $\delta z_l^4\sim\epsilon v_Al$ and the displayed shell-integrated [turbulent energy spectrum](#turbulent-energy-spectrum). Isotropy is an additional assumption, not a consequence of a strong guide field.

<h4 id="goldreich-sridhar-turbulence">Goldreich–Sridhar turbulence</h4>

↑ **Parent:** [Alfvénic turbulence](#alfvenic-turbulence)

[Goldreich–Sridhar turbulence](#goldreich-sridhar-turbulence) combines [critical balance](#critical-balance), balanced counterpropagating [Alfvén waves](astrophysical-fluid-dynamics.md#alfven-wave), a local perpendicular cascade, and constant [energy](classical-mechanics.md#energy) flux per unit mass $\mathcal E$. With $\tau_{\mathrm{nl}}\sim\ell_\perp/\delta u_\ell$ and $\mathcal E\sim\delta u_\ell^2/\tau_{\mathrm{nl}}$, one obtains $\delta u_\ell\sim(\mathcal E\ell_\perp)^{1/3}$. Defining the one-dimensional perpendicular [turbulent energy spectrum](#turbulent-energy-spectrum) by $\delta u_\ell^2\sim k_\perp E(k_\perp)$ gives $E(k_\perp)\sim\mathcal E^{2/3}k_\perp^{-5/3}$. [Critical balance](#critical-balance) also gives $k_\parallel\sim\mathcal E^{1/3}k_\perp^{2/3}/v_A$. This scaling argument neglects scale-dependent alignment and intermittency corrections, which are additional physical effects rather than consequences of the stated assumptions.

## Turbulence closure

↑ **Parent:** [Turbulence](turbulence.md)

A turbulence closure approximates the unclosed higher-order [moments](probability-theory.md#moment) in evolution equations for lower-order turbulent statistics. For example, an equation for the [velocity correlation tensor](#velocity-correlation-tensor) involves triple correlations, whose evolution involves fourth-order correlations and pressure. A closure must be checked against [conservation laws](physics.md#conservation-law), realizability and boundary conditions; matching an energy spectrum alone does not establish all these properties.

### Constant-skewness turbulence closure

↑ **Parent:** [Turbulence closure](#turbulence-closure)

This [turbulence closure](#turbulence-closure) assumes the [velocity increment](#velocity-increment) [skewness](probability-theory.md#skewness) is the same throughout the [equilibrium range](#equilibrium-range), with its value fixed by the [Kolmogorov two-thirds law](#kolmogorov-two-thirds-law) and [Kolmogorov four-fifths law](#kolmogorov-four-fifths-law). It yields a simple crossover between differentiable and inertial-scale increments, but suppresses the scale dependence of [skewness](probability-theory.md#skewness) and has no independent spectral-transfer dynamics.

#### Normalized constant-skewness structure-function equation

↑ **Parent:** [Constant-skewness turbulence closure](#constant-skewness-turbulence-closure)

Set $S_2=\sqrt{15}\beta^{3/2}v_\eta^2h$ and $r=(15\beta)^{3/4}\eta x$. The [Kolmogorov equation for structure functions](#kolmogorov-equation-for-structure-functions) and the [constant-skewness turbulence closure](#constant-skewness-turbulence-closure) give the displayed [ordinary differential equation](differential-equation.md#ordinary-differential-equation), with $h(0)=0$. Its small-separation balance is $h\sim x^2$; its large-separation balance is $h\sim x^{2/3}$. The first matches differentiable [velocity increments](#velocity-increment), and the second recovers the assumed [Kolmogorov two-thirds law](#kolmogorov-two-thirds-law).

### Eddy-damped quasi-normal Markovian closure

↑ **Parent:** [Turbulence closure](#turbulence-closure)

[EDQNM closure](#eddy-damped-quasi-normal-markovian-closure) models the evolution of the [turbulent energy spectrum](#turbulent-energy-spectrum) through [spectral triad interactions](#spectral-triad-interaction). Fourth-order correlations are approximated using products of second-order correlations, an eddy damping limits the resulting triple correlations, and their memory integrals are replaced by expressions using current spectra. The modeled damping times are additional physical input. This allows evolving spectra and scale-dependent transfer, but does not automatically recover coherent structures or [internal intermittency](#internal-intermittency). [Bertoglio, Squires and Ferziger's simulation comparison](https://ntrs.nasa.gov/api/citations/19880013707/downloads/19880013707.pdf) explains the damping assumptions and tests their limitations.

## K-epsilon turbulence model

↑ **Parent:** [Turbulence](turbulence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/K-epsilon_turbulence_model)

A two-equation closure transporting [turbulent kinetic energy](#turbulent-kinetic-energy) $k$ and its [turbulent kinetic energy dissipation rate](stokes-flow.md#turbulent-kinetic-energy-dissipation-rate) $\epsilon$. Its [eddy viscosity](#eddy-viscosity) is $C_\mu k^2/\epsilon$. In a high-Reynolds-number wall-normal reduction, turbulent diffusion has coefficients $\nu_T/\sigma_k$ and $\nu_T/\sigma_\epsilon$; the energy equation has shear production $P$ and destruction $\epsilon$, while the dissipation equation has modeled production $C_{\epsilon1}P\epsilon/k$ and destruction $C_{\epsilon2}\epsilon^2/k$. The dissipation production/destruction terms are closure terms, not a second conservation of energy.

### K-epsilon turbulence front

↑ **Parent:** [K-epsilon turbulence model](#k-epsilon-turbulence-model)

A stationary turbulence edge with no production has an advection–turbulent-diffusion leading balance. For $k\propto x^p$, $\epsilon\propto x^q$ and $\nu_T=C_\mu k^2/\epsilon$, this balance gives $2p-q=1$ and $q/p=\sigma_\epsilon/\sigma_k=\sigma$. The integral length $k^{3/2}/\epsilon$ and turnover frequency $\epsilon/k$ both tend to zero when $1<\sigma<3/2$. The front viscosity is linear, with $\nu_T'(0^+)=(2\sigma_k-\sigma_\epsilon)U_0$. This is formal high-Reynolds-number consistency, not a uniform justification for neglecting molecular viscosity at the exact edge.

### Log-layer solution of the k-epsilon model

↑ **Parent:** [K-epsilon turbulence model](#k-epsilon-turbulence-model)

In the constant-stress overlap layer, the [law of the wall](continuum-mechanics.md#law-of-the-wall) gives $U_y=u_*/(\kappa y)$ and the [Reynolds stress](#reynolds-stress) gives $-\overline{u'v'}\simeq u_*^2$. Thus $\nu_T=u_*\kappa y$ and local balance gives $P\simeq\epsilon=u_*^3/(\kappa y)$. Combining with the [K-epsilon model](#k-epsilon-turbulence-model) viscosity formula gives the displayed constant $k$. The energy diffusion term then vanishes. The dissipation diffusion term does not: it is $u_*^4/(\sigma_\epsilon y^2)$. Balancing it against the dissipation-equation source terms yields the displayed [Von Kármán constant](continuum-mechanics.md#von-karman-constant) relation. Neglecting dissipation diffusion would incorrectly require equal production and destruction constants.

## Turbulent mixing

↑ **Parent:** [Turbulence](turbulence.md)

Turbulent mixing redistributes a transported scalar, such as temperature or particle [concentration](physics.md#concentration), through irregular fluid motions and eventual molecular diffusion. A [top-hat plume model](turbulent-plume.md#top-hat-plume-model) assumes this mixing keeps the scalar approximately uniform within a selected cross section; that uniformity is an additional closure, not a consequence of thin geometry alone.

### Richardson pair dispersion

↑ **Parent:** [Turbulent mixing](#turbulent-mixing)

Richardson pair dispersion concerns relative separation of two marked [fluid elements](continuum-mechanics.md#fluid-element), rather than their centre-of-mass motion. In an [inertial range](#inertial-range), scale-local relative diffusivity is of order $\epsilon^{1/3}r^{4/3}$. A self-similar closure gives $d\langle r^2\rangle/dt=A\epsilon^{1/3}\langle r^2\rangle^{2/3}$ and hence a $t^3$ regime after loss of memory of initial separation. Stationarity and inertial-range separation alone do not imply this law at arbitrarily short times.

#### Three-regime turbulent pair-separation model

↑ **Parent:** [Richardson pair dispersion](#richardson-pair-dispersion)

For positive initial separation below the [Kolmogorov length scale](#kolmogorov-length-scale), a phenomenological pair-dispersion model has smooth-flow exponential stretching, inertial-range [Richardson pair dispersion](#richardson-pair-dispersion), and [diffusive large-scale pair dispersion](#diffusive-large-scale-pair-dispersion) beyond the [integral scale of turbulence](#integral-scale-of-turbulence). A positive [Lyapunov exponent](dynamical-systems.md#lyapunov-exponent) is needed for the first regime, scale locality and initial-memory loss for the second, and integrable relative-velocity [autocorrelation](time-series.md#autocorrelation) for the third. The inertial-range crossing time is of order $L^{2/3}\epsilon^{-1/3}$, one outer [eddy turnover time](#eddy-turnover-time).

#### Diffusive large-scale pair dispersion

↑ **Parent:** [Richardson pair dispersion](#richardson-pair-dispersion)

At separations well above the [integral scale of turbulence](#integral-scale-of-turbulence), two fluid velocities can decorrelate spatially. If the relative-velocity [autocorrelation](time-series.md#autocorrelation) $R_{\mathrm{rel}}$ is stationary and integrable, the displacement identity used in [Taylor turbulent dispersion](#taylor-turbulent-dispersion) gives the displayed long-time linear mean-square growth. With speed $U$ and [Lagrangian integral time](#lagrangian-integral-time) of order $L/U$, its relative [diffusivity](brownian-motion.md#diffusion-coefficient) is of order $UL$. The characteristic separation grows as $t^{1/2}$, unlike inertial-range [Richardson pair dispersion](#richardson-pair-dispersion).

#### Richardson constant

↑ **Parent:** [Richardson pair dispersion](#richardson-pair-dispersion)

The dimensionless Richardson constant is the coefficient in the mean-square pair-separation law. Under the simple self-similar diffusivity closure, $g=(A/3)^3$. Its universality requires scale locality, adequate scale separation and loss of initial-condition memory; a finite-time fit need not isolate this asymptotic coefficient.

### Taylor turbulent dispersion

↑ **Parent:** [Turbulent mixing](#turbulent-mixing)

Taylor turbulent dispersion describes the absolute displacement of a marked [fluid element](continuum-mechanics.md#fluid-element) in stationary [homogeneous turbulence](#homogeneous-turbulence). Here $R_L$ is its Lagrangian velocity [autocorrelation](time-series.md#autocorrelation). Continuous correlation at zero gives ballistic spreading at short times, and an integrable correlation gives diffusive spreading at long times. This is distinct from shear-induced [Taylor dispersion](fluid-mechanics.md#taylor-dispersion) and from [Richardson pair dispersion](#richardson-pair-dispersion).

#### Power-law velocity-correlation dispersion

↑ **Parent:** [Taylor turbulent dispersion](#taylor-turbulent-dispersion)

For a zero-mean stationary [velocity](classical-mechanics.md#velocity) process of variance $\sigma_v^2$ and normalized [autocorrelation](time-series.md#autocorrelation) $(1+|s|)^{-\alpha}$, integrating velocity twice gives the displayed expression, exactly rather than just asymptotically. For $\alpha>1$ the long-time [diffusion coefficient](brownian-motion.md#diffusion-coefficient) is $\sigma_v^2/(\alpha-1)$. At $\alpha=1$, the displacement variance is asymptotic to $2\sigma_v^2t\log t$. For $0<\alpha<1$, it is asymptotic to $2\sigma_v^2t^{2-\alpha}/[(1-\alpha)(2-\alpha)]$. Linear variance growth does not by itself imply a [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) or a [normal distribution](probability-theory.md#normal-distribution) for displacement.

#### Lagrangian velocity autocorrelation

↑ **Parent:** [Taylor turbulent dispersion](#taylor-turbulent-dispersion)

For stationary statistics along a [Lagrangian trajectory](continuum-mechanics.md#lagrangian-trajectory) $\mathbf X$, the velocity [autocorrelation](time-series.md#autocorrelation) depends on the lag $s$. Integrating velocity twice gives the mean-square displacement $2\int_0^t(t-s)R_L(s)ds$. If $R_L$ is integrable, the long-time displacement is diffusive. Its normalized one-sided area is the [Lagrangian integral time](#lagrangian-integral-time).

#### Lagrangian integral time

↑ **Parent:** [Taylor turbulent dispersion](#taylor-turbulent-dispersion)

The Lagrangian integral time is the area under a normalized velocity [autocorrelation](time-series.md#autocorrelation) along a [Lagrangian trajectory](continuum-mechanics.md#lagrangian-trajectory). If this correlation is integrable, Taylor turbulent dispersion has asymptotic mean-square displacement $2R_L(0)t_Lt$. The integral time need not equal every short-time decorrelation scale, particularly when the autocorrelation oscillates.

### Forced stratified mixing with square-root power input

↑ **Parent:** [Turbulent mixing](#turbulent-mixing)

For $A=U_0^2(1/L_f-1/L_\rho)>0$, define $K_\infty=A L_v$ and $y=\sqrt{K/K_\infty}$. The positive-energy solution is $y(t)=[y_0+\tanh(\sqrt{K_\infty}t/(2L_v))]/[1+y_0\tanh(\sqrt{K_\infty}t/(2L_v))]$. Energies above and below $K_\infty$ approach it from their respective sides. The zero-energy equation is not Lipschitz and admits both permanent rest and delayed startup, so a unique positive steady limit needs a positive seed or an additional startup prescription. With negligible available and internal energy exchange, the long-time [instantaneous mixing efficiency](#instantaneous-mixing-efficiency) fraction is $L_f/L_\rho$, independent of $L_v$.

### Stratified mixing energy budget

↑ **Parent:** [Turbulent mixing](#turbulent-mixing)

With boundary fluxes suppressed, let $B$ transfer [kinetic energy](classical-mechanics.md#kinetic-energy) to [potential energy](classical-mechanics.md#potential-energy), $M$ transfer [available potential energy](classical-mechanics.md#available-potential-energy) irreversibly to [background potential energy](classical-mechanics.md#background-potential-energy), and $W$ transfer [internal energy](thermodynamics.md#internal-energy) to potential energy. Then $\dot P=B+W$, $\dot P_b=M+W$, $\dot A=B-M$, and $\dot K=F-B-\epsilon$. The internal reservoir has $\dot I=\epsilon-W$, conserving total energy apart from forcing $F$. The distinction between reversible buoyancy exchange and irreversible mixing is essential outside a quasi-steady negligible-$A$ regime.

#### Instantaneous mixing efficiency

↑ **Parent:** [Stratified mixing energy budget](#stratified-mixing-energy-budget)

Instantaneous mixing efficiency is the fraction of instantaneous irreversible mechanical-energy loss that raises [background potential energy](classical-mechanics.md#background-potential-energy), after subtracting internal-to-potential exchange. The ratio $\Gamma=M/\epsilon$ is a different quantity, related by $\eta=\Gamma/(1+\Gamma)$. Replacing $M$ by buoyancy exchange $B$ additionally assumes negligible change of [available potential energy](classical-mechanics.md#available-potential-energy).

##### Cumulative mixing efficiency

↑ **Parent:** [Instantaneous mixing efficiency](#instantaneous-mixing-efficiency)

Cumulative mixing efficiency is the ratio of total irreversible density-mixing conversion to total irreversible mechanical-energy loss over an interval. It is a loss-rate-weighted average of [instantaneous mixing efficiency](#instantaneous-mixing-efficiency), not an unweighted time average. Stored [kinetic energy](classical-mechanics.md#kinetic-energy), changes in [available potential energy](classical-mechanics.md#available-potential-energy) and boundary work must be accounted for before replacing its denominator by integrated forcing.

## Turbulent plane jet similarity

↑ **Parent:** [Turbulence](turbulence.md)

For a slender plane jet with conserved specific momentum flux $M_0=\int U^2dy$ and a [mixing length](#mixing-length) proportional to transverse position, dimensional balance gives width proportional to $x$ and centreline speed proportional to $\sqrt{M_0/x}$. The [streamfunction](fluid-mechanics.md#stream-function) $\psi=\sqrt{M_0x}f(\eta)$, $\eta=y/x$, yields $U=\sqrt{M_0/x}f'$ and $V=\sqrt{M_0/x}(\eta f'-f/2)$. With $l=C_1|y|$, the upper-half [Reynolds-averaged momentum equation](#reynolds-averaged-momentum-equation) integrates to $ff'=2C_1^2\eta^2(f'')^2$ for a finite centreline velocity and zero centreline stress. The momentum normalization is $2\int_0^{\eta_w}(f')^2d\eta=1$ for a compact jet, or the same integral to infinity for a decaying jet. These formal equations do not justify an independently imposed edge condition.

### Finite-edge stress condition for a mixing-length jet

↑ **Parent:** [Turbulent plane jet similarity](#turbulent-plane-jet-similarity)

For a symmetric localized [turbulent plane jet similarity](#turbulent-plane-jet-similarity) profile, integrated momentum balance gives $ff'=2C_1^2\eta^2(f'')^2$ on $\eta>0$. At a finite free edge $\eta_w>0$, $f'(\eta_w)=0$ and finite $f(\eta_w)$ force $f''(\eta_w)=0$. Thus the [mixing length](#mixing-length) model $l=C_1|y|$ cannot simultaneously impose zero velocity and a nonzero maximum velocity gradient at the edge. Its [eddy viscosity](#eddy-viscosity) vanishes there. Moreover, a nonzero finite centreline speed $f'(0)=a$ forces $|f''|\sim a/(\sqrt2C_1\sqrt\eta)$ near the centre, displaying a singular-shear defect of that local closure. The molecular-viscosity neglect cannot be uniform in this core.

## Mixing length

↑ **Parent:** [Turbulence](turbulence.md)

A mixing length is the characteristic transverse displacement over which a turbulent parcel retains its streamwise momentum before mixing with its surroundings. Taylor expansion of a mean velocity profile gives a fluctuation of magnitude $l|U_y|$. Combining comparable transverse fluctuations with down-gradient [Reynolds stress](#reynolds-stress) transport gives the closure $\overline{u'v'}=-l^2|U_y|U_y$. This is a phenomenological approximation, not a consequence of the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation). In a free jet, a prescribed local [mixing length](#mixing-length) must also be compatible with centreline regularity and vanishing outer momentum flux.

### Mixing-length closure

↑ **Parent:** [Mixing length](#mixing-length)

A mixing-length closure uses a prescribed [mixing length](#mixing-length) $\ell$ to approximate turbulent transport. For mean shear $\partial_zU$, a standard model gives [eddy viscosity](#eddy-viscosity) $\nu_t=\ell^2|\partial_zU|$ and down-gradient [Reynolds stress](#reynolds-stress). Scalar-diffusion versions replace momentum transport by an appropriate scalar flux. The choice of length and correlations is a modelling assumption rather than an exact closure of the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation).

## Turbulent kinetic energy

↑ **Parent:** [Turbulence](turbulence.md)

Kinetic energy per unit mass in velocity fluctuations. Mean shear, buoyancy and transport supply or redistribute it, while molecular viscosity dissipates it. Its local budget motivates the [local turbulent kinetic energy balance](#local-turbulent-kinetic-energy-balance) when storage and transport are negligible.

### Mean-shear production of turbulent kinetic energy

↑ **Parent:** [Turbulent kinetic energy](#turbulent-kinetic-energy)

The work of the [Reynolds stress](#reynolds-stress) against the mean velocity gradient transfers kinetic energy from the mean flow into fluctuations. In a plane shear flow $U(y)$ this is $P=-\overline{u'v'}U_y$. The [eddy viscosity](#eddy-viscosity) closure gives $P=\nu_T U_y^2\geq0$. Buoyancy production and transport are separate terms in the [turbulent kinetic energy](#turbulent-kinetic-energy) budget.

### Local turbulent kinetic energy balance

↑ **Parent:** [Turbulent kinetic energy](#turbulent-kinetic-energy)

In stationary locally equilibrated turbulence, mean-shear production and buoyancy production balance viscous dissipation after transport terms are neglected. Stable buoyancy flux is negative and consumes part of the shear input. This approximation gives $\epsilon=u_*^3/(\kappa z)$ in a neutral logarithmic layer and $\epsilon\sim B_0$ in buoyancy-dominated free convection.

#### Fixed-correlation equilibrium model for stratified turbulence

↑ **Parent:** [Local turbulent kinetic energy balance](#local-turbulent-kinetic-energy-balance)

Let $S=U_z>0$, $N^2=-(g/\rho_0)\overline\rho_z>0$, $q^2=\overline{u_i'u_i'}$, and constant correlations $C_u=-\overline{u'w'}/q^2$ and $C_\rho^2=\overline{\rho'w'}^2/(q^2\overline{\rho'^2})$. Using $\epsilon=q^3/L_u$ and $\chi=\overline{\rho'^2}q/L_\rho$, the scalar-variance balance implies $\overline{\rho'w'}=-C_\rho^2L_\rho q\overline\rho_z$. Substituting in the energy budget gives the displayed quadratic for $q>0$.

Write $a=C_\rho^2L_\rho N^2/(C_uS)$ and $b=1/(L_uC_uS)$. The ratio of total sinks to production is $R=a/q+bq$. Positive equilibria exist only for $4ab\leq1$, equivalent to $\mathrm{Ri}\leq L_uC_u^2/(4L_\rho C_\rho^2)$. The larger-$q$ root has flux Richardson number $(1-\sqrt{1-4ab})/2$; the smaller root has the plus sign. Under the local kinetic-energy evolution the larger root is stable and the smaller root unstable. The critical value is closure-dependent and is not the universal inviscid linear-stability threshold.

## Reynolds stress

↑ **Parent:** [Turbulence](turbulence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reynolds_stress)

Velocity-fluctuation covariances transport mean momentum. For positive wall shear, $-\overline{u'w'}$ is the downward momentum-transport magnitude and contributes to the total shear stress. Some stress conventions include the minus sign in the definition of the tensor itself; the momentum equation must use the same convention.

### Nondiffusive convective angular momentum transport

↑ **Parent:** [Reynolds stress](#reynolds-stress)

Rotating anisotropic [convection](fluid-mechanics.md#convection) can produce an azimuthal-meridional [velocity](classical-mechanics.md#velocity) correlation even without a gradient of the mean rotation rate. Its [Reynolds stress](#reynolds-stress) transports [angular momentum](classical-mechanics.md#angular-momentum) and can drive [differential rotation](astrophysical-fluid-dynamics.md#differential-rotation), whereas a purely viscous closure only erases shear. Energy comes from the thermally driven [convection](fluid-mechanics.md#convection); the [Coriolis force](physics.md#coriolis-force) changes the correlations but does no work on a parcel.

### Reynolds-stress energy production in a shearing sheet

↑ **Parent:** [Reynolds stress](#reynolds-stress)

For shear $\mathbf u_0=-2Ax\mathbf e_y$, the spatially averaged perturbation [kinetic energy](classical-mechanics.md#kinetic-energy) obeys $dE/dt=2A\rho\langle u_x'u_y'\rangle-\rho\nu\langle|\nabla\mathbf u'|^2\rangle$. [Pressure](thermodynamics.md#pressure) and the [Coriolis force](physics.md#coriolis-force) do no net work. Thus positive radial-azimuthal velocity correlation extracts mean-flow [energy](classical-mechanics.md#energy). A leading two-dimensional [shearing wave](gravitational-instability-of-an-astrophysical-disk.md#shearing-wave) has $\operatorname{Re}(v_xv_y^*)=-k_xk_y|Z|^2/k^4>0$.

// Target: astrophysics.bigb

### Constant-stress Reynolds-averaged wall flow

↑ **Parent:** [Reynolds stress](#reynolds-stress)

For a stationary, horizontally homogeneous mean flow without a horizontal pressure gradient, the averaged horizontal [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) is $\nu U_{zz}-(\overline{u'w'})_z=0$. Integrating gives the displayed physical [shear stress](viscous-fluid-flow.md#shear-stress). The derivative of the Reynolds covariance belongs in the stress-divergence equation, not inside the stress itself. The kinematic stress is $\tau_d/\rho$, which must be used when an [eddy viscosity](#eddy-viscosity) with units of kinematic viscosity multiplies the mean gradient.

### Eddy viscosity

↑ **Parent:** [Reynolds stress](#reynolds-stress)

An eddy viscosity parametrizes turbulent momentum transport by $\overline{u'v'}=-\nu_TU_y$. The [mixing length](#mixing-length) model gives $\nu_T=l^2|U_y|\geq0$. This coefficient depends on the mean flow and position; it is distinct from molecular [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity). It describes momentum transport rather than molecular energy dissipation.

### Reynolds-averaged momentum equation

↑ **Parent:** [Reynolds stress](#reynolds-stress)

An [Eulerian time average](continuum-mechanics.md#eulerian-time-average) of an incompressible constant-density [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) gives the displayed mean momentum equation. Decompose velocity into its mean and a zero-mean fluctuation. In conservative form, the averaged momentum flux is $\overline{u_iu_j}=U_iU_j+\overline{u_i'u_j'}$; mean [incompressibility](fluid-mechanics.md#incompressible-flow) then turns its first term into mean advection. The fluctuation covariance is the [Reynolds stress](#reynolds-stress) divided by density, using the positive covariance convention. Closing this extra unknown requires a turbulence model.

## Internal intermittency

↑ **Parent:** [Turbulence](turbulence.md)

[Internal intermittency](#internal-intermittency) is the fluctuating concentration of gradients, transfer and [viscous dissipation](stokes-flow.md#viscous-dissipation) inside turbulent fluid. It is distinct from an interface between turbulent and non-turbulent regions intermittently passing an observer. Its scale dependence is reflected in non-Gaussian increments and coarse-grained [viscous dissipation](stokes-flow.md#viscous-dissipation) [moments](probability-theory.md#moment).

### Kolmogorov refined similarity hypothesis

↑ **Parent:** [Internal intermittency](#internal-intermittency)

[Refined similarity](#kolmogorov-refined-similarity-hypothesis) writes $\Delta v=(r\epsilon_r)^{1/3}V$ with universal normalized conditional statistics at high local [Reynolds number](fluid-mechanics.md#reynolds-number). Then $S_p=C_pr^{p/3}\langle\epsilon_r^{p/3}\rangle$. The distribution of [coarse-grained energy dissipation](#coarse-grained-energy-dissipation) need not be universal. [Refined similarity](#kolmogorov-refined-similarity-hypothesis) itself does not prescribe that distribution.

#### Lognormal intermittency model

↑ **Parent:** [Kolmogorov refined similarity hypothesis](#kolmogorov-refined-similarity-hypothesis)

If $\log(\epsilon_r/\epsilon)$ is Gaussian with [variance](variance.md) $\sigma_r^2$, normalization gives $\langle\epsilon_r^q\rangle/\epsilon^q=\exp[q(q-1)\sigma_r^2/2]$. Taking $\exp(\sigma_r^2)=B(\ell/r)^\mu$ predicts $\zeta_p=p/3-\mu p(p-3)/18$. Its eventual negative high-order exponents show that this extrapolation cannot hold for arbitrarily large orders with finite uniform velocity [moments](probability-theory.md#moment).

### Coarse-grained energy dissipation

↑ **Parent:** [Internal intermittency](#internal-intermittency)

[Coarse-grained energy dissipation](#coarse-grained-energy-dissipation) is a spatial average of the local rate $2\nu S_{ij}S_{ij}$ over a region of size $r$. Its random value $\epsilon_r$ has mean $\epsilon$ in [homogeneous turbulence](#homogeneous-turbulence). [Refined similarity](#kolmogorov-refined-similarity-hypothesis) uses this local averaged [viscous dissipation](stokes-flow.md#viscous-dissipation) to scale velocity increments.

### Integral-scale intermittency

↑ **Parent:** [Internal intermittency](#internal-intermittency)

[Integral-scale intermittency](#integral-scale-intermittency) is modulation of the energy-containing motions and the energy supply on large lengths or long turnover times. Averaging velocity statistics over regions or realizations with differing [viscous dissipation](stokes-flow.md#viscous-dissipation) rates can invalidate universal coefficients based only on the global mean [viscous dissipation](stokes-flow.md#viscous-dissipation).

#### Landau intermittency counterexample

↑ **Parent:** [Integral-scale intermittency](#integral-scale-intermittency)

Mixing turbulent populations with differing [viscous dissipation](stokes-flow.md#viscous-dissipation) gives $S_p=\beta_pr^{p/3}\langle\epsilon_a^{p/3}\rangle$. Relative to the same power of the mean [viscous dissipation](stokes-flow.md#viscous-dissipation), the coefficient changes with the intensity distribution except at $p=3$. Thus universality of all unconditional coefficients is incompatible with arbitrary [integral-scale intermittency](#integral-scale-intermittency).

## Energy cascade

↑ **Parent:** [Turbulence](turbulence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Energy_cascade)

An [energy cascade](#energy-cascade) transfers [kinetic energy](classical-mechanics.md#kinetic-energy) among scales through nonlinear motion. A forward cascade carries energy toward smaller spatial scales, where [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) can dissipate it. Conservation and a mean scale-space flux do not uniquely prescribe the geometry or locality of the transfer mechanism.

### Spectral triad interaction

↑ **Parent:** [Energy cascade](#energy-cascade)

The quadratic nonlinear term of the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) couples three [Fourier modes](fourier-analysis.md#fourier-mode) whose [wave vectors](continuum-mechanics.md#wavevector) close to a triangle. These [spectral triad interactions](#spectral-triad-interaction) transfer [kinetic energy](classical-mechanics.md#kinetic-energy) between wave numbers. A [turbulence closure](#turbulence-closure) can model their triple correlations while retaining more scale information than a prescribed local power law.

### Zeroth law of turbulence

↑ **Parent:** [Energy cascade](#energy-cascade)

At fixed outer [velocity](classical-mechanics.md#velocity) and [integral scale of turbulence](#integral-scale-of-turbulence), the mean [viscous dissipation](stokes-flow.md#viscous-dissipation) per unit mass approaches a positive finite value as the [Reynolds number](fluid-mechanics.md#reynolds-number) becomes large. The dimensionless coefficient $C_\epsilon=\epsilon\ell/u^3$ is then of order one. This is a phenomenological property of established three-dimensional [turbulence](turbulence.md), not a consequence of taking [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) to zero in an arbitrary smooth flow.

#### Turbulent dissipation anomaly

↑ **Parent:** [Zeroth law of turbulence](#zeroth-law-of-turbulence)

Although the local [viscous dissipation](stokes-flow.md#viscous-dissipation) is $2\nu S_{ij}S_{ij}$, increasingly intense [velocity gradients](continuum-mechanics.md#velocity-gradient) can compensate for vanishing [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity). A [Burgers vortex](continuum-mechanics.md#burgers-vortex) illustrates this mechanism: its radius shrinks while its excess integrated [viscous dissipation](stokes-flow.md#viscous-dissipation) remains finite. Such a local model does not by itself prove the [zeroth law of turbulence](#zeroth-law-of-turbulence) for a whole flow.

### Eddy turnover time

↑ **Parent:** [Energy cascade](#energy-cascade)

The eddy turnover time estimates how long a velocity difference $\delta u_l$ takes to distort a structure of size $l$. In a local strong [energy cascade](#energy-cascade), the transfer time is assumed comparable to it. A [weak wave cascade](#weak-wave-cascade) can transfer energy much more slowly because a single encounter makes only a small fractional change.

### Two-dimensional enstrophy cascade

↑ **Parent:** [Energy cascade](#energy-cascade)

A two-dimensional forward [two-dimensional enstrophy cascade](#two-dimensional-enstrophy-cascade) has the idealized spectrum $E(k)\propto k^{-3}$. The energy integral above a wavenumber scales as its inverse square, whereas the cumulative [enstrophy](fluid-mechanics.md#enstrophy) integral $\int k^2E(k)\,dk$ grows logarithmically. The spectrum used here omits possible further logarithmic corrections.

#### Logarithmic structure function in an enstrophy cascade

↑ **Parent:** [Two-dimensional enstrophy cascade](#two-dimensional-enstrophy-cascade)

For a wide $Ck^{-3}$ range and separation well below its outer scale, the second-order [longitudinal structure function](#longitudinal-velocity-structure-function) is controlled by $\int_{k_0}^{\pi/r}k^2E(k)\,dk$. The low-wavenumber filter term gives $S_2(r)\simeq Cr^2\log[\pi/(k_0r)]/4$, larger than the order-$r^2$ energy above the cutoff. This is a marginal dependence on larger-scale [enstrophy](fluid-mechanics.md#enstrophy).

### Townsend-Betchov cascade cartoon

↑ **Parent:** [Energy cascade](#energy-cascade)

The [Townsend-Betchov cascade cartoon](#townsend-betchov-cascade-cartoon) organizes [inertial range](#inertial-range) [vorticity](fluid-mechanics.md#vorticity) into sheets by [bi-axial strain](viscous-fluid-flow.md#bi-axial-strain), then uses sheet instability and roll-up to generate finer [vortex tubes](fluid-mechanics.md#vortex-tube). Dissipative tube cores balance stretching with [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity). Such differing mechanisms across scales challenge literal identical-step, memoryless cascade models without contradicting a mean [energy flux](physics.md#energy-flux).

### Kolmogorov 1941 theory

↑ **Parent:** [Energy cascade](#energy-cascade)

[Kolmogorov 1941 theory](#kolmogorov-1941-theory) assumes locally universal small-scale velocity statistics set by mean [viscous dissipation](stokes-flow.md#viscous-dissipation) and [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) at large [Reynolds number](fluid-mechanics.md#reynolds-number). In its [inertial range](#inertial-range) dimensional form, $S_p(r)\sim\epsilon^{p/3}r^{p/3}$. Large-scale modulation and [internal intermittency](#internal-intermittency) require qualifying this unconditional scaling.

#### Kolmogorov second similarity hypothesis

↑ **Parent:** [Kolmogorov 1941 theory](#kolmogorov-1941-theory)

In the [inertial range](#inertial-range), [velocity increment](#velocity-increment) statistics also become independent of [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity). Combined with the [Kolmogorov first similarity hypothesis](#kolmogorov-first-similarity-hypothesis), this gives $S_p(r)=\beta_p(\epsilon r)^{p/3}$ by [dimensional analysis](physics.md#dimensional-analysis). Signed integer [moments](probability-theory.md#moment) and absolute noninteger [moments](probability-theory.md#moment) must be distinguished; the signed third-order coefficient is negative in a forward [energy cascade](#energy-cascade).

##### Kolmogorov two-thirds law

↑ **Parent:** [Kolmogorov second similarity hypothesis](#kolmogorov-second-similarity-hypothesis)

The second-order [longitudinal structure function](#longitudinal-velocity-structure-function) has the displayed form in the idealized [inertial range](#inertial-range) of [Kolmogorov 1941 theory](#kolmogorov-1941-theory). It predicts that the typical longitudinal [velocity increment](#velocity-increment) grows as the cube root of separation. Unlike the [Kolmogorov four-fifths law](#kolmogorov-four-fifths-law), its exponent and coefficient are not exact consequences of the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation).

#### Kolmogorov first similarity hypothesis

↑ **Parent:** [Kolmogorov 1941 theory](#kolmogorov-1941-theory)

In the locally isotropic [equilibrium range](#equilibrium-range), the small-scale [velocity increment](#velocity-increment) statistics depend on the separation, mean [viscous dissipation](stokes-flow.md#viscous-dissipation) and [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity), independently of large-scale forcing details. [Dimensional analysis](physics.md#dimensional-analysis) leaves the [Kolmogorov microscales](#kolmogorov-microscales) as normalization scales and gives the displayed second-order [longitudinal structure function](#longitudinal-velocity-structure-function). Universality of $F$ is part of the hypothesis, not something proved by [dimensional analysis](physics.md#dimensional-analysis).

### Equilibrium range

↑ **Parent:** [Energy cascade](#energy-cascade)

The [equilibrium range](#equilibrium-range) consists of scales below the energy-containing motions whose statistics can adjust rapidly to the local energy supply. It includes the [inertial range](#inertial-range) and dissipative scales. Approximate equilibrium concerns mean transfer and [viscous dissipation](stokes-flow.md#viscous-dissipation), not absence of intermittent spatial fluctuations.

### Dissipation range

↑ **Parent:** [Energy cascade](#energy-cascade)

The [dissipation range](#dissipation-range) contains scales at which [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) appreciably affects [velocity gradients](continuum-mechanics.md#velocity-gradient) and converts [kinetic energy](classical-mechanics.md#kinetic-energy) into heat. In a high-Reynolds-number three-dimensional cascade its characteristic length and time are the [Kolmogorov microscales](#kolmogorov-microscales). Intense vortex cores can be intermittent within this range.

#### Kolmogorov microscales

↑ **Parent:** [Dissipation range](#dissipation-range)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov_microscales)

The Kolmogorov length, velocity and time are $\eta=(\nu^3/\epsilon)^{1/4}$, $v_\eta=(\nu\epsilon)^{1/4}$ and $\tau_\eta=(\nu/\epsilon)^{1/2}$. With $\epsilon\sim u^3/\ell$, their ratios to the [integral scales of turbulence](#integral-scale-of-turbulence) are powers of the [Reynolds number](fluid-mechanics.md#reynolds-number). They describe a mean scale balance; intermittent dissipative structures can have other local scales.

##### Kolmogorov length scale

↑ **Parent:** [Kolmogorov microscales](#kolmogorov-microscales)

The Kolmogorov length scale is the length among the [Kolmogorov microscales](#kolmogorov-microscales). [Kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu$ and mean energy dissipation per unit mass $\epsilon$ give the displayed dimensional scale. The associated speed is $(\nu\epsilon)^{1/4}$, so the [Reynolds number](fluid-mechanics.md#reynolds-number) formed at this length is one.

### Inertial range

↑ **Parent:** [Energy cascade](#energy-cascade)

The [inertial range](#inertial-range) lies between the energy-containing and viscous scales. Direct forcing and [viscous dissipation](stokes-flow.md#viscous-dissipation) are small there, and nonlinear transfer carries an approximately constant mean [energy flux](physics.md#energy-flux) in a three-dimensional forward cascade. Scale similarity and universality are additional statistical hypotheses.

## Homogeneous turbulence

↑ **Parent:** [Turbulence](turbulence.md)

[Homogeneous turbulence](#homogeneous-turbulence) has velocity statistics unchanged by translating all observation points. Mean spatial divergences vanish when the [moments](probability-theory.md#moment) exist and averaging commutes with derivatives. Homogeneity is distinct from isotropy: it does not require equal statistics in different directions.

### Integral scale of turbulence

↑ **Parent:** [Homogeneous turbulence](#homogeneous-turbulence)

The [integral scale of turbulence](#integral-scale-of-turbulence) characterizes energy-containing velocity correlations; in [isotropic turbulence](#isotropic-turbulence) one definition is $\ell=\int_0^\infty f(r)\,dr$. Its turnover time is of order $\ell/u$. Large-scale intensity fluctuations can change the energy supplied to the [equilibrium range](#equilibrium-range).

### Betchov relation

↑ **Parent:** [Homogeneous turbulence](#homogeneous-turbulence)

For differentiable homogeneous [incompressible flow](fluid-mechanics.md#incompressible-flow), $\langle\operatorname{tr}A^3\rangle=0$. One divergence representation is $\operatorname{tr}A^3=\partial_i[u_j(\partial_j u_k)(\partial_k u_i)-u_i\operatorname{tr}A^2/2]$. Splitting the [velocity gradient tensor](fluid-mechanics.md#velocity-gradient-tensor) into strain and rotation gives $\langle\omega_i\omega_jS_{ij}\rangle=-4\langle abc\rangle$. It connects mean [vortex stretching](physics.md#vortex-stretching) to the cubic strain statistic, without requiring isotropy.

### Isotropic turbulence

↑ **Parent:** [Homogeneous turbulence](#homogeneous-turbulence)

[Isotropic turbulence](#isotropic-turbulence) has statistics invariant under rotations as well as translations. With no mean velocity, its two-point [velocity correlation tensor](#velocity-correlation-tensor) depends on separation length and on longitudinal/transverse directions, and its one-component velocity [variances](variance.md) are equal.

#### Local isotropy of turbulence

↑ **Parent:** [Isotropic turbulence](#isotropic-turbulence)

Small-scale joint [velocity increment](#velocity-increment) statistics become approximately invariant under [rotations](riemannian-geometry.md#rotation-mathematics) of the observation configuration, even when the energy-containing flow is anisotropic. This is a scale-restricted hypothesis; it does not make the entire [velocity field](fluid-mechanics.md#velocity-field) isotropic or remove [internal intermittency](#internal-intermittency).

#### Loitsyansky integral

↑ **Parent:** [Isotropic turbulence](#isotropic-turbulence)

The Loitsyansky integral is the second spatial moment of the trace [velocity correlation tensor](#velocity-correlation-tensor), with the displayed sign convention. If correlations decay sufficiently rapidly, it is the coefficient of $k^4/(24\pi^2)$ in the [turbulent energy spectrum](#turbulent-energy-spectrum). In terms of the normalized [longitudinal velocity correlation](#longitudinal-velocity-correlation) it is $8\pi u^2\int_0^\infty r^4f(r)dr$ when the boundary terms vanish; conventions omitting $8\pi$ also occur. Its evolution is $\dot I=8\pi[r^4u^3K]_\infty-12\nu L$, where $L$ is the [Saffman integral](#saffman-integral). Thus it is invariant when $L=0$ and the longitudinal triple correlation is $o(r^{-4})$, not under arbitrary turbulent conditions.

##### Landau angular-momentum argument for turbulent decay

↑ **Parent:** [Loitsyansky integral](#loitsyansky-integral)

For a confined [incompressible flow](fluid-mechanics.md#incompressible-flow) with no velocity flux across the boundary, an integrated divergence identity gives $\langle|\int\boldsymbol x\times\boldsymbol u\,dV|^2\rangle=-\iint r^2\langle\boldsymbol u\cdot\boldsymbol u'\rangle dVdV'$. In a large approximately homogeneous region with short correlations, the latter is approximately $VI$. [Conservation of angular momentum](classical-mechanics.md#conservation-of-angular-momentum) in an isolated torque-free cloud then motivates conservation of the [Loitsyansky integral](#loitsyansky-integral). A fixed subvolume of infinite turbulence is not an isolated cloud: advective transport, pressure torques, wall stresses and long-range correlations can invalidate the argument.

##### Kolmogorov decay law

↑ **Parent:** [Loitsyansky integral](#loitsyansky-integral)

Assume a nonzero invariant [Loitsyansky integral](#loitsyansky-integral), self-preserving large-scale correlations, and high-[Reynolds number](fluid-mechanics.md#reynolds-number) freely decaying [isotropic turbulence](#isotropic-turbulence). Then $I\propto u^2\ell^5$ and $-d(u^2)/dt\propto u^3/\ell$ imply the displayed decay and growth laws. The assumptions on correlation shape and the dissipation coefficient are needed in addition to conservation of the integral.

#### Saffman integral

↑ **Parent:** [Isotropic turbulence](#isotropic-turbulence)

The [Saffman integral](#saffman-integral) is $L=\int\langle\mathbf u(\mathbf x)\cdot\mathbf u(\mathbf x+\mathbf r)\rangle\,d^3r$. With integrable trace correlation it equals the large-volume limit of $\langle|\int_V\mathbf u\,dV|^2\rangle/|V|$. It is nonnegative and measures [momentum](classical-mechanics.md#momentum)-fluctuation density. Under appropriate unforced far-field flux conditions it is invariant.

##### Saffman decay law

↑ **Parent:** [Saffman integral](#saffman-integral)

With nonzero invariant $L$, a self-preserving [integral scale of turbulence](#integral-scale-of-turbulence) gives $L\propto\mathcal E\ell^3$. Combining this with freely decaying high-Reynolds-number [viscous dissipation](stokes-flow.md#viscous-dissipation) $\epsilon\propto\mathcal E^{3/2}/\ell$ gives $\mathcal E\propto(t-t_*)^{-6/5}$ and $\ell\propto(t-t_*)^{2/5}$. The closure assumptions, not the invariant alone, determine this exponent.

##### Small-wavenumber spectrum with nonzero Saffman integral

↑ **Parent:** [Saffman integral](#saffman-integral)

A finite nonzero [Saffman integral](#saffman-integral) gives $E(k)=Lk^2/(4\pi^2)+o(k^2)$ in the standard isotropic spectrum normalization. This follows by expanding the radial spectral transform at small wavenumber. A further analytic term requires additional correlation [moments](probability-theory.md#moment).

#### Velocity correlation tensor

↑ **Parent:** [Isotropic turbulence](#isotropic-turbulence)

The [velocity correlation tensor](#velocity-correlation-tensor) is $Q_{ij}(\mathbf r)=\langle u_i(\mathbf x)u_j(\mathbf x+\mathbf r)\rangle$. For [isotropic turbulence](#isotropic-turbulence) it splits into longitudinal and transverse parts. Incompressibility constrains them, while the [Fourier transform](analysis.md#fourier-transform) gives the [turbulent energy spectrum](#turbulent-energy-spectrum). Its trace is the scalar velocity-dot-product correlation.

<h5 id="karman-howarth-equation">Kármán-Howarth equation</h5>

↑ **Parent:** [Velocity correlation tensor](#velocity-correlation-tensor)

The [Kármán-Howarth equation](#karman-howarth-equation) evolves two-point correlations in homogeneous [isotropic turbulence](#isotropic-turbulence). In trace form it is $\partial_tC=r^{-2}\partial_r[r^{-1}\partial_r(r^4u^3K)]+2\nu r^{-2}\partial_r(r^2C\prime)$. Integrating with radial volume weight reduces conservation of the [Saffman integral](#saffman-integral) to vanishing nonlinear and viscous boundary fluxes.

###### Kolmogorov equation for structure functions

↑ **Parent:** [Kármán-Howarth equation](#karman-howarth-equation)

For unforced [homogeneous turbulence](#homogeneous-turbulence) with [isotropic turbulence](#isotropic-turbulence) statistics, put $F=u^2f=u^2-S_2/2$ and $S_3=6u^3K$. The longitudinal [Kármán-Howarth equation](#karman-howarth-equation) is $F_t=r^{-4}\partial_r[r^4(S_3/6-\nu S_2')]$. Since $\partial_tu^2=-2\epsilon/3$, regularity at zero gives

$$
S_3-6\nu S_2'=-\frac45\epsilon r-\frac3{r^4}\int_0^r s^4\partial_tS_2(s,t)\,ds.
$$

Neglecting the last term in a locally equilibrated small-scale range gives the displayed equation. The [Kolmogorov four-fifths law](#kolmogorov-four-fifths-law) follows where the viscous term is negligible as well.

###### Kolmogorov four-fifths law

↑ **Parent:** [Kolmogorov equation for structure functions](#kolmogorov-equation-for-structure-functions)

The signed third-order [longitudinal structure function](#longitudinal-velocity-structure-function) has this leading [inertial range](#inertial-range) form under homogeneity, isotropy and the usual local-equilibrium scale separation. Its coefficient follows from the [Kármán-Howarth equation](#karman-howarth-equation) and the mean [kinetic energy](classical-mechanics.md#kinetic-energy) budget, without assuming the [Kolmogorov two-thirds law](#kolmogorov-two-thirds-law). Its negative sign encodes a forward [energy cascade](#energy-cascade); it does not establish every higher-order similarity exponent.

##### Longitudinal velocity correlation

↑ **Parent:** [Velocity correlation tensor](#velocity-correlation-tensor)

For a separation parallel to a unit vector $\mathbf n$, the [longitudinal velocity correlation](#longitudinal-velocity-correlation) is $Q_{LL}=\langle u_L(\mathbf x)u_L(\mathbf x+r\mathbf n)\rangle=u^2f(r)$. In isotropic incompressible [turbulence](turbulence.md) the transverse normalized correlation is $g=f+rf\prime/2$ and the trace is $C=u^2(3f+rf\prime)$.

###### Longitudinal velocity structure function

↑ **Parent:** [Longitudinal velocity correlation](#longitudinal-velocity-correlation)

The order-$p$ [longitudinal velocity structure function](#longitudinal-velocity-structure-function) is $S_p(r)=\langle[u_L(\mathbf x+r\mathbf n)-u_L(\mathbf x)]^p\rangle$; absolute increments are used for noninteger orders. At second order $S_2=2u^2[1-f(r)]$. It suppresses a smooth common velocity but does not exactly remove all contributions from motions larger than the separation.

###### Velocity increment

↑ **Parent:** [Longitudinal velocity structure function](#longitudinal-velocity-structure-function)

A velocity increment is the difference of a [velocity field](fluid-mechanics.md#velocity-field) between two positions. Its longitudinal component is the projection onto their separation direction. Moments of increments define [longitudinal structure functions](#longitudinal-velocity-structure-function); the [Kolmogorov 1941 theory](#kolmogorov-1941-theory) estimates a typical inertial-range magnitude as $(\epsilon r)^{1/3}$.

###### Large-scale contributions to structure functions

↑ **Parent:** [Longitudinal velocity structure function](#longitudinal-velocity-structure-function)

A smooth velocity varying on a scale larger than $r$ contributes $\Delta U_L\simeq r\partial_LU_L$ to a velocity increment. Higher powers produce mixed [moments](probability-theory.md#moment) with smaller-scale increments. [longitudinal structure functions](#longitudinal-velocity-structure-function) therefore attenuate, but do not exactly filter out, large-scale strain and intensity modulation.

###### Structure-function spectral filter

↑ **Parent:** [Longitudinal velocity structure function](#longitudinal-velocity-structure-function)

In isotropic incompressible three-dimensional [turbulence](turbulence.md), $3S_2(r)/4=\int E(k)H(kr)\,dk$, with $H(x)=1+3\cos x/x^2-3\sin x/x^3$. It is smooth at zero, where $H=x^2/10+O(x^4)$, and tends to one at large argument. A sharp wavenumber cutoff omits the finite large-scale-gradient contribution.

#### Turbulent energy spectrum

↑ **Parent:** [Isotropic turbulence](#isotropic-turbulence)

The [turbulent energy spectrum](#turbulent-energy-spectrum) $E(k)$ distributes [kinetic energy](classical-mechanics.md#kinetic-energy) over wavenumber shells, normalized by $\int_0^\infty E(k)\,dk=\langle|\mathbf u|^2\rangle/2$. For isotropic [incompressible flow](fluid-mechanics.md#incompressible-flow) its tensor form is $\Phi_{ij}=E(k)(\delta_{ij}-k_ik_j/k^2)/(4\pi k^2)$. Its low-wavenumber behavior records large-eddy [momentum](classical-mechanics.md#momentum) statistics.

#### Longitudinal velocity-gradient skewness

↑ **Parent:** [Isotropic turbulence](#isotropic-turbulence)

For isotropic [incompressible flow](fluid-mechanics.md#incompressible-flow), directional averaging gives $\langle(\partial_xu_x)^3\rangle=(8/105)\langle\operatorname{tr}S^3\rangle=-(2/35)\langle\omega_i\omega_jS_{ij}\rangle$. Positive mean [vortex stretching](physics.md#vortex-stretching) therefore implies negative longitudinal derivative [skewness](probability-theory.md#skewness). [Statistical homogeneity](probability-and-statistics.md#statistical-homogeneity) alone does not determine the sign in a fixed direction.

## Eddy diffusion

↑ **Parent:** [Turbulence](turbulence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eddy_diffusion)

Mixing by [turbulence](turbulence.md) is represented approximately by a diffusive flux down a mean concentration gradient. Its coefficient is the [eddy diffusivity](#eddy-diffusivity). A constant-coefficient model gives a $D\nabla^2\sigma$ term and a smoothing rate $Dk^2$ for a [Fourier mode](fourier-analysis.md#fourier-mode). Effective diffusion can suppress slow gravitational concentration even when microscopic diffusion is negligible.

### Buoyancy-driven turbulent density diffusion

↑ **Parent:** [Eddy diffusion](#eddy-diffusion)

In a narrow tube with unstable mean density gradient $q=\partial_z\bar\rho>0$, width-limited turbulent eddies have velocity scale $u_*\sim W\sqrt{gq/\rho_0}$. A mixing-length diffusivity gives downward density flux $F_\rho=KW^2\sqrt{g/\rho_0}\,q^{3/2}$ per unit area. With upward coordinate $z$, conservation is $\bar\rho_t=\partial_zF_\rho$ and $q_t=KW^2\sqrt{g/\rho_0}\,\partial_z^2(q^{3/2})$. The closure presupposes established high-[Reynolds number](fluid-mechanics.md#reynolds-number) turbulence and requires boundary fluxes and finite available potential energy to be respected.

#### Quintic density-profile similarity in an unstable tube

↑ **Parent:** [Buoyancy-driven turbulent density diffusion](#buoyancy-driven-turbulent-density-diffusion)

Ignoring end boundaries, the [buoyancy-driven turbulent density diffusion](#buoyancy-driven-turbulent-density-diffusion) model admits $\bar\rho=\rho_0[1+A(t)Cz^5]$ for $C>0$. Since $(\partial_z\bar\rho)^{3/2}\propto A^{3/2}z^6$, the amplitude obeys $A'=6\,5^{3/2}KW^2\sqrt{gC}\,A^{3/2}$. With $A(0)=1$, $A=(1-t/t_*)^{-2}$ and $t_*=[3\,5^{3/2}KW^2\sqrt{gC}]^{-1}$. Its formal growth is not a physical finite-time singularity of a closed mixing tube: ignored end fluxes, loss of the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) and the finite energy budget invalidate the continuation.

### Density-variance dissipation rate

↑ **Parent:** [Eddy diffusion](#eddy-diffusion)

Molecular scalar diffusion removes density-fluctuation variance at the positive rate displayed here. With this convention the budget for one half of the variance has dissipation term $-\chi$; the full variance budget has $-2\chi$. In a stationary locally homogeneous shear flow the half-variance budget gives $\overline{\rho'w'}\,\overline\rho_z+\chi=0$. An integral-scale model writes $\chi=\overline{\rho'^2}q/L_\rho$, absorbing any normalization constant into $L_\rho$.

### Turbulent Prandtl number

↑ **Parent:** [Eddy diffusion](#eddy-diffusion)

The ratio of turbulent momentum diffusivity to buoyancy or heat diffusivity. Their ratio determines how the [gradient Richardson number](gravity-wave.md#gradient-richardson-number) is related to the energy-budget [Flux Richardson number](gravity-wave.md#flux-richardson-number). It is generally a closure-dependent function of the flow, not necessarily one.

#### Reynolds analogy

↑ **Parent:** [Turbulent Prandtl number](#turbulent-prandtl-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reynolds_analogy)

An ideal correspondence between turbulent momentum and scalar transfer. In the local gradient-diffusion form used for a surface layer, the ideal analogy sets $\mathrm{Pr}_t=1$. It is an additional modeling approximation; measured buoyancy and momentum similarity functions need not be identical.

### Vertical turbulent buoyancy flux

↑ **Parent:** [Eddy diffusion](#eddy-diffusion)

The covariance of vertical velocity and buoyancy fluctuations has dimensions length squared per time cubed. It supplies buoyancy production in the [local turbulent kinetic energy balance](#local-turbulent-kinetic-energy-balance). This local flux density differs dimensionally from the section-integrated [buoyancy flux](turbulent-plume.md#buoyancy-flux) of a plume, which includes an area or width integration.

### Buoyancy-gradient mixing-length closure

↑ **Parent:** [Eddy diffusion](#eddy-diffusion)

For positive dense-fluid [reduced gravity](reduced-gravity.md) $G$ and upward coordinate $z$, an unstable gradient $G_z>0$ supplies buoyant work of order $d^2G_z$ over mixing length $d$. [velocity](classical-mechanics.md#velocity) $u\sim d\sqrt{G_z}$ and [eddy diffusivity](#eddy-diffusivity) $K\sim ud$ follow. Order-one constants depend on the [turbulence](turbulence.md) model. This closure is for an unstable gradient; its square root must not be applied to a stable negative gradient.

#### Arrested cubic buoyancy profile

↑ **Parent:** [Buoyancy-gradient mixing-length closure](#buoyancy-gradient-mixing-length-closure)

An upward [volume flux](fluid-mechanics.md#volumetric-flow-rate) $Q$ and a downward turbulent buoyancy transport $d^4(G_z)^{3/2}$ balance in a steady reactor. Matching $G=G_z=0$ below $-H$ gives $QG=d^4(G_z)^{3/2}$. Integrating yields the cubic profile above the front. If downward source [buoyancy flux](turbulent-plume.md#buoyancy-flux) is $B_s$, then $H=3d^{8/3}B_s^{1/3}/Q$. The corresponding [eddy diffusivity](#eddy-diffusivity) is $K=Q(z+H)/(3d^2)$. All these prefactors use the same area and mixing-length normalization; an actual cross-sectional area $S$ replaces the denominator in $K$ by $3S$.

#### Flux convergence in turbulent buoyancy mixing

↑ **Parent:** [Buoyancy-gradient mixing-length closure](#buoyancy-gradient-mixing-length-closure)

In the area normalization $d^2$, the [buoyancy-gradient mixing-length closure](#buoyancy-gradient-mixing-length-closure) transports dense-fluid buoyancy downward with magnitude $\mathcal F=d^2KG_z=d^4(G_z)^{3/2}$. Its convergence in an upward coordinate is $\mathcal F_z$. Transport has units $L^4T^{-3}$ and convergence units $L^3T^{-3}$. Constant positive $G_z$ has nonzero transport and zero convergence; the two quantities cannot be identified.

## Eddy diffusivity

↑ **Parent:** [Turbulence](turbulence.md)

An eddy diffusivity is a transport closure representing unresolved [turbulence](turbulence.md) by a mean scalar flux proportional to a negative mean [concentration](physics.md#concentration) gradient. A local estimate is $K\sim U\ell$, where $U$ and $\ell$ are turbulent speed and length scales. In a [line plume](turbulent-plume.md#line-plume) with constant characteristic speed and width proportional to $z$, this gives $K\propto z$. Its coefficient is an independent closure parameter; [fluid entrainment](fluid-mechanics.md#fluid-entrainment) conservation alone does not determine it.

### Turbulent Schmidt number

↑ **Parent:** [Eddy diffusivity](#eddy-diffusivity)

The ratio of turbulent momentum diffusivity to turbulent scalar diffusivity. It need not equal the analogous molecular diffusivity ratio, and it is unrelated to the Schmidt number used for quantum entanglement. For $\kappa_T=\nu_T/2$ its value is two.

## Turbulent round jet

↑ **Parent:** [Turbulence](turbulence.md)

A circular [turbulent round jet](#turbulent-round-jet) supplied with kinematic [momentum flux](physics.md#momentum-flux) $m_0$ but negligible [buoyancy flux](turbulent-plume.md#buoyancy-flux) conserves $m=m_0$. A [top-hat plume model](turbulent-plume.md#top-hat-plume-model) and constant [Batchelor entrainment](turbulent-plume.md#batchelor-entrainment-hypothesis) give $dq/ds=2\alpha\sqrt{\pi m_0}$. From a point source with zero [volume flux](fluid-mechanics.md#volumetric-flow-rate), $q=2\alpha\sqrt{\pi m_0}s$, radius $b=2\alpha s$, and axial [velocity](classical-mechanics.md#velocity) $V=m_0/q\propto s^{-1}$.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (33)

- [Buoyancy-gradient mixing-length closure](#buoyancy-gradient-mixing-length-closure)
- [Eddy diffusion](#eddy-diffusion)
- [Eddy diffusivity](#eddy-diffusivity)
- [Entropy mode](astrophysical-fluid-dynamics.md#entropy-mode)
- [Internal-wave breaking](gravity-wave.md#internal-wave-breaking)
- [Longitudinal velocity correlation](#longitudinal-velocity-correlation)
- [Mean enstrophy balance](fluid-mechanics.md#mean-enstrophy-balance)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-38.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-76.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-79.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-90.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73.md#4/vii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-79.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-79.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-65.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73.md#3/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-57.md#2/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-74.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345.md#2/a/solution)
- [Structure-function spectral filter](#structure-function-spectral-filter)
- [Turbulent mixing of a secularly unstable dust layer](gravitational-instability-of-an-astrophysical-disk.md#turbulent-mixing-of-a-secularly-unstable-dust-layer)
- [Zeroth law of turbulence](#zeroth-law-of-turbulence)
