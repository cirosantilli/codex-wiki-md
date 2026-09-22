# Cosmic microwave background anisotropy

↑ **Parent:** [Cosmic microwave background](cosmology.md#cosmic-microwave-background)

Cosmic microwave background anisotropies are direction-dependent perturbations of the relic radiation temperature and polarization.

**Table of contents**

- [Finite-width last-scattering damping](#finite-width-last-scattering-damping)
- [Reduced CMB bispectrum](#reduced-cmb-bispectrum)
  - [Full-sky cubic bispectrum estimator](#full-sky-cubic-bispectrum-estimator)
    - [Monopole cancellation of internal cubic-estimator contractions](#monopole-cancellation-of-internal-cubic-estimator-contractions)
  - [Primordial-to-angular bispectrum projection](#primordial-to-angular-bispectrum-projection)
  - [Sachs-Wolfe projection of a constant bispectrum](#sachs-wolfe-projection-of-a-constant-bispectrum)
- [CMB lensing potential](#cmb-lensing-potential)
- [Cosmic microwave background power spectrum](#cosmic-microwave-background-power-spectrum)
  - [Sachs-Wolfe plateau](#sachs-wolfe-plateau)
  - [Cosmic variance](#cosmic-variance)
- [Cosmic microwave background polarization](#cosmic-microwave-background-polarization)
  - [B-mode polarization](#b-mode-polarization)
  - [E-mode polarization](#e-mode-polarization)
    - [Scalar E-mode radial projection](#scalar-e-mode-radial-projection)
    - [Low-multipole kernel of polarization potentials](#low-multipole-kernel-of-polarization-potentials)
- [Photon temperature multipole](#photon-temperature-multipole)
  - [Photon multipole normalization change](#photon-multipole-normalization-change)
  - [Photon angular temperature moments](#photon-angular-temperature-moments)
    - [Photon temperature perturbation](#photon-temperature-perturbation)
  - [Photon monopole](#photon-monopole)
    - [Sachs-Wolfe combination](#sachs-wolfe-combination)
      - [Sachs-Wolfe radiation-to-matter matching](#sachs-wolfe-radiation-to-matter-matching)
      - [Sachs-Wolfe effect](#sachs-wolfe-effect)
      - [Doppler CMB anisotropy](#doppler-cmb-anisotropy)
      - [Integrated Sachs-Wolfe effect](#integrated-sachs-wolfe-effect)
        - [Rees-Sciama effect](#rees-sciama-effect)
  - [Photon dipole](#photon-dipole)
  - [Photon quadrupole](#photon-quadrupole)
- [Photon-baryon fluid](#photon-baryon-fluid)
  - [Baryon Euler equation with Thomson drag](#baryon-euler-equation-with-thomson-drag)
  - [Baryon loading parameter](#baryon-loading-parameter)
  - [Thomson scattering](#thomson-scattering)
  - [Tight-coupling approximation](#tight-coupling-approximation)
    - [Photon opacity normalization for a velocity potential](#photon-opacity-normalization-for-a-velocity-potential)
    - [Temperature-only tight-coupling quadrupole](#temperature-only-tight-coupling-quadrupole)
    - [Photon-baryon acoustic oscillator](#photon-baryon-acoustic-oscillator)
      - [Coherent initial phases are needed for acoustic variance peaks](#coherent-initial-phases-are-needed-for-acoustic-variance-peaks)
    - [Photon-baryon sound speed](#photon-baryon-sound-speed)
    - [Photon-baryon velocity slip](#photon-baryon-velocity-slip)
    - [Photon quadrupole in tight coupling with polarization](#photon-quadrupole-in-tight-coupling-with-polarization)
    - [Photon-baryon diffusion damping equation](#photon-baryon-diffusion-damping-equation)
      - [Shear-only photon diffusion damping](#shear-only-photon-diffusion-damping)
        - [Slowly varying shear-damped photon oscillator](#slowly-varying-shear-damped-photon-oscillator)
  - [Sound horizon](#sound-horizon)
    - [Sound-horizon angle in an open matter universe](#sound-horizon-angle-in-an-open-matter-universe)
  - [Cosmic microwave background diffusion damping](#cosmic-microwave-background-diffusion-damping)
- [Adiabatic initial conditions](#adiabatic-initial-conditions)
  - [Adiabatic matter-string density relation](#adiabatic-matter-string-density-relation)
- [Cosmic microwave background acoustic peak](#cosmic-microwave-background-acoustic-peak)
  - [Angular projection of density and Doppler acoustic sources](#angular-projection-of-density-and-doppler-acoustic-sources)
  - [Adiabatic acoustic-peak spacing](#adiabatic-acoustic-peak-spacing)
- [Free-streaming photon Boltzmann equation](#free-streaming-photon-boltzmann-equation)
  - [Photon brightness perturbation](#photon-brightness-perturbation)
    - [Synchronous photon brightness equation](#synchronous-photon-brightness-equation)
      - [Photon brightness equation for a negative spatial perturbation](#photon-brightness-equation-for-a-negative-spatial-perturbation)
      - [Synchronous photon momentum redshift](#synchronous-photon-momentum-redshift)
  - [Photon Boltzmann hierarchy](#photon-boltzmann-hierarchy)
    - [Vector photon Boltzmann hierarchy](#vector-photon-boltzmann-hierarchy)
    - [Photon continuity equation](#photon-continuity-equation)
    - [Photon Euler equation](#photon-euler-equation)
  - [Line-of-sight solution for free-streaming photons](#line-of-sight-solution-for-free-streaming-photons)
    - [Matter-era photon endpoint solution](#matter-era-photon-endpoint-solution)
    - [Synchronous Sachs-Wolfe line-of-sight formula](#synchronous-sachs-wolfe-line-of-sight-formula)
      - [Endpoint terms in the synchronous Sachs-Wolfe formula](#endpoint-terms-in-the-synchronous-sachs-wolfe-formula)
  - [Photon Boltzmann equation with Thomson scattering](#photon-boltzmann-equation-with-thomson-scattering)
    - [Cosmological optical depth](#cosmological-optical-depth)
      - [Cosmological visibility function](#cosmological-visibility-function)
        - [Cosmic microwave background line-of-sight solution](#cosmic-microwave-background-line-of-sight-solution)
          - [Tensor CMB line-of-sight source](#tensor-cmb-line-of-sight-source)

## Finite-width last-scattering damping

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

A finite visibility width averages photon sources over emission time and radial position. For a Gaussian visibility profile, a plane-wave radial phase has the displayed damping factor; its power has the square of this amplitude factor. An acoustic source also varies with frequency $kc_s$, so its rapid oscillations are averaged. This averaging is distinct from [Silk damping](#cosmic-microwave-background-diffusion-damping), which smooths the perturbations by photon diffusion before decoupling. Angular projection and source evolution prevent a universal isotropic damping coefficient based only on radial width.

## Reduced CMB bispectrum

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

A statistically isotropic [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md) has $\langle a_{\ell_1m_1}a_{\ell_2m_2}a_{\ell_3m_3}\rangle=\mathcal G^{\ell_1\ell_2\ell_3}_{m_1m_2m_3}b_{\ell_1\ell_2\ell_3}$, where $\mathcal G$ is the integral of the three [spherical harmonics](analysis.md#spherical-harmonic). The reduced CMB bispectrum removes this angular geometric factor and retains the primordial and transfer-function dependence. A [Sachs-Wolfe projection of a constant bispectrum](#sachs-wolfe-projection-of-a-constant-bispectrum) is an analytic large-angle example.

### Full-sky cubic bispectrum estimator

↑ **Parent:** [Reduced CMB bispectrum](#reduced-cmb-bispectrum)

For an isotropic, full-sky temperature map with a fixed bispectrum template $b=f_{\mathrm{NL}}b^1$, the inverse-variance-weighted cubic statistic has normalization $F=\frac16\sum (b^1)^2\mathcal G^2/(C_1C_2C_3)$ over ordered triples. It is unbiased under the linear template relation and has Gaussian [cosmic variance](#cosmic-variance) $1/F$. The factor $1/6$ counts the six cross-triple [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction). A removed monopole cancels the nine internal-pairing terms; incomplete sky coverage or anisotropic noise generally require a linear correction.

#### Monopole cancellation of internal cubic-estimator contractions

↑ **Parent:** [Full-sky cubic bispectrum estimator](#full-sky-cubic-bispectrum-estimator)

In a [full-sky cubic bispectrum estimator](#full-sky-cubic-bispectrum-estimator), pairwise Gaussian covariance within one triple gives a sum of [Gaunt integrals](analysis.md#gaunt-integral) with opposite $m$ indices. The [spherical harmonic addition theorem](analysis.md#spherical-harmonic-addition-theorem) turns their pair into the constant $(2\ell+1)/(4\pi)$; its integral against $Y_{LM}$ vanishes for $L>0$. A zero temperature monopole removes $L=0$. Thus only the six pairings connecting the two triples survive in the Gaussian variance; isotropic weights are essential for the cancellation.

### Primordial-to-angular bispectrum projection

↑ **Parent:** [Reduced CMB bispectrum](#reduced-cmb-bispectrum)

Linear cosmological transfer maps the [primordial bispectrum](cosmology.md#primordial-bispectrum) to the [reduced CMB bispectrum](#reduced-cmb-bispectrum). A Fourier representation of the momentum delta function and three [Rayleigh plane-wave expansions](analysis.md#rayleigh-plane-wave-expansion) separate the radial transfer integrals from a [Gaunt integral](analysis.md#gaunt-integral). The six angular factors and three Fourier measures give $(4\pi)^6/(2\pi)^9=(2/\pi)^3$. The observer-position phase cancels by momentum conservation; the remaining radial position is an auxiliary integration variable.

### Sachs-Wolfe projection of a constant bispectrum

↑ **Parent:** [Reduced CMB bispectrum](#reduced-cmb-bispectrum)

For a [constant primordial bispectrum](cosmology.md#constant-primordial-bispectrum) and large-angle transfer function $\Delta_\ell(k)=j_\ell(kR)/5$, the [spherical Bessel product integral](analysis.md#spherical-bessel-product-integral) reduces the radial projection to $\int_0^1r^{L+2}\,dr+\int_1^\infty r^{-L-1}\,dr$. For $L>0$ this equals $1/(L+3)+1/L$, giving the displayed [reduced CMB bispectrum](#reduced-cmb-bispectrum). All powers of the distance $R$ cancel. Under common large-multipole scaling it behaves as $\ell^{-4}$ at fixed shape; this is angular scale invariance, not a constant angular bispectrum. The all-monopole case $L=0$ has a logarithmically divergent radial tail and is excluded.

## CMB lensing potential

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

The CMB lensing potential is the line-of-sight projection of gravitational potential that remaps observed CMB directions by the deflection angle $\nabla\psi$.

## Cosmic microwave background power spectrum

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

The CMB angular power spectrum decomposes the variance of temperature or polarization anisotropy by angular multipole. Its large-angle plateau and acoustic peaks encode primordial perturbations and photon-baryon evolution.

### Sachs-Wolfe plateau

↑ **Parent:** [Cosmic microwave background power spectrum](#cosmic-microwave-background-power-spectrum)

For a scale-invariant potential spectrum with $\mathcal A_\Phi=k^3P_\Phi/(2\pi^2)$ constant, the matter-era [Sachs-Wolfe effect](#sachs-wolfe-effect) gives $C_\ell=(4\pi\mathcal A_\Phi/9)\int j_\ell(x)^2dx/x$. The [logarithmic spherical Bessel square integral](analysis.md#logarithmic-spherical-bessel-square-integral) then gives $\ell(\ell+1)C_\ell=2\pi\mathcal A_\Phi/9$. This plateau applies to large-angle temperature anisotropies, neglecting acoustic evolution and late evolving potentials; it is not a constant $C_\ell$ spectrum.

### Cosmic variance

↑ **Parent:** [Cosmic microwave background power spectrum](#cosmic-microwave-background-power-spectrum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cosmic_variance)

Cosmic variance is the sampling uncertainty caused by observing only one realization of a cosmological random field. For a Gaussian isotropic full-sky temperature field and an ideal noiseless estimate, $\operatorname{Var}(\widehat C_\ell)=2C_\ell^2/(2\ell+1)$ because there are only $2\ell+1$ independent real angular degrees of freedom.

## Cosmic microwave background polarization

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cosmic_microwave_background_polarization)

Thomson scattering of a local radiation quadrupole generates linear cosmic microwave background polarization. Its acoustic phase follows the photon velocity and is shifted by one quarter-period relative to the monopole temperature oscillation.

### B-mode polarization

↑ **Parent:** [Cosmic microwave background polarization](#cosmic-microwave-background-polarization)

The parity-odd part of linear sky polarization is represented by the pseudoscalar potential $P_B$. At linear order an axisymmetric [scalar cosmological perturbation](linear-cosmological-perturbation-theory.md#scalar-cosmological-perturbation) gives no physical B mode. Tensor or vector sources and lensing conversion of [E-mode polarization](#e-mode-polarization) are outside that scalar-source statement.

### E-mode polarization

↑ **Parent:** [Cosmic microwave background polarization](#cosmic-microwave-background-polarization)

The parity-even part of linear sky polarization can be represented by a scalar potential $P_E$ through $Q\pm iU=\eth_{\pm}^2(P_E\pm iP_B)$. It is naturally separated from [B-mode polarization](#b-mode-polarization) by the parity of its spherical multipoles. Linear [scalar cosmological perturbations](linear-cosmological-perturbation-theory.md#scalar-cosmological-perturbation) generate E modes; the potential has an unobservable low-multipole kernel.

#### Scalar E-mode radial projection

↑ **Parent:** [E-mode polarization](#e-mode-polarization)

For a scalar [photon quadrupole](#photon-quadrupole) emitted at distance $\chi_*$, the meridian-basis source is $Q\pm iU\propto\Theta_2e^{-ik\chi_*\mu}(1-\mu^2)$. Integrating its scalar-potential equation and removing the [low-multipole kernel of polarization potentials](#low-multipole-kernel-of-polarization-potentials) yields $P_E\propto\sum_{\ell\ge2}(-i)^\ell(2\ell+1)\Theta_2j_\ell(k\chi_*)P_\ell(\mu)/(k\chi_*)^2$, with no scalar $P_B$. The apparent $k^{-2}$ divergence lies in discarded low multipoles; $j_\ell(x)=O(x^\ell)$ makes the physical small-$x$ limit regular.

#### Low-multipole kernel of polarization potentials

↑ **Parent:** [E-mode polarization](#e-mode-polarization)

Twice-applied spin-raising or lowering annihilates the ordinary spherical-harmonic multipoles $\ell=0,1$. Polarization potentials therefore have a four-dimensional monopole/dipole ambiguity on the sphere. For an axisymmetric mode it is $A+B\cos\theta$. Setting these components to zero defines the observable $\ell\ge2$ potentials without changing $Q$ or $U$.

## Photon temperature multipole

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

For Fourier wavevector $\mathbf k$ and photon direction $\widehat{\mathbf p}$, the temperature perturbation is expanded as

$$
\Theta(\mu)=\sum_{\ell=0}^{\infty}(-i)^\ell(2\ell+1)
\Theta_\ell P_\ell(\mu),
\qquad
\mu=\widehat{\mathbf k}\mathbin\cdot\widehat{\mathbf p}.
$$

### Photon multipole normalization change

↑ **Parent:** [Photon temperature multipole](#photon-temperature-multipole)

For a fixed angular order $m$, write $\Theta=\sum_\ell C_\ell q_\ell Y_{\ell m}$. Streaming by $ik\mu$ contributes $ik(C_{\ell+1}/C_\ell)a_{\ell+1,m}q_{\ell+1}+ik(C_{\ell-1}/C_\ell)a_{\ell,m}q_{\ell-1}$. Thus rescaling the expansion coefficients also rescales the hierarchy couplings and source amplitudes. Replacing $C_\ell=(-i)^\ell\sqrt{(2\ell+1)/(8\pi)}$ by $\widetilde C_\ell=(-i)^\ell\sqrt{2\pi/(2\ell+1)}$ requires $\widetilde q_\ell=(2\ell+1)q_\ell/(4\pi)$; the temperature field is unchanged. This prevents mixing incompatible [photon temperature multipole](#photon-temperature-multipole) conventions.

### Photon angular temperature moments

↑ **Parent:** [Photon temperature multipole](#photon-temperature-multipole)

Let $\langle F\rangle=(4\pi)^{-1}\int F\,d\Omega$ and $f=\bar f(\epsilon)-\epsilon\bar f'(\epsilon)\Theta(\mathbf e)$ with comoving energy $\epsilon=aE$. If $\epsilon^4\bar f$ vanishes at both integration endpoints, [integration by parts](calculus.md#integration-by-parts) gives $-\int\epsilon^4\bar f'\,d\epsilon=4\int\epsilon^3\bar f\,d\epsilon$. The [kinetic stress-energy tensor](statistical-physics.md#kinetic-stress-energy-tensor) then gives $\delta_\gamma=4\langle\Theta\rangle$, $v_\gamma^i=3\langle\Theta e^i\rangle$, $\delta P=\bar\rho\delta_\gamma/3$, and $\pi^{ij}=4\bar\rho\langle\Theta(e^ie^j-\delta^{ij}/3)\rangle$. If $\Pi=-\pi$ is used, the last expression changes sign. Frequency independence of $\Theta$ is essential to this common temperature description.

#### Photon temperature perturbation

↑ **Parent:** [Photon angular temperature moments](#photon-angular-temperature-moments)

A direction-dependent fractional photon temperature change. For a thermal spectrum, $f(\epsilon)=\bar f(\epsilon)-\Theta\epsilon\bar f'(\epsilon)$ is its linear expansion at fixed comoving energy. For a nonthermal spectrum the same ansatz is a brightness dilation, rather than necessarily a thermodynamic temperature. In unweighted [Legendre polynomial](differential-equation.md#legendre-polynomial) multipoles, $\Theta=\sum_\ell(-i)^\ell\Theta_\ell P_\ell$, the photon density, velocity and [anisotropic stress](general-relativity.md#anisotropic-stress) are $\delta_\gamma=4\Theta_0$, $v_\gamma=-\Theta_1$ and $\Pi_\gamma=-3\Theta_2/5$.

### Photon monopole

↑ **Parent:** [Photon temperature multipole](#photon-temperature-multipole)

The photon monopole is the direction-averaged fractional temperature perturbation. In Newtonian gauge its gravitationally observable effective temperature is the Sachs-Wolfe combination $\Theta_0+\Psi$.

#### Sachs-Wolfe combination

↑ **Parent:** [Photon monopole](#photon-monopole)

In Newtonian gauge, $\Theta_0+\Psi$ combines the intrinsic photon temperature perturbation with the gravitational redshift at emission. With constant potentials and negligible baryon loading it oscillates as $\cos(kr_s)$ for adiabatic initial conditions.

##### Sachs-Wolfe radiation-to-matter matching

↑ **Parent:** [Sachs-Wolfe combination](#sachs-wolfe-combination)

For a constant growing adiabatic mode with curvature convention $\mathcal R=-\phi-\mathcal H(\phi'+\mathcal H\phi)/[4\pi Ga^2(\bar\rho+\bar P)]$, $\phi_{\rm rad}=-2\mathcal R/3$ and $\phi_{\rm mat}=-3\mathcal R/5$. The superhorizon [photon continuity equation](#photon-continuity-equation) conserves $\Theta_0-\phi$. With radiation initial value $\Theta_0=\mathcal R/3$, it gives $\Theta_{0,\rm mat}=2\mathcal R/5$ and $(\Theta_0+\psi)_{\rm mat}=-\mathcal R/5$ when $\psi=\phi$.

##### Sachs-Wolfe effect

↑ **Parent:** [Sachs-Wolfe combination](#sachs-wolfe-combination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sachs-Wolfe_effect)

The Sachs-Wolfe effect is the large-angle CMB temperature anisotropy produced by intrinsic photon-temperature perturbations and gravitational redshift at last scattering. For an adiabatic mode during matter domination, $\Theta_0+\Psi=\Psi/3$ on superhorizon scales.

##### Doppler CMB anisotropy

↑ **Parent:** [Sachs-Wolfe combination](#sachs-wolfe-combination)

The Doppler CMB anisotropy is the line-of-sight velocity contribution from the last-scattering plasma. With the convention used here it contributes $-\widehat{\mathbf n}\mathbin\cdot\mathbf v_e$ to the observed fractional temperature perturbation.

##### Integrated Sachs-Wolfe effect

↑ **Parent:** [Sachs-Wolfe combination](#sachs-wolfe-combination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integrated_Sachs-Wolfe_effect)

The integrated Sachs-Wolfe effect is the CMB temperature shift produced when the gravitational potentials traversed by a photon evolve with time. Its line-of-sight source is proportional to $\Phi'+\Psi'$.

###### Rees-Sciama effect

↑ **Parent:** [Integrated Sachs-Wolfe effect](#integrated-sachs-wolfe-effect)

The [Rees-Sciama effect](#rees-sciama-effect) is the microwave temperature shift produced by time-dependent gravitational potentials in nonlinear structure. A photon gains energy entering a potential well and loses it leaving; the shifts do not cancel when the well changes during transit. To leading order in its effect on the photon spectrum, this is a frequency-independent thermodynamic temperature shift, unlike the [thermal Sunyaev-Zeldovich effect](cosmology.md#thermal-sunyaev-zeldovich-effect). A nonlinear potential can evolve even during matter domination, when linear growing-mode potentials are constant.

### Photon dipole

↑ **Parent:** [Photon temperature multipole](#photon-temperature-multipole)

The photon dipole represents the bulk velocity of the radiation. In tight coupling to baryons, $v_b=-3\Theta_1$ under the convention used here.

### Photon quadrupole

↑ **Parent:** [Photon temperature multipole](#photon-temperature-multipole)

The photon quadrupole is the leading anisotropy that sources linear polarization through Thomson scattering.

## Photon-baryon fluid

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

Before recombination, frequent Thomson scattering couples photons, electrons, and baryons into an acoustic fluid.

### Baryon Euler equation with Thomson drag

↑ **Parent:** [Photon-baryon fluid](#photon-baryon-fluid)

For the velocity convention $v_\gamma=-\Theta_1$ and $\dot\tau<0$, momentum-conserving [Thomson scattering](#thomson-scattering) gives $\dot v_b+\mathcal H v_b+k\psi=(\dot\tau/R)(v_b-v_\gamma)$. Here $R$ is the [baryon loading parameter](#baryon-loading-parameter). Its collision force is opposite to the photon force when both are weighted by their enthalpies.

### Baryon loading parameter

↑ **Parent:** [Photon-baryon fluid](#photon-baryon-fluid)

The inertia ratio of the [photon-baryon fluid](#photon-baryon-fluid) is $R=3\bar\rho_b/(4\bar\rho_\gamma)$. Photon momentum is weighted by the radiation enthalpy $4\bar\rho_\gamma/3$, so this ratio controls momentum exchange, the common sound speed and the offset of the acoustic oscillator. Background conservation gives $R\propto a$ and $\dot R=\mathcal H R$.

### Thomson scattering

↑ **Parent:** [Photon-baryon fluid](#photon-baryon-fluid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thomson_scattering)

Thomson scattering is the low-energy elastic scattering of electromagnetic radiation by a free charged particle. Before cosmological recombination, repeated photon-electron scattering couples photons to the baryon velocity and damps higher photon multipoles.

### Tight-coupling approximation

↑ **Parent:** [Photon-baryon fluid](#photon-baryon-fluid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tight-coupling_approximation)

The tight-coupling approximation expands the photon-baryon Boltzmann equations in powers of $k/\Gamma$ and $\mathcal H/\Gamma$, where $\Gamma$ is the Thomson scattering rate.

#### Photon opacity normalization for a velocity potential

↑ **Parent:** [Tight-coupling approximation](#tight-coupling-approximation)

With Fourier convention $\mathbf v=i\mathbf k\theta$, the velocity divergence is $-k^2\theta$. Thomson drag in the velocity equation is the conformal scattering rate $q=a n_e\sigma_T$ times the velocity difference. Taking its divergence and dividing the whole divergence equation by $-k^2$ leaves the same rate multiplying the difference of velocity potentials; an additional $k^{-2}$ is not retained. Weighting the photon Euler equation by $R=4\bar\rho_\gamma/(3\bar\rho_b)$ and adding the baryon equation cancels the drag. In tight coupling the remaining equation is $(1+R)\theta'+\mathcal H\theta+R(\delta_\gamma/4-\sigma_\gamma)=0$, with sound speed $R/[3(1+R)]$.

#### Temperature-only tight-coupling quadrupole

↑ **Parent:** [Tight-coupling approximation](#tight-coupling-approximation)

For $\Theta(\mu)=\sum_\ell(-i)^\ell\Theta_\ell P_\ell(\mu)$ and a Thomson collision operator omitting polarization feedback, the quadrupole relaxes with rate $(9/10)\Gamma_T$, where $\Gamma_T=-\tau'>0$. Balancing its leading streaming source gives $\Theta_2=20k\Theta_1/(27\Gamma_T)$. This differs from [photon quadrupole in tight coupling with polarization](#photon-quadrupole-in-tight-coupling-with-polarization); the two formulas expand different collision operators.

#### Photon-baryon acoustic oscillator

↑ **Parent:** [Tight-coupling approximation](#tight-coupling-approximation)

With $v_b=v_\gamma$ at leading order and $c_s^2=1/[3(1+R)]$, the [photon continuity equation](#photon-continuity-equation) and total Euler equation give $\ddot\delta_\gamma+\dot R\dot\delta_\gamma/(1+R)+k^2\delta_\gamma/[3(1+R)]=4\ddot\phi+4\dot R\dot\phi/(1+R)-4k^2\psi/3$. The [baryon loading parameter](#baryon-loading-parameter) changes inertia and shifts the gravitational equilibrium. The leading equations omit diffusion damping.

##### Coherent initial phases are needed for acoustic variance peaks

↑ **Parent:** [Photon-baryon acoustic oscillator](#photon-baryon-acoustic-oscillator)

A damped mode $\delta=e^{-k^2/k_D^2}(A\cos q+B\sin q)$ does not alone imply oscillations in its ensemble [power spectrum](probability-and-statistics.md#power-spectrum). Averaging its modulus squared gives the displayed formula. Equal independent initial variances, $P_A=P_B$ and $P_{AB}=0$, erase the oscillatory variance through $\cos^2q+\sin^2q=1$. A coherent initial phase, as supplied by a regular growing [adiabatic mode](linear-cosmological-perturbation-theory.md#adiabatic-mode), selects one common oscillator phase and retains acoustic peaks. Its leading density and velocity oscillations are a quarter-period apart, and angular projection also preserves their correlated contribution.

#### Photon-baryon sound speed

↑ **Parent:** [Tight-coupling approximation](#tight-coupling-approximation)

For baryon-loading ratio $R=3\rho_b/(4\rho_\gamma)$, the photon-baryon sound speed is $c_s^2=1/[3(1+R)]$.

#### Photon-baryon velocity slip

↑ **Parent:** [Tight-coupling approximation](#tight-coupling-approximation)

The velocity slip is the difference between the bulk velocities of photons and baryons. [Thomson scattering](#thomson-scattering) suppresses it at a rate $\Gamma(1+R^{-1})$, where $R=3\rho_b/(4\rho_\gamma)$ and $\Gamma=-\dot\tau>0$. Its first correction in the [tight-coupling approximation](#tight-coupling-approximation) produces heat-conduction damping of acoustic waves.

#### Photon quadrupole in tight coupling with polarization

↑ **Parent:** [Tight-coupling approximation](#tight-coupling-approximation)

For the expansion $\Theta(\mu)=\sum_\ell(-i)^\ell\Theta_\ell P_\ell(\mu)$ without a $(2\ell+1)$ factor, the leading polarization relation is $E_2=-\sqrt6\,\Theta_2/4$. The [photon Boltzmann hierarchy](#photon-boltzmann-hierarchy) then gives $\Theta_2=-8k\Theta_1/(9\dot\tau)$. This small [photon quadrupole](#photon-quadrupole) supplies the shear-viscosity part of [Silk damping](#cosmic-microwave-background-diffusion-damping).

#### Photon-baryon diffusion damping equation

↑ **Parent:** [Tight-coupling approximation](#tight-coupling-approximation)

When gravity and expansion can be neglected and $R$ is constant, the [photon monopole](#photon-monopole) satisfies

$$
\ddot\Theta_0+
\frac{k^2}{3(1+R)\Gamma}
\left(\frac{R^2}{1+R}+\frac{16}{15}\right)\dot\Theta_0+
\frac{k^2}{3(1+R)}\Theta_0=0.
$$

The first damping contribution comes from [photon-baryon velocity slip](#photon-baryon-velocity-slip); the second comes from the [photon quadrupole](#photon-quadrupole). This is a local form of [Silk damping](#cosmic-microwave-background-diffusion-damping).

##### Shear-only photon diffusion damping

↑ **Parent:** [Photon-baryon diffusion damping equation](#photon-baryon-diffusion-damping-equation)

For the simplified quadrupole equation $\sigma_\gamma'+4k^2\theta_\gamma/15=-\sigma_\gamma/\tau_c$, neglecting its time derivative and gravitational driving gives $\sigma_\gamma=-\tau_c\delta_\gamma'/5$. A radiation-dominated inertia then obeys $\delta_\gamma''+4\tau_ck^2\delta_\gamma'/15+k^2\delta_\gamma/3=0$. On slowly varying subhorizon scales the amplitude is damped by $\exp[-(2/15)k^2\int\tau_cd\tau]$. This coefficient belongs to that truncated collision model, rather than the polarization-inclusive [Silk damping](#cosmic-microwave-background-diffusion-damping) equation.

###### Slowly varying shear-damped photon oscillator

↑ **Parent:** [Shear-only photon diffusion damping](#shear-only-photon-diffusion-damping)

Removing the first derivative from the truncated photon diffusion equation gives the displayed transformed oscillator. Constant mean free time changes its oscillation frequency only at second order. For a slowly varying mean free time and subhorizon wavelengths, derivative corrections to the phase and prefactor are small; the leading solution is an acoustic sine/cosine multiplied by $\exp[-k^2/k_D^2]$, where $k_D^{-2}=2\int\tau_c d\tau/15$. Dropping the derivative correction requires slow variation as well as a small mean free time; it is not an exact solution for arbitrary time dependence.

### Sound horizon

↑ **Parent:** [Photon-baryon fluid](#photon-baryon-fluid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sound_horizon)

The comoving sound horizon is the distance traveled by an acoustic wave,

$$
r_s(\eta)=\int_0^\eta c_s(\eta')\,d\eta'.
$$

#### Sound-horizon angle in an open matter universe

↑ **Parent:** [Sound horizon](#sound-horizon)

For last scattering well inside [matter domination](linear-cosmological-density-perturbation.md#matter-domination), $c_s=c/\sqrt3$ gives physical sound radius $R_s=2ca_*^{3/2}/(\sqrt3H_0\sqrt{\Omega_m})$. Neglecting the early [conformal time](cosmology.md#conformal-time) in the observer distance, an open dust cosmology has transverse comoving last-scattering distance $r_*=2c/(H_0\Omega_m)$. Thus $\theta_s=R_s/(a_*r_*)=\sqrt{\Omega_m a_*/3}$ and $\ell\sim\pi/\theta_s$. Radiation, baryon sound-speed evolution and acoustic phase shifts refine this estimate.

// Target: cosmology.bigb

### Cosmic microwave background diffusion damping

↑ **Parent:** [Photon-baryon fluid](#photon-baryon-fluid)

Cosmic microwave background diffusion damping is the suppression of small-angular-scale anisotropy as photons random-walk out of overdense regions during the finite-width recombination epoch. It produces an approximately exponential damping tail in the [Cosmic microwave background power spectrum](#cosmic-microwave-background-power-spectrum) at multipoles $\ell\gtrsim1000$.

## Adiabatic initial conditions

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

Adiabatic initial conditions perturb every species by the same local time shift, so their relative number-density ratios are initially unperturbed. Photon acoustic modes then begin predominantly as displacement modes with cosine phase.

Equivalently, $\delta\rho_i/\dot{\bar\rho}_i$ is independent of the component $i$. The [non-adiabatic pressure perturbation](cosmic-inflation.md#non-adiabatic-pressure-perturbation) then vanishes, and the [comoving curvature perturbation](cosmic-inflation.md#comoving-curvature-perturbation) is conserved on [superhorizon scales](cosmic-inflation.md#superhorizon-scale) when anisotropic stress and gradient terms can be neglected.

### Adiabatic matter-string density relation

↑ **Parent:** [Adiabatic initial conditions](#adiabatic-initial-conditions)

For separately conserved barotropic components, an [adiabatic cosmological perturbation](#adiabatic-initial-conditions) has equal $\delta_N/(1+w_N)$. Pressureless matter and a $w=-1/3$ string component therefore have $\delta_s=2\delta_c/3$ on [superhorizon scales](cosmic-inflation.md#superhorizon-scale). In the supplied perfect-fluid synchronous equations, neglecting spatial gradients gives $S''+2\mathcal H S'=0$ for $S=\delta_s-2\delta_c/3$. Both $S$ and its independent decaying-mode amplitude must vanish to select the growing adiabatic solution. At finite wavenumber, pressure gradients generate departures from this leading long-wavelength relation.

## Cosmic microwave background acoustic peak

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

Cosmic microwave background acoustic peaks arise from photon-baryon oscillations caught at successive extrema at recombination. Their approximate phase is set by $kr_s=n\pi$ and their angular positions measure the sound horizon relative to the distance to last scattering.

### Angular projection of density and Doppler acoustic sources

↑ **Parent:** [Cosmic microwave background acoustic peak](#cosmic-microwave-background-acoustic-peak)

For an outward sightline, Fourier velocity $v_b^i=ik^i\theta_b$, and sudden last scattering, intrinsic photon temperature projects with a [Spherical Bessel function](analysis.md#spherical-bessel-function), while the Doppler term projects with its derivative. Density and velocity acoustic sources are approximately a quarter cycle out of phase. Their amplitude is suppressed by photon diffusion, giving a power damping envelope $e^{-2k^2/k_D^2}$. Projection maps the sound scale to peak spacing approximately $\pi D_*/r_s$ and the damping scale to angular multipoles of order $k_DD_*$.

### Adiabatic acoustic-peak spacing

↑ **Parent:** [Cosmic microwave background acoustic peak](#cosmic-microwave-background-acoustic-peak)

[Adiabatic initial conditions](#adiabatic-initial-conditions) select coherent cosine phases of the [photon-baryon acoustic oscillator](#photon-baryon-acoustic-oscillator). Its extrema at last scattering satisfy $kr_s\simeq n\pi$ and project to $\ell\simeq k\chi_*$. Thus $\ell_n\simeq n\pi\chi_*/r_s(\eta_*)$, with comoving [sound horizon](#sound-horizon) $r_s=\int d\eta/\sqrt{3(1+R)}$. Projection, driving and finite last-scattering width modify the exact peak locations.

## Free-streaming photon Boltzmann equation

↑ **Parent:** [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md)

In the absence of collisions, a photon phase-space density is constant along its geodesic. Linearizing this statement gives a first-order transport equation for the direction-dependent temperature perturbation.

### Photon brightness perturbation

↑ **Parent:** [Free-streaming photon Boltzmann equation](#free-streaming-photon-boltzmann-equation)

The photon brightness perturbation is the fractional frequency-integrated directional energy perturbation. For a small blackbody temperature shift $\Theta=\delta T/T$, $f_1=-qf_0'(q)\Theta$. Integration by parts gives $\Delta=4\Theta$. Its direction average is the photon density contrast. This temperature identification assumes a perturbation of blackbody form; the integrated brightness definition itself is more general.

// Target: cosmology.bigb

#### Synchronous photon brightness equation

↑ **Parent:** [Photon brightness perturbation](#photon-brightness-perturbation)

For collisionless photons in [synchronous gauge](linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology), their perturbed momentum obeys $q'=-qh'_{ij}n^in^j/2$. Terms in $q'\partial_qf_1$ and direction deflection times angular derivatives of $f_1$ are second order. Integrating the remaining linear [Collisionless Boltzmann equation](galaxy.md#collisionless-boltzmann-equation) over $q^3dq$ gives the displayed equation, because $\int q^4f_0' dq=-4\int q^3f_0dq$.

// Target: cosmology.bigb

##### Photon brightness equation for a negative spatial perturbation

↑ **Parent:** [Synchronous photon brightness equation](#synchronous-photon-brightness-equation)

For [synchronous gauge](linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) metric $ds^2=a^2[-d\tau^2+(\delta_{ij}-h_{ij})dx^idx^j]$, conserved-background [comoving momentum](linear-cosmological-density-perturbation.md#comoving-momentum) obeys $q'=qh'_{ij}n^in^j/2$. In the linear [Collisionless Boltzmann equation](galaxy.md#collisionless-boltzmann-equation), insert $\Delta=-4f_1/(qf_0')$ to obtain the displayed source. Using $\delta_{ij}+h_{ij}$ instead reverses both signs; it does not change the physics. The scalar contraction is $h'_{ij}n^in^j=(h'-h_s')/3+\mu^2h_s'$.

##### Synchronous photon momentum redshift

↑ **Parent:** [Synchronous photon brightness equation](#synchronous-photon-brightness-equation)

For a photon in $ds^2=a^2[-d\tau^2+(\delta_{ij}+h_{ij})dx^idx^j]$, the [null geodesic](special-relativity.md#null-geodesic) condition cancels the homogeneous $2\mathcal H p^0$ term in the derivative of $q=a^2p^0$. The remaining first-order [geodesic equation](riemannian-geometry.md#geodesic-equation) gives the displayed momentum change. Its direction is constant at zeroth order, so first-order redshift and brightness sources can be evaluated on the unperturbed ray; direction deflection multiplied by an already first-order anisotropy is second order.

### Photon Boltzmann hierarchy

↑ **Parent:** [Free-streaming photon Boltzmann equation](#free-streaming-photon-boltzmann-equation)

Expanding the direction-dependent photon temperature in [Legendre polynomials](differential-equation.md#legendre-polynomial) turns its transport equation into an infinite hierarchy. Free streaming couples each multipole $\Theta_\ell$ only to its neighbours $\Theta_{\ell-1}$ and $\Theta_{\ell+1}$.

#### Vector photon Boltzmann hierarchy

↑ **Parent:** [Photon Boltzmann hierarchy](#photon-boltzmann-hierarchy)

With $B_i^{(\pm)}=iB^{(\pm)}m_i^{(\pm)}/\sqrt2$ and the same convention for baryon velocity, choose $\Theta^{(\pm)}=\sum_{\ell\geq1}(-i)^\ell\sqrt{2\pi/(2\ell+1)}\Theta_\ell^{(\pm)}Y_{\ell,\pm1}$. The [spherical-harmonic streaming recurrence](analysis.md#spherical-harmonic-streaming-recurrence) gives

$$
\dot\Theta_\ell^{(\pm)}+k\left[\frac{\sqrt{(\ell+1)^2-1}}{2\ell+3}\Theta_{\ell+1}^{(\pm)}-\frac{\sqrt{\ell^2-1}}{2\ell-1}\Theta_{\ell-1}^{(\pm)}\right]=\dot\tau\left(1-\frac{\delta_{\ell2}}{10}\right)\Theta_\ell^{(\pm)}\mp(\dot B^{(\pm)}+\dot\tau v_b^{(\pm)})\delta_{\ell1}.
$$

This is the temperature-only [Thomson scattering](#thomson-scattering) hierarchy without polarization feedback, with optical depth to the observer satisfying $\dot\tau<0$. A [photon multipole normalization change](#photon-multipole-normalization-change) changes the denominators and the dipole-source prefactor. The lower coupling vanishes at $\ell=1$, so no vector monopole occurs.

#### Photon continuity equation

↑ **Parent:** [Photon Boltzmann hierarchy](#photon-boltzmann-hierarchy)

In [Newtonian gauge in cosmology](linear-cosmological-perturbation-theory.md#newtonian-gauge), the [Free-streaming photon Boltzmann equation](#free-streaming-photon-boltzmann-equation) is $\dot\Theta+\mathbf e\cdot\nabla\Theta=\dot\phi-\mathbf e\cdot\nabla\psi$. Angular averaging and the [photon angular temperature moments](#photon-angular-temperature-moments) give the displayed [continuity equation](physics.md#continuity-equation). Its dipole yields the [photon Euler equation](#photon-euler-equation), with the sign of the [anisotropic stress](general-relativity.md#anisotropic-stress) term determined by the stress convention.

#### Photon Euler equation

↑ **Parent:** [Photon Boltzmann hierarchy](#photon-boltzmann-hierarchy)

The dipole member of the photon Boltzmann hierarchy is the photon Euler equation. In Newtonian gauge and without collisions,

$$
\Theta_1'=\frac{k}{3}(\Theta_0+\Psi-2\Theta_2).
$$

### Line-of-sight solution for free-streaming photons

↑ **Parent:** [Free-streaming photon Boltzmann equation](#free-streaming-photon-boltzmann-equation)

The line-of-sight solution integrates the gravitational source along the unperturbed photon trajectory. In Fourier space the integrating factor $e^{ik\mu\eta}$ accounts for free streaming between emission and observation.

#### Matter-era photon endpoint solution

↑ **Parent:** [Line-of-sight solution for free-streaming photons](#line-of-sight-solution-for-free-streaming-photons)

In the negative-spatial-perturbation convention, a matter-era scalar solution $h=h_s+C=Ak^{1/2}\tau^2/4$ gives the displayed exact [photon brightness perturbation](#photon-brightness-perturbation). Integration gives emission bracket $\Delta_*+iAk^{-1/2}\mu\tau_*-Ak^{-3/2}$ times the propagation phase, plus observer monopole $Ak^{-3/2}$ and dipole $-iAk^{-1/2}\mu\tau_0$. Under ordinary adiabatic growing-mode initial conditions and $k\tau_*\ll1$, the emission gravitational term dominates higher angular multipoles. Arbitrary freely specified initial brightness need not obey this dominance.

#### Synchronous Sachs-Wolfe line-of-sight formula

↑ **Parent:** [Line-of-sight solution for free-streaming photons](#line-of-sight-solution-for-free-streaming-photons)

With instantaneous photon decoupling and tight-coupling initial brightness, integrate the [synchronous photon brightness equation](#synchronous-photon-brightness-equation) along the unperturbed ray $\mathbf x(\tau)=\mathbf x_0-\mathbf n(\tau_0-\tau)$. The direction $\mathbf n$ here is photon propagation, opposite to the observer-to-source sky direction. Emission terms are evaluated at the emitter, not the observer. The synchronous metric integral combines endpoint gravitational redshifts and evolving-potential effects when expressed in Newtonian gauge; it is not solely the [Integrated Sachs-Wolfe effect](#integrated-sachs-wolfe-effect).

// Target: cosmology.bigb

##### Endpoint terms in the synchronous Sachs-Wolfe formula

↑ **Parent:** [Synchronous Sachs-Wolfe line-of-sight formula](#synchronous-sachs-wolfe-line-of-sight-formula)

Use $h_{ij}n^in^j=h/3+(\mu^2-1/3)h_s$. Two integrations by parts of the anisotropic source give the exact [Cosmic microwave background anisotropy](cosmic-microwave-background-anisotropy.md) amplitude $W_*[\delta_\gamma/4+3i\mu\delta_\gamma'/(4k)+i\mu(h'-h_s')/(2k)+h_s''/(2k^2)]_*+[i\mu h_s'/(2k)-h_s''/(2k^2)]_0-\int_*^0W[(h'-h_s')/6-h_s'''/(2k^2)]d\tau$. The emission velocity was eliminated using $\delta_\gamma'+4ik\cdot v/3+2h'/3=0$. The local observer bracket is a monopole plus a dipole and can be discarded only after explicitly restricting to the measured higher angular multipoles. This identity fixes endpoint signs and integral factors without importing a different scalar-metric convention.

### Photon Boltzmann equation with Thomson scattering

↑ **Parent:** [Free-streaming photon Boltzmann equation](#free-streaming-photon-boltzmann-equation)

At linear order in Newtonian gauge, free streaming, gravitational redshift, and Thomson scattering combine into a first-order transport equation for the photon temperature perturbation. The collision term drives the radiation toward its monopole plus the electron bulk-velocity dipole.

#### Cosmological optical depth

↑ **Parent:** [Photon Boltzmann equation with Thomson scattering](#photon-boltzmann-equation-with-thomson-scattering)

The optical depth from conformal time $\eta$ to observation at $\eta_0$ is

$$
\tau(\eta)=\int_\eta^{\eta_0}\Gamma(\eta')\,d\eta'.
$$

The factor $e^{-\tau(\eta)}$ is the probability that a photon travels from $\eta$ to the observer without another scattering.

##### Cosmological visibility function

↑ **Parent:** [Cosmological optical depth](#cosmological-optical-depth)

The visibility function

$$
g(\eta)=\partial_\eta e^{-\tau(\eta)}
=\Gamma(\eta)e^{-\tau(\eta)}
$$

is the probability density for the conformal time of a CMB photon's last scattering.

This probability density describes last scattering during [cosmological recombination](cosmology.md#recombination-cosmology) and is built from the optical depth, rather than naming the recombination process itself.

###### Cosmic microwave background line-of-sight solution

↑ **Parent:** [Cosmological visibility function](#cosmological-visibility-function)

The CMB line-of-sight solution separates sharply localized last-scattering sources, weighted by the [cosmological visibility function](#cosmological-visibility-function), from integrated gravitational sources weighted by $e^{-\tau}$ along the photon trajectory.

###### Tensor CMB line-of-sight source

↑ **Parent:** [Cosmic microwave background line-of-sight solution](#cosmic-microwave-background-line-of-sight-solution)

Ignoring the last-scattering angular source and later scattering, the tensor-induced temperature anisotropy is $\Theta=-\tfrac12\int_{\eta_*}^{\eta_0}\dot h_{ij}(\eta,\mathbf x_0-(\eta_0-\eta)\mathbf e)e^ie^j d\eta$. An instantaneous [cosmological visibility function](#cosmological-visibility-function) alone leaves a scattering source at last scattering; leading tensor [tight coupling](#tight-coupling-approximation) supplies the additional reason to neglect it.

## ↑ Ancestors (5)

1. [Cosmic microwave background](cosmology.md#cosmic-microwave-background)
2. [Cosmology](cosmology.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (12)

- [Dark radiation on a cosmological brane](physics.md#dark-radiation-on-a-cosmological-brane)
- [Endpoint terms in the synchronous Sachs-Wolfe formula](#endpoint-terms-in-the-synchronous-sachs-wolfe-formula)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41.md#3/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-67.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-75.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-67.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-64.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-55.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-310.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-310.md#1/e/solution)
- [Reduced CMB bispectrum](#reduced-cmb-bispectrum)
- [Reionization damping of cosmic microwave background temperature anisotropy](cosmology.md#reionization-damping-of-cosmic-microwave-background-temperature-anisotropy)
