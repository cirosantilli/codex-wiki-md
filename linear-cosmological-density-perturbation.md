# Linear cosmological density perturbation

↑ **Parent:** [Cosmology](cosmology.md)

For pressureless subhorizon matter perturbations, a Fourier mode in conformal time obeys

$$
\delta''+\mathcal H\delta'-\frac32\Omega_M\mathcal H^2\delta=0,
$$

where $\mathcal H=a'/a$.

These equations describe the small-amplitude phase of [structure formation](cosmology.md#structure-formation); nonlinear growth requires a more general treatment.

**Table of contents**

- [Expansion-weighted derivative of a passive density perturbation](#expansion-weighted-derivative-of-a-passive-density-perturbation)
- [Cold-matter growth in a matter-coasting-fluid universe](#cold-matter-growth-in-a-matter-coasting-fluid-universe)
- [Linear density modes with polytropic pressure](#linear-density-modes-with-polytropic-pressure)
  - [Bessel density modes of a polytropic expanding universe](#bessel-density-modes-of-a-polytropic-expanding-universe)
    - [Pressure correction to a growing polytropic cosmological mode](#pressure-correction-to-a-growing-polytropic-cosmological-mode)
  - [Jeans modes of a four-thirds polytropic cosmological fluid](#jeans-modes-of-a-four-thirds-polytropic-cosmological-fluid)
  - [Repeated-root cosmological density mode](#repeated-root-cosmological-density-mode)
- [Peculiar gravitational potential](#peculiar-gravitational-potential)
- [Density contrast](#density-contrast)
  - [Comoving-gauge density contrast](#comoving-gauge-density-contrast)
    - [Growing-mode velocity potential in matter domination](#growing-mode-velocity-potential-in-matter-domination)
    - [Constant-equation-of-state comoving density equation](#constant-equation-of-state-comoving-density-equation)
      - [Radiation-era comoving density mode](#radiation-era-comoving-density-mode)
  - [Newtonian-gauge matter density from a constant gravitational potential](#newtonian-gauge-matter-density-from-a-constant-gravitational-potential)
  - [Smoothed matter density variance](#smoothed-matter-density-variance)
  - [Spherical top-hat window function](#spherical-top-hat-window-function)
  - [Linear growth factor](#linear-growth-factor)
    - [Einstein-de Sitter density-growth modes](#einstein-de-sitter-density-growth-modes)
    - [Matter-spectrum response to extra dark energy](#matter-spectrum-response-to-extra-dark-energy)
    - [Linear matter perturbation growth equation](#linear-matter-perturbation-growth-equation)
      - [Growth-time form of cosmological dust equations](#growth-time-form-of-cosmological-dust-equations)
        - [Pure growing-mode scaled velocity](#pure-growing-mode-scaled-velocity)
      - [Hubble parameter as a solution of the dust growth equation](#hubble-parameter-as-a-solution-of-the-dust-growth-equation)
    - [Linear growth equation](#linear-growth-equation)
      - [Reduced gravitational clustering strength](#reduced-gravitational-clustering-strength)
        - [Matter-era growth with reduced gravitational clustering strength](#matter-era-growth-with-reduced-gravitational-clustering-strength)
    - [Matter-dominated density-perturbation modes](#matter-dominated-density-perturbation-modes)
    - [Logarithmic growth of matter perturbations during radiation domination](#logarithmic-growth-of-matter-perturbations-during-radiation-domination)
      - [Radiation-background Bessel basis for matter perturbations](#radiation-background-bessel-basis-for-matter-perturbations)
    - [Freezing of matter perturbations during curvature domination](#freezing-of-matter-perturbations-during-curvature-domination)
  - [Linearized cosmological continuity equation](#linearized-cosmological-continuity-equation)
- [Jeans wavenumber](#jeans-wavenumber)
  - [Jeans instability](#jeans-instability)
    - [Nonrelativistic density equation in synchronous gauge](#nonrelativistic-density-equation-in-synchronous-gauge)
      - [CDM density equation in a matter-radiation universe](#cdm-density-equation-in-a-matter-radiation-universe)
        - [Superhorizon adiabatic CDM mode in radiation domination](#superhorizon-adiabatic-cdm-mode-in-radiation-domination)
          - [Superhorizon radiation-era entropy integration constants](#superhorizon-radiation-era-entropy-integration-constants)
    - [Jeans length](#jeans-length)
      - [Jeans support versus forced baryon response](#jeans-support-versus-forced-baryon-response)
    - [Jeans instability with Yukawa gravity](#jeans-instability-with-yukawa-gravity)
    - [Jeans swindle](#jeans-swindle)
    - [Static-universe Jeans modes](#static-universe-jeans-modes)
    - [Comoving Jeans length](#comoving-jeans-length)
      - [Baryon Jeans length across recombination](#baryon-jeans-length-across-recombination)
      - [Collisionless Jeans length](#collisionless-jeans-length)
        - [Cold-dark-matter kinetic Jeans scale](#cold-dark-matter-kinetic-jeans-scale)
        - [Free streaming](#free-streaming)
          - [Accumulated free-streaming distance in a radiation-dominated universe](#accumulated-free-streaming-distance-in-a-radiation-dominated-universe)
          - [Comoving momentum](#comoving-momentum)
            - [Physical momentum in an FRW universe](#physical-momentum-in-an-frw-universe)
- [Cosmological sound speed](#cosmological-sound-speed)
  - [Gradient instability of a negative-pressure perfect fluid](#gradient-instability-of-a-negative-pressure-perfect-fluid)
  - [Cosmological adiabatic sound speed](#cosmological-adiabatic-sound-speed)
- [Suppression of matter growth by smooth accelerated expansion](#suppression-of-matter-growth-by-smooth-accelerated-expansion)
  - [Matter density modes during cosmological-constant domination](#matter-density-modes-during-cosmological-constant-domination)
    - [Bessel density modes during exponential expansion](#bessel-density-modes-during-exponential-expansion)
      - [Monotone Jeans growth with positive cosmological constant](#monotone-jeans-growth-with-positive-cosmological-constant)
  - [Matter growth equation as a function of scale factor](#matter-growth-equation-as-a-function-of-scale-factor)
    - [Integral linear growth factor in a matter-Lambda universe](#integral-linear-growth-factor-in-a-matter-lambda-universe)
      - [Freezing of linear growth under a positive cosmological constant](#freezing-of-linear-growth-under-a-positive-cosmological-constant)
      - [Finite lower limit in the integral matter growth solution](#finite-lower-limit-in-the-integral-matter-growth-solution)
      - [Galaxy-formation bound on the cosmological constant](#galaxy-formation-bound-on-the-cosmological-constant)
- [Radiation domination](#radiation-domination)
  - [Mészáros effect](#meszaros-effect)
    - [Adiabatic radiation-era cold-dark-matter transfer solution](#adiabatic-radiation-era-cold-dark-matter-transfer-solution)
    - [Logarithmic CDM growth after radiation-era horizon entry](#logarithmic-cdm-growth-after-radiation-era-horizon-entry)
      - [Matching the CDM growing mode at horizon entry](#matching-the-cdm-growing-mode-at-horizon-entry)
    - [Mészáros equation](#meszaros-equation)
      - [Mészáros equation solution basis](#meszaros-equation-solution-basis)
- [Matter domination](#matter-domination)
- [Matter-era growing and decaying density modes](#matter-era-growing-and-decaying-density-modes)
  - [Cosmic-time matter density modes](#cosmic-time-matter-density-modes)
  - [Matter-era linear growth factor](#matter-era-linear-growth-factor)
- [Cosmological horizon crossing](#cosmological-horizon-crossing)
  - [Cosmological horizon entry](#cosmological-horizon-entry)
  - [Horizon-crossing time across matter-radiation equality](#horizon-crossing-time-across-matter-radiation-equality)
  - [Matter-era transfer of a horizon-crossing amplitude](#matter-era-transfer-of-a-horizon-crossing-amplitude)
- [Matter power spectrum](#matter-power-spectrum)
  - [Eight-megaparsec density fluctuation amplitude](#eight-megaparsec-density-fluctuation-amplitude)
  - [Potential fluctuations per logarithmic wavenumber](#potential-fluctuations-per-logarithmic-wavenumber)
  - [Band-limited linear density correlation](#band-limited-linear-density-correlation)
  - [Scale-free density correlation transform](#scale-free-density-correlation-transform)
  - [Harrison-Peebles-Zeldovich spectrum](#harrison-peebles-zeldovich-spectrum)
    - [Gaussian horizon-crossing variance for a Harrison-Zeldovich spectrum](#gaussian-horizon-crossing-variance-for-a-harrison-zeldovich-spectrum)
  - [Broken matter power spectrum from horizon entry](#broken-matter-power-spectrum-from-horizon-entry)
- [Neutrino free streaming](#neutrino-free-streaming)
  - [Neutrino Boltzmann hierarchy](#neutrino-boltzmann-hierarchy)

## Expansion-weighted derivative of a passive density perturbation

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

When the self-gravity source in the pressureless [linear cosmological density perturbation](linear-cosmological-density-perturbation.md) equation is negligible, $\ddot\delta+2(\dot a/a)\dot\delta=0$. Multiplication by $a^2$ makes it $d(a^2\dot\delta)/dt=0$, so $\delta=C_1+C_2\int dt/a^2(t)$. This explains how [Hubble friction](cosmology.md#hubble-friction) changes growth for an arbitrary positive [scale factor](cosmology.md#scale-factor-cosmology). For $a\propto t^p$, the nonconstant mode is $t^{1-2p}$ when $p\ne1/2$ and $\log t$ when $p=1/2$.

## Cold-matter growth in a matter-coasting-fluid universe

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

In a spatially flat universe containing separately conserved [pressureless matter](cosmology.md#pressureless-matter) and a [coasting fluid](cosmology.md#coasting-fluid) with $w=-1/3$, the ratio $\eta=\rho_s/\rho_m$ is proportional to the [scale factor](cosmology.md#scale-factor-cosmology). If the coasting component is modeled by the barotropic fluid perturbation equations with no [anisotropic stress](general-relativity.md#anisotropic-stress), its contribution to the trace gravitational source vanishes because $1+3w=0$. The matter growing mode is

$$
D(\eta)=\frac52\frac{\sqrt{1+\eta}}{\eta^{3/2}}\int_0^\eta\frac{x^{3/2}}{(1+x)^{3/2}}\,dx.
$$

A decaying solution is $D_-=\sqrt{1+\eta}/\eta^{3/2}$. The [reduction of order](differential-equation.md#reduction-of-order) formula with integrating factor $\eta^{3/2}\sqrt{1+\eta}$ produces the integral solution. It has $D=\eta[1-4\eta/7+O(\eta^2)]$ during [matter domination](#matter-domination) and tends to $5/2$ during coasting-fluid domination. Thus growth freezes rather than continuing in proportion to the [scale factor](cosmology.md#scale-factor-cosmology). The background geometry is flat despite the same background expansion law as an open dust universe.

## Linear density modes with polytropic pressure

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

In a flat matter-dominated universe with $a\propto t^{2/3}$ and $P\propto\rho^{4/3}$, the squared [sound speed](compressible-flow.md#speed-of-sound) scales as $t^{-2/3}$. Each comoving Fourier mode then satisfies an [Euler-Cauchy equation](differential-equation.md#euler-cauchy-equation), with gravitational growth at long wavelengths and logarithmic-time acoustic oscillations at short wavelengths.

### Bessel density modes of a polytropic expanding universe

↑ **Parent:** [Linear density modes with polytropic pressure](#linear-density-modes-with-polytropic-pressure)

For a flat Newtonian expanding background $R\propto t^{2/3}$ with [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state) $p=K\rho^\gamma$, a comoving [density contrast](#density-contrast) satisfies $\ddot\delta+4\dot\delta/(3t)+[\Lambda^2t^{-2\nu-2}-2/(3t^2)]\delta=0$. Here $\Lambda=kc(t_0)t_0^{\gamma-1/3}$ and $\nu=\gamma-4/3$. For $\nu>0$, substitution $z=\Lambda/(\nu t^\nu)$ and $\delta=t^{-1/6}y(z)$ gives the [Bessel equation](analysis.md#bessel-differential-equation) of order $\lambda$. A universally valid basis uses the [Bessel function of the first kind](analysis.md#bessel-function-of-the-first-kind) and [Bessel function of the second kind](analysis.md#bessel-function-of-the-second-kind), $t^{-1/6}J_\lambda(z)$ and $t^{-1/6}Y_\lambda(z)$. When $\lambda$ is not an integer, $J_{-\lambda}$ can replace $Y_\lambda$. For $4/3<\gamma<5/3$, the early oscillatory envelope is $t^{(3\gamma-5)/6}$; late modes have leading powers $t^{2/3}$ and $t^{-1}$. Late growth requires a nonzero coefficient of the growing branch.

#### Pressure correction to a growing polytropic cosmological mode

↑ **Parent:** [Bessel density modes of a polytropic expanding universe](#bessel-density-modes-of-a-polytropic-expanding-universe)

Put $\delta=t^{2/3}h(t)$ in the [Bessel density modes of a polytropic expanding universe](#bessel-density-modes-of-a-polytropic-expanding-universe) equation. It becomes $h''+8h'/(3t)+\Lambda^2t^{-2\nu-2}h=0$. Substituting $h=1+a\Lambda^2t^{-2\nu}+\cdots$ gives $a=[2\nu(5/3-2\nu)]^{-1}$. Since $ck/R=\Lambda t^{-\nu-1}$, the fractional pressure correction is small when $(ck/R)^2t^2\ll2\nu(5/3-2\nu)$. For $0<\nu<1/3$, this is the order-of-magnitude condition $ck/R\ll\sqrt{6\pi\nu G\rho}$. It describes approach to the dust-like growing branch, not an exact universal time at which every initial perturbation starts increasing. The instantaneous [Jeans instability](#jeans-instability) balance instead compares $(ck/R)^2$ with $4\pi G\rho$.

### Jeans modes of a four-thirds polytropic cosmological fluid

↑ **Parent:** [Linear density modes with polytropic pressure](#linear-density-modes-with-polytropic-pressure)

For a nonrelativistic [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state) $P=K\rho^{4/3}$ during [matter domination](#matter-domination), $c_s^2\propto a^{-1}$ and the comoving [Jeans wavenumber](#jeans-wavenumber) is constant. The leading density equation becomes $\ddot\delta+4\dot\delta/(3t)+[2(q-1)/(3t^2)]\delta=0$, giving the displayed powers. A growing mode exists for $q<1$; at $q=1$ one mode is constant. At $q=25/24$ the repeated root has the second solution $t^{-1/6}\ln t$. For $q>25/24$ both real solutions oscillate in $\ln t$ with envelope $t^{-1/6}$. Thus the instability threshold and the onset of oscillatory solutions are distinct in an expanding background.

### Repeated-root cosmological density mode

↑ **Parent:** [Linear density modes with polytropic pressure](#linear-density-modes-with-polytropic-pressure)

When the characteristic exponents of the density-mode [Euler-Cauchy equation](differential-equation.md#euler-cauchy-equation) coincide, the second independent solution gains a logarithm. In the polytropic matter-era example the complete solution at this threshold is $t^{-1/6}(A+B\log t)$.

## Peculiar gravitational potential

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

The peculiar gravitational potential is the Newtonian potential after subtracting the potential of the homogeneous expanding background. In comoving coordinates it obeys a Poisson equation sourced by the [density contrast](#density-contrast), so its gradient accelerates matter relative to the [Hubble flow](cosmology.md#hubble-flow).

## Density contrast

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Density_contrast)

The density contrast is the fractional perturbation $\delta=(\rho-\bar\rho)/\bar\rho$.

### Comoving-gauge density contrast

↑ **Parent:** [Density contrast](#density-contrast)

For a [perfect fluid](general-relativity.md#perfect-fluid) with $P=w\rho$, in [Newtonian gauge in cosmology](linear-cosmological-perturbation-theory.md#newtonian-gauge) the density perturbation on fluid-comoving slices is the displayed combination of the fractional density perturbation and velocity potential. The Einstein energy and momentum constraints combine into $\nabla^2\phi=4\pi Ga^2\bar\rho\Delta$ when scalar anisotropic stress vanishes. This gives a relativistic Poisson constraint valid beyond the subhorizon limit.

#### Growing-mode velocity potential in matter domination

↑ **Parent:** [Comoving-gauge density contrast](#comoving-gauge-density-contrast)

During [matter domination](#matter-domination) in a flat universe, the growing [comoving-gauge density contrast](#comoving-gauge-density-contrast) is proportional to $a\propto\eta^2$. Its Newtonian potential is constant by the Poisson constraint. The momentum constraint gives $v=-2\phi/(3\mathcal H)=-\eta\phi/3$. Thus the peculiar velocity potential grows as $a^{1/2}$ in the convention where the peculiar velocity is $\nabla v$.

#### Constant-equation-of-state comoving density equation

↑ **Parent:** [Comoving-gauge density contrast](#comoving-gauge-density-contrast)

For a flat single-fluid background with constant [barotropic equation of state](cosmology.md#barotropic-equation-of-state), $w\ne-1/3$, adiabatic perturbations and zero anisotropic stress, $a\propto\eta^{2/(1+3w)}$ and $a^2\bar\rho\propto\eta^{-2}$. The scalar potential obeys $\phi''+[6(1+w)/(1+3w)]\phi'/\eta-w\nabla^2\phi=0$. Substituting the Poisson constraint $\Delta\propto\eta^2\nabla^2\phi$ gives the displayed equation. The homogeneous mode and the degenerate vacuum fluid $w=-1$ require separate interpretation.

##### Radiation-era comoving density mode

↑ **Parent:** [Constant-equation-of-state comoving density equation](#constant-equation-of-state-comoving-density-equation)

For [radiation in cosmology](cosmology.md#radiation-in-cosmology), the [comoving-gauge density contrast](#comoving-gauge-density-contrast) satisfies $\Delta_k''+(k^2/3-2/\eta^2)\Delta_k=0$. The displayed basis solves it. The first mode is regular and grows as $Ax^2/3$ outside the [sound horizon](cosmic-microwave-background-anisotropy.md#sound-horizon); the second diverges as $B/x$ toward the initial singularity. At large $x$, the regular mode approaches $-A\cos x$ and has constant-amplitude acoustic oscillations.

### Newtonian-gauge matter density from a constant gravitational potential

↑ **Parent:** [Density contrast](#density-contrast)

In [matter domination](#matter-domination) with the constant growing potential, the full Newtonian-gauge energy constraint gives the stated [density contrast](#density-contrast). The second term dominates inside the [Hubble radius](cosmology.md#hubble-radius) and grows as $a$, because $\mathcal H^2\propto a^{-1}$. Outside the [Hubble radius](cosmology.md#hubble-radius), the constant $-2\Phi$ term dominates and is gauge dependent. The comoving density combination $\Delta_c=\delta_c+3\mathcal H\theta_c/k^2$ cancels it for $\theta_c=2k^2\Phi/(3\mathcal H)$, leaving the [cosmological Poisson equation](linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) relation. Matter-spectrum power laws must specify whether they refer to this comoving density or to subhorizon Newtonian-gauge density.

### Smoothed matter density variance

↑ **Parent:** [Density contrast](#density-contrast)

The [smoothed matter density variance](#smoothed-matter-density-variance) measures the root-mean-square linear [density contrast](#density-contrast) after applying a window corresponding to a Lagrangian mass scale. For a homogeneous isotropic field it is $\sigma^2=(1/(2\pi^2))\int k^2P(k)|W(kR)|^2dk$. The variance convention, growth epoch and smoothing mass-density relation must agree with the collapse barrier used in a halo abundance calculation.

### Spherical top-hat window function

↑ **Parent:** [Density contrast](#density-contrast)

A spherical top-hat window function averages a field uniformly inside a [sphere](geometry-and-topology.md#sphere) of radius $R$ and gives zero weight outside it. Its normalized real-space kernel is $W_R(\mathbf x)=3/(4\pi R^3)$ for $|\mathbf x|\leq R$, and its [Fourier transform](analysis.md#fourier-transform) is

$$
\widetilde W_R(k)=3\frac{\sin(kR)-kR\cos(kR)}{(kR)^3}.
$$

### Linear growth factor

↑ **Parent:** [Density contrast](#density-contrast)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_growth_factor)

The linear growth factor multiplies the growing mode of a linear cosmological density perturbation, so $\delta(\mathbf x,t)=D(t)\delta(\mathbf x,t_0)/D(t_0)$ when scale-independent growth applies.

#### Einstein-de Sitter density-growth modes

↑ **Parent:** [Linear growth factor](#linear-growth-factor)

For pressureless [linear cosmological density perturbations](linear-cosmological-density-perturbation.md) in an [Einstein-de Sitter universe](large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $H=2/(3t)$ and $4\pi G\bar\rho_m=2/(3t^2)$. The growth equation is an [Euler differential equation](differential-equation.md#cauchy-euler-equation) whose indicial equation is $(p-2/3)(p+1)=0$. Hence the independent modes are $\delta_+\propto t^{2/3}\propto a$ and $\delta_-\propto t^{-1}\propto a^{-3/2}$. The first is the growing [linear growth factor](#linear-growth-factor), while the second is a decaying transient.

#### Matter-spectrum response to extra dark energy

↑ **Parent:** [Linear growth factor](#linear-growth-factor)

With physical matter and radiation densities, primordial amplitudes and spatial flatness fixed, extra smooth late [dark energy](cosmology.md#dark-energy) increases $H_0$ but keeps $\Omega_mH_0^2$ fixed. Provided the [dark energy](cosmology.md#dark-energy) is negligible at equality, the early [cosmological transfer function](linear-cosmological-perturbation-theory.md#cosmological-transfer-function) and equality wavenumber in physical units are unchanged. Earlier accelerated expansion suppresses the [linear growth factor](#linear-growth-factor), lowering present dimensional matter power by its squared growth ratio. Units involving $h$ can additionally relabel the horizontal and vertical axes.

#### Linear matter perturbation growth equation

↑ **Parent:** [Linear growth factor](#linear-growth-factor)

For pressureless sub-Hubble perturbations, combine the [linearized cosmological continuity equation](#linearized-cosmological-continuity-equation), [cosmological Euler equation](linear-cosmological-perturbation-theory.md#cosmological-euler-equation) and gravitational [Poisson equation](partial-differential-equation.md#poisson-equation) with matter as its source. The expansion contributes a $2H$ friction term and matter self-gravity contributes the negative coefficient of $\delta$. The background expansion can include radiation or dark energy; treating their perturbations as additional sources requires a more complete system.

##### Growth-time form of cosmological dust equations

↑ **Parent:** [Linear matter perturbation growth equation](#linear-matter-perturbation-growth-equation)

Use a monotone [linear growth factor](#linear-growth-factor) $b(t)$ as time, $\mathbf u=\dot{\mathbf x}/\dot b$, and $\psi=a\varphi/(Cb)$ with $C=3H_0^2\Omega_{m0}/2$ and $a_0=1$. The [cosmological Poisson equation](linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) becomes $\nabla^2\psi=\delta/b$; the [continuity equation](physics.md#continuity-equation) becomes $\partial_b\delta+\nabla\cdot[(1+\delta)\mathbf u]=0$. The material derivative is $D_b=\partial_b+\mathbf u\cdot\nabla$. Substitution into the pressureless [cosmological Euler equation](linear-cosmological-perturbation-theory.md#cosmological-euler-equation), followed by the growth equation and $\dot b=Hbf$, proves the displayed motion equation, with $f=d\ln b/d\ln a$. The density derivative in the conservative continuity equation is Eulerian, not material.

###### Pure growing-mode scaled velocity

↑ **Parent:** [Growth-time form of cosmological dust equations](#growth-time-form-of-cosmological-dust-equations)

For a pure scalar growing [density contrast](#density-contrast) with time-independent boundary conditions, $\nabla^2\psi=\delta_*$ fixes the scaled [peculiar gravitational potential](#peculiar-gravitational-potential) up to an irrelevant constant. The linearized continuity equation fixes the longitudinal scaled velocity to $-\nabla\psi$. The remaining homogeneous velocity is $\mathbf u_h=\mathbf C(\mathbf x)/(a^2\dot b)$; a divergence-free such field does not change the growing density at linear order. Excluding this decaying velocity component is necessary for time-independent $\mathbf u$. In an [Einstein-de Sitter universe](large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $b=a$ and $\mathbf u_h\propto a^{-3/2}$, furnishing a counterexample if the pure growing-velocity hypothesis is omitted.

##### Hubble parameter as a solution of the dust growth equation

↑ **Parent:** [Linear matter perturbation growth equation](#linear-matter-perturbation-growth-equation)

For dust, curvature and a constant [cosmological constant](cosmology.md#cosmological-constant), write $H^2=Aa^{-3}+Ba^{-2}+C$. Then $\dot H=-3Aa^{-3}/2-Ba^{-2}$ and $\ddot H=H(9Aa^{-3}/2+2Ba^{-2})$, which imply $\ddot H+2H\dot H-3Aa^{-3}H/2=0$. Thus $H$ is a solution of the pressureless [linear matter perturbation growth equation](#linear-matter-perturbation-growth-equation). In an [Einstein-de Sitter universe](large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $H\propto t^{-1}$ is the decaying mode and the independent growing mode is $t^{2/3}$. Additional dynamical components need not preserve this identity.

#### Linear growth equation

↑ **Parent:** [Linear growth factor](#linear-growth-factor)

For pressureless matter on subhorizon scales, the [linear growth factor](#linear-growth-factor) obeys

$$
\ddot D+2H\dot D-4\pi G\bar\rho_mD=0.
$$

The second term is dilution by [cosmic expansion](cosmology.md#expansion-of-the-universe), while the final term drives [Jeans instability](#jeans-instability).

##### Reduced gravitational clustering strength

↑ **Parent:** [Linear growth equation](#linear-growth-equation)

Replacing the self-gravity term in the matter growth equation by $(1-f)4\pi G\bar\rho_mD$, with $0<1-f<1$, weakens clustering while leaving the background expansion unchanged.

###### Matter-era growth with reduced gravitational clustering strength

↑ **Parent:** [Reduced gravitational clustering strength](#reduced-gravitational-clustering-strength)

During matter domination, the growing mode under a reduced clustering strength $1-f$ is

$$
D(t)\propto t^{s(f)},
\qquad
s(f)=\frac{-1+\sqrt{25-24f}}6.
$$

It grows more slowly than the standard $t^{2/3}$ mode whenever $0<f<1$.

#### Matter-dominated density-perturbation modes

↑ **Parent:** [Linear growth factor](#linear-growth-factor)

In a matter-dominated universe, the long-wavelength pressureless growth equation has modes

$$
\delta_+\propto a,
\qquad
\delta_-\propto a^{-3/2}.
$$

#### Logarithmic growth of matter perturbations during radiation domination

↑ **Parent:** [Linear growth factor](#linear-growth-factor)

When matter self-gravity is negligible during radiation domination, $a\propto t^{1/2}$ and $\ddot\delta+2H\dot\delta=0$ gives $\delta=C_1+C_2\log a$.

##### Radiation-background Bessel basis for matter perturbations

↑ **Parent:** [Logarithmic growth of matter perturbations during radiation domination](#logarithmic-growth-of-matter-perturbations-during-radiation-domination)

In a radiation-dominated background with matter self-gravity retained, $\delta_{aa}+\delta_a/a-3\delta/(2aa_{\rm eq})=0$. A change to $x=\sqrt{6a/a_{\rm eq}}$ gives the [Modified Bessel differential equation](analysis.md#modified-bessel-differential-equation) of order zero. The [Modified Bessel function of the first kind](analysis.md#modified-bessel-function-of-the-first-kind) increases as $1+3a/(2a_{\rm eq})+\cdots$; the [Modified Bessel function of the second kind](analysis.md#modified-bessel-function-of-the-second-kind) decreases with a leading negative logarithm. The early solution space has the constant/logarithmic behaviors, not the $a$ growth of [matter domination](#matter-domination). This background approximation must not be extrapolated through equality.

#### Freezing of matter perturbations during curvature domination

↑ **Parent:** [Linear growth factor](#linear-growth-factor)

During curvature domination $a\propto t$, so a pressureless perturbation without a self-gravity term has modes $1$ and $a^{-1}$. The surviving mode is constant.

### Linearized cosmological continuity equation

↑ **Parent:** [Density contrast](#density-contrast)

For a pressureless fluid with

$$
\rho=\bar\rho+\epsilon\,\delta\rho,
\qquad
\mathbf v=\epsilon\,\delta\mathbf v,
$$

the first-order [density contrast](#density-contrast) $\delta=\delta\rho/\bar\rho$ obeys

$$
\dot\delta=-\frac1a\nabla\cdot\delta\mathbf v.
$$

## Jeans wavenumber

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

The Jeans wavenumber separates pressure-supported modes from gravitationally unstable density modes.

### Jeans instability

↑ **Parent:** [Jeans wavenumber](#jeans-wavenumber)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jeans_instability)

Jeans instability is the gravitational growth of density perturbations whose self-gravity overcomes pressure support. For physical sound speed $c_s$, the comoving threshold is

$$
k_J=\frac{a\sqrt{4\pi G\bar\rho}}{c_s}.
$$

Modes with $k\ll k_J$ grow gravitationally, whereas modes with $k\gg k_J$ undergo pressure-supported acoustic oscillations.

#### Nonrelativistic density equation in synchronous gauge

↑ **Parent:** [Jeans instability](#jeans-instability)

For a matter-dominated fluid with constant $c_s^2=w\ll1$, combine [stress-energy conservation](general-relativity.md#stress-energy-conservation) in synchronous gauge with the scalar trace Einstein equation. Discard pressure corrections to the background gravitational and velocity-damping terms while retaining the potentially large pressure-gradient term $wk^2\delta$. This produces the displayed leading nonrelativistic equation. It is not an exact equation at finite $w$. At negligible pressure the growing and decaying matter-era solutions are $\tau^2$ and $\tau^{-3}$.

// Target: cosmology.bigb

##### CDM density equation in a matter-radiation universe

↑ **Parent:** [Nonrelativistic density equation in synchronous gauge](#nonrelativistic-density-equation-in-synchronous-gauge)

In [Synchronous gauge in cosmology](linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) with coordinates comoving with [cold dark matter](cosmology.md#cold-dark-matter), the linearized [Einstein field equations](general-relativity.md#einstein-field-equations) and matter conservation give the displayed density equation. Primes denote [conformal time](cosmology.md#conformal-time) derivatives. The radiation term contains its pressure contribution and cannot be dropped on [superhorizon scales](cosmic-inflation.md#superhorizon-scale) merely because radiation oscillates after [cosmological horizon entry](#cosmological-horizon-entry).

###### Superhorizon adiabatic CDM mode in radiation domination

↑ **Parent:** [CDM density equation in a matter-radiation universe](#cdm-density-equation-in-a-matter-radiation-universe)

During [radiation domination](#radiation-domination), $a\propto\tau$ and $8\pi G\rho_Ra^2=3/\tau^2$. The [adiabatic initial conditions](cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) reduce the [CDM density equation in a matter-radiation universe](#cdm-density-equation-in-a-matter-radiation-universe) to $\delta_C''+\delta_C'/\tau-4\delta_C/\tau^2=0$. Its [Euler-Cauchy equation](differential-equation.md#euler-cauchy-equation) powers are two and minus two. The growing solution is the displayed one, in the stated CDM-comoving [synchronous gauge](linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology).

###### Superhorizon radiation-era entropy integration constants

↑ **Parent:** [Superhorizon adiabatic CDM mode in radiation domination](#superhorizon-adiabatic-cdm-mode-in-radiation-domination)

In the leading [radiation domination](#radiation-domination) limit, neglect $k^2\delta_r$ and the matter contribution to gravity. The radiation equation gives $S''=0$. Substitution into $\delta_c''+\delta_c'/\tau=3\delta_r/\tau^2$ gives

$$
\delta_c=C_g\tau^2+C_d\tau^{-2}-\frac34S_0-S_1\tau,\qquad
\delta_r=\frac43C_g\tau^2+\frac43C_d\tau^{-2}-\frac13S_1\tau.
$$

Thus [adiabatic initial conditions](cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) select both $S_0=0$ and $S_1=0$, leaving the growing and decaying power-law modes. The four constants describe the leading supplied coupled system; regularity and additional initial [Einstein field equations](general-relativity.md#einstein-field-equations) constraints can further restrict their physical interpretation.

#### Jeans length

↑ **Parent:** [Jeans instability](#jeans-instability)

With physical wavelength $2\pi/k$, the [Jeans length](#jeans-length) is $2\pi/k_J$, where the [Jeans wavenumber](#jeans-wavenumber) is $\sqrt{4\pi G\rho}/c_s$. Linear pressure support dominates gravity below this length, whereas longer wavelengths can grow. In an expanding background the growth also depends on the Hubble damping term, so the static threshold does not by itself give the time dependence.

##### Jeans support versus forced baryon response

↑ **Parent:** [Jeans length](#jeans-length)

When baryons are a small fraction of the gravitating matter, their perturbation is forced by the [cold dark matter](cosmology.md#cold-dark-matter) potential. Comparing pressure frequency $c_s^2k^2$ with $4\pi Ga^2\bar\rho_C$ yields the scale $\lambda_J=c_s\sqrt{\pi/(G\bar\rho_C)}$ for following the growing matter mode. It is not an absolute statement that every sub-Jeans baryon perturbation is zero or cannot be forced: a slowly varying response is $\delta_B\simeq(k_J^2/k^2)\delta_C$. In the pressureless limit the difference from CDM is a constant plus a decaying mode during [matter domination](#matter-domination), so baryons catch up in relative amplitude.

#### Jeans instability with Yukawa gravity

↑ **Parent:** [Jeans instability](#jeans-instability)

For the screened attraction $-Gm e^{-\alpha r}/r$ with $\alpha\geq0$, $(\nabla^2-\alpha^2)\phi=4\pi G\rho$. A static homogeneous barotropic medium with [sound speed](compressible-flow.md#speed-of-sound) $v_s>0$ has $\omega^2=k^2[v_s^2-4\pi G\rho_0/(k^2+\alpha^2)]$. A growing mode exists iff $4\pi G\rho_0>v_s^2\alpha^2$, with $0<k<\sqrt{4\pi G\rho_0/v_s^2-\alpha^2}$. For nonzero screening the growth rate tends to zero as $k\to0$; the homogeneous mode is not an exponentially growing density fluctuation. Finite interaction range can therefore remove the instability entirely, while all sufficiently small nonzero wavenumbers remain unstable when the threshold is exceeded.

#### Jeans swindle

↑ **Parent:** [Jeans instability](#jeans-instability)

The [Jeans swindle](#jeans-swindle) is the removal of the unperturbed uniform density's gravitational field when treating an infinite homogeneous Newtonian medium as static. Without such subtraction or an external supporting prescription, a nonzero constant density and zero background gravitational [acceleration](classical-mechanics.md#acceleration) cannot satisfy Poisson's equation. Linear perturbations then obey $\nabla^2\delta\phi=4\pi G\delta\rho$. This is a specified idealization, not an exact isolated infinite equilibrium.

#### Static-universe Jeans modes

↑ **Parent:** [Jeans instability](#jeans-instability)

In a static homogeneous universe, a density mode obeys

$$
\ddot\delta_k+c_s^2(k^2-k_J^2)\delta_k=0.
$$

Modes with $k>k_J$ oscillate as sound waves, while modes with $k<k_J$ have one exponentially growing and one exponentially decaying solution.

#### Comoving Jeans length

↑ **Parent:** [Jeans instability](#jeans-instability)

Up to a convention-dependent numerical factor, a collisional fluid has comoving Jeans length $\lambda_{J,\mathrm{com}}=(c_s/a)\sqrt{\pi/(G\bar\rho)}$.

##### Baryon Jeans length across recombination

↑ **Parent:** [Comoving Jeans length](#comoving-jeans-length)

Before [cosmological recombination](cosmology.md#recombination-cosmology), [photon-baryon sound speed](cosmic-microwave-background-anisotropy.md#photon-baryon-sound-speed) controls the baryonic [comoving Jeans length](#comoving-jeans-length). The tightly coupled [photon-baryon fluid](cosmic-microwave-background-anisotropy.md#photon-baryon-fluid) has $c_s^2=c^2/[3(1+R_b)]$, where $R_b=3\bar\rho_b/(4\bar\rho_\gamma)\propto a$. Using total background density in the instantaneous dynamical Jeans estimate, the scale grows as $a$ during [radiation domination](#radiation-domination), approaches a plateau in strongly baryon-loaded [matter domination](#matter-domination), and drops when [photon decoupling](cosmology.md#photon-decoupling) removes photon pressure support. Subsequently, adiabatic monatomic-gas cooling gives $T_b\propto a^{-2}$ and a [comoving Jeans length](#comoving-jeans-length) proportional to $a^{-1/2}$. Residual [Compton scattering](physics.md#compton-scattering) can delay that cooling law.

##### Collisionless Jeans length

↑ **Parent:** [Comoving Jeans length](#comoving-jeans-length)

For collisionless matter, velocity dispersion replaces sound speed in the Jeans estimate. After free decoupling, a nonrelativistic thermal velocity dispersion redshifts as $a^{-1}$.

###### Cold-dark-matter kinetic Jeans scale

↑ **Parent:** [Collisionless Jeans length](#collisionless-jeans-length)

An instantaneous kinetic suppression estimate replaces [sound speed](compressible-flow.md#speed-of-sound) by the [velocity dispersion](galaxy.md#velocity-dispersion) of [cold dark matter](cosmology.md#cold-dark-matter). Nonrelativistic particles in thermal contact with [photons](quantum-mechanics.md#photon) have $\sigma\propto a^{-1/2}$; after [kinetic decoupling](cosmology.md#kinetic-decoupling), their momenta redshift and $\sigma\propto a^{-1}$. A background dynamical estimate using total density is then constant during [radiation domination](#radiation-domination) and decreases as $a^{-1/2}$ during [matter domination](#matter-domination). Using only the species' own matter density instead makes the self-gravitating [collisionless Jeans length](#collisionless-jeans-length) decrease as $a^{-1/2}$ throughout the decoupled nonrelativistic era. Neither instantaneous estimate is the accumulated distance traveled by [collisionless free streaming](#free-streaming).

###### Free streaming

↑ **Parent:** [Collisionless Jeans length](#collisionless-jeans-length)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_streaming)

Collisionless free streaming is the ballistic motion of particles out of an overdensity. It erases perturbations below the comoving distance travelled by particles while their thermal velocities are appreciable.

###### Accumulated free-streaming distance in a radiation-dominated universe

↑ **Parent:** [Free streaming](#free-streaming)

Suppose a collisionless particle has [momentum](classical-mechanics.md#momentum) $p=T_r\propto a^{-1}$ during pure [radiation domination](#radiation-domination). Since $a\propto t^{1/2}$, integrating $\chi=\int_0^t v(t')dt'/a(t')$ gives the displayed [comoving distance](cosmology.md#comoving-radial-distance). The physical distance at observation is $a\chi=H^{-1}\operatorname{arsinh}(y)/y$, $y=m/T_r$. The printed expression without $a^{-1}$ is consequently a physical distance, or a comoving distance in coordinates normalized to $a=1$ at observation. Its ratio tends to one in the relativistic limit and to $\log(2y)/y$ in the [nonrelativistic limit](special-relativity.md#nonrelativistic-limit). The accumulated scale differs from an instantaneous velocity-over-expansion-rate estimate.

###### Comoving momentum

↑ **Parent:** [Free streaming](#free-streaming)

[Spatial translation](general-relativity.md#spatial-translation) symmetry in a flat [FRW metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric) conserves the covariant [canonical momentum](classical-mechanics.md#canonical-momentum) $q_i=ma^2dx^i/ds$ of a freely falling massive particle. An orthonormal spatial frame gives $p_{{\rm phys},i}=q_i/a$, so physical [momentum](classical-mechanics.md#momentum) [redshifts](optics.md#redshift) as $a^{-1}$ even while the particle changes from relativistic to nonrelativistic motion. The local [energy](classical-mechanics.md#energy) is $E=\sqrt{m^2+q^2/a^2}$ and the coordinate [velocity](classical-mechanics.md#velocity) is $d\mathbf x/dt=\mathbf q/[a\sqrt{q^2+m^2a^2}]$.

###### Physical momentum in an FRW universe

↑ **Parent:** [Comoving momentum](#comoving-momentum)

A freely falling particle's physical [momentum](classical-mechanics.md#momentum) is measured in the local [orthonormal frame](general-relativity.md#orthonormal-frame-in-spacetime) of a [comoving observer](cosmology.md#comoving-observer). With proper [peculiar velocity](cosmology.md#peculiar-velocity) $\mathbf v=a\,d\mathbf x/dt$ and [Lorentz factor](special-relativity.md#lorentz-factor) $\gamma=(1-v^2)^{-1/2}$, it is $m\gamma\mathbf v$. It differs by one factor of the [scale factor](cosmology.md#scale-factor-cosmology) from the conserved [comoving momentum](#comoving-momentum). For a [nonrelativistic particle](special-relativity.md#nonrelativistic-particle), its [peculiar velocity](cosmology.md#peculiar-velocity) therefore decays as $a^{-1}$.

## Cosmological sound speed

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

For a barotropic fluid, the squared sound speed is $c_s^2=\partial P/\partial\rho$. A Fourier density mode obeys

$$
\ddot\delta+2H\dot\delta
+\left(\frac{c_s^2k^2}{a^2}-4\pi G\bar\rho\right)\delta=0
$$

in linear Newtonian perturbation theory.

### Gradient instability of a negative-pressure perfect fluid

↑ **Parent:** [Cosmological sound speed](#cosmological-sound-speed)

For a barotropic [perfect fluid](general-relativity.md#perfect-fluid) with constant $w$, its [cosmological adiabatic sound speed](#cosmological-adiabatic-sound-speed) satisfies $c_s^2=w$. If $w<0$, the short-wavelength pressure term has the wrong sign for restoring oscillations: a mode grows as $\exp(\sqrt{-w}\,k\tau)$ when expansion can be neglected. For $w=-1/3$ in a coasting background with constant conformal expansion rate $K$, the exponents are $-K\pm\sqrt{K^2+k^2/3}$. This is a gradient instability, not ordinary positive-pressure [Jeans instability](#jeans-instability). A network with tension or elastic [anisotropic stress](general-relativity.md#anisotropic-stress) needs different constitutive perturbation equations; a negative background [equation of state](thermodynamics.md#equation-of-state) alone does not establish its perturbation sound speed.

### Cosmological adiabatic sound speed

↑ **Parent:** [Cosmological sound speed](#cosmological-sound-speed)

The squared adiabatic sound speed is the ratio of background pressure and energy-density time derivatives. For a [barotropic equation of state](cosmology.md#barotropic-equation-of-state) it is $dP/d\rho$. The [non-adiabatic pressure perturbation](cosmic-inflation.md#non-adiabatic-pressure-perturbation) is the difference $\delta P-c_a^2\delta\rho$; in a general field or multicomponent model this background quantity need not equal the rest-frame propagation speed.

## Suppression of matter growth by smooth accelerated expansion

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

If a smooth component dominates the expansion but does not cluster, pressureless matter still satisfies

$$
\ddot\delta+2H\dot\delta-4\pi G\bar\rho_m\delta=0.
$$

As $\bar\rho_m$ becomes negligible, Hubble friction leaves a constant mode and a decaying mode, so structure growth freezes.

### Matter density modes during cosmological-constant domination

↑ **Parent:** [Suppression of matter growth by smooth accelerated expansion](#suppression-of-matter-growth-by-smooth-accelerated-expansion)

When $H$ is constant and the matter source is negligible,

$$
\ddot\delta_m+2H\dot\delta_m=0,
$$

so $\delta_m=C_1+C_2a^{-2}$. The growing matter-era mode therefore approaches a constant after cosmological-constant domination begins.

#### Bessel density modes during exponential expansion

↑ **Parent:** [Matter density modes during cosmological-constant domination](#matter-density-modes-during-cosmological-constant-domination)

For constant positive [Hubble parameter](cosmology.md#hubble-parameter) $\mu$ and a four-thirds [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state), a [linear cosmological density perturbation](linear-cosmological-density-perturbation.md) obeys $\ddot\delta+2\mu\dot\delta+\eta^2e^{-3\mu t}\delta=0$. Put $\delta=e^{-\mu t}y$ and $x=2|\eta|e^{-3\mu t/2}/(3\mu)$. The resulting [Bessel differential equation](analysis.md#bessel-differential-equation) has order $2/3$; use ordinary [Bessel functions](analysis.md#bessel-function) for $\eta^2>0$ and [modified Bessel functions](analysis.md#modified-bessel-function) for $\eta^2<0$. Their small-$x$ expansions give one constant limiting mode and one $e^{-2\mu t}$ mode. The constant limit need not exceed the initial amplitude without an initial-velocity condition.

##### Monotone Jeans growth with positive cosmological constant

↑ **Parent:** [Bessel density modes during exponential expansion](#bessel-density-modes-during-exponential-expansion)

If $\eta^2=-s^2<0$, $\delta(0)>0$ and $\dot\delta(0)\geq0$, the [integrating factor](differential-equation.md#integrating-factor) identity $(e^{2\mu t}\dot\delta)'=s^2e^{-\mu t}\delta$ proves that $\delta$ stays positive and increases. Its finite limit satisfies $\delta_\infty=\delta(0)+\dot\delta(0)/(2\mu)+s^2\int_0^\infty e^{-3\mu t}\delta(t)dt/(2\mu)>\delta(0)$. The initial sign condition is essential: the positive decaying [modified Bessel function](analysis.md#modified-bessel-function) mode has limit zero.

### Matter growth equation as a function of scale factor

↑ **Parent:** [Suppression of matter growth by smooth accelerated expansion](#suppression-of-matter-growth-by-smooth-accelerated-expansion)

In a matter-plus-cosmological-constant universe, changing the independent variable from cosmic time to $a$ gives

$$
\frac{d^2\delta_m}{da^2}
+\left(\frac{d\log H}{da}+\frac3a\right)\frac{d\delta_m}{da}
-\frac{3\Omega_{m,0}H_0^2}{2a^5H^2}\delta_m=0.
$$

#### Integral linear growth factor in a matter-Lambda universe

↑ **Parent:** [Matter growth equation as a function of scale factor](#matter-growth-equation-as-a-function-of-scale-factor)

The growing solution of the matter perturbation equation in a spatially flat matter-plus-cosmological-constant universe is

$$
D_+(a)=\frac52\Omega_{m,0}H_0^2H(a)
\int_0^a\frac{da'}{a'^3H(a')^3},
$$

normalized so that $D_+(a)\sim a$ during early matter domination.

##### Freezing of linear growth under a positive cosmological constant

↑ **Parent:** [Integral linear growth factor in a matter-Lambda universe](#integral-linear-growth-factor-in-a-matter-lambda-universe)

When $H\to H_\Lambda>0$, the growth [integral](calculus.md#integral) has an integrable $a^{-3}$ tail. Its product with $H$ tends to a constant, with leading correction proportional to $a^{-2}$ in a matter-plus-Lambda background. Both displayed basis functions can tend to constants; a linear combination cancels that constant and isolates the truly decaying late-time $a^{-2}$ behavior.

##### Finite lower limit in the integral matter growth solution

↑ **Parent:** [Integral linear growth factor in a matter-Lambda universe](#integral-linear-growth-factor-in-a-matter-lambda-universe)

Changing the lower limit in $H(a)\int_{a_i}^{a}d\widetilde a/(\widetilde aH)^3$ adds a constant multiple of $H(a)$, the independent matter-era decaying solution. Thus a finite lower limit defines a useful independent solution but can include a decaying admixture. A pure growing normalization is selected by an appropriate linear combination.

##### Galaxy-formation bound on the cosmological constant

↑ **Parent:** [Integral linear growth factor in a matter-Lambda universe](#integral-linear-growth-factor-in-a-matter-lambda-universe)

If a perturbation has amplitude $A\ll1$ at decoupling, it needs a growth factor of at least $A^{-1}$ before cosmological-constant domination freezes its growth. The order-of-magnitude requirement is

$$
\rho_\Lambda\lesssim A^3\rho_m(t_{\rm dec}),
$$

up to the collapse threshold and the gradual transition encoded by the exact growth factor.

## Radiation domination

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

During radiation domination in a flat expanding universe, $a(t)\propto t^{1/2}$ and $H=1/(2t)$.

<h3 id="meszaros-effect">Mészáros effect</h3>

↑ **Parent:** [Radiation domination](#radiation-domination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mészáros_effect)

The Mészáros effect is the suppression of subhorizon cold-dark-matter growth during radiation domination. The growing solution is only logarithmic until matter-radiation equality.

#### Adiabatic radiation-era cold-dark-matter transfer solution

↑ **Parent:** [Mészáros effect](#meszaros-effect)

In a radiation-dominated background with comoving [cold dark matter](cosmology.md#cold-dark-matter), neglect its contribution to gravity but retain the radiation perturbation. The regular [adiabatic initial conditions](cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) select $F(x)=\int_0^x(1-\cos t)dt/t+\sin x/x-(1-\cos x)/x^2-1/2$. It obeys $x^2F^{(4)}+5xF^{(3)}+x^2F''+xF'=0$, with $F\sim x^2/8$ at zero and $F\sim\ln x+\gamma-1/2$ at infinity. The accompanying radiation contrast is $K[-2\cos x+4\sin x/x-4(1-\cos x)/x^2]/3$. This exact leading-radiation solution explains the transition from common superhorizon growth to acoustic radiation oscillations and logarithmic matter growth.

#### Logarithmic CDM growth after radiation-era horizon entry

↑ **Parent:** [Mészáros effect](#meszaros-effect)

After [cosmological horizon entry](#cosmological-horizon-entry) during [radiation domination](#radiation-domination), neglect averaged radiation forcing and the small matter self-gravity term. The [CDM density equation in a matter-radiation universe](#cdm-density-equation-in-a-matter-radiation-universe) becomes $(\tau\delta_C')'=0$, giving the displayed logarithmic solution. Entry at $\tau_h\sim k^{-1}$ matches a superhorizon amplitude of order $A_R/k^2$, fixing the coefficient scale. Detailed radiation forcing near entry determines its order-one numerical factor. This is the [Mészáros effect](#meszaros-effect) for the initially adiabatic mode.

##### Matching the CDM growing mode at horizon entry

↑ **Parent:** [Logarithmic CDM growth after radiation-era horizon entry](#logarithmic-cdm-growth-after-radiation-era-horizon-entry)

In an instantaneous-transition approximation, match the [superhorizon adiabatic CDM mode in radiation domination](#superhorizon-adiabatic-cdm-mode-in-radiation-domination) and its first derivative to the radiation-era logarithmic solution at $\tau_h=1/k$. Its value is $A_R/k^2$ and its derivative is $2A_R/k$. The two matching equations give the displayed expression. Its coefficient two belongs to this approximation; a smooth radiation forcing through entry changes the constants while preserving the [logarithmic CDM growth after radiation-era horizon entry](#logarithmic-cdm-growth-after-radiation-era-horizon-entry) scaling.

<h4 id="meszaros-equation">Mészáros equation</h4>

↑ **Parent:** [Mészáros effect](#meszaros-effect)

In a flat universe containing [pressureless matter](cosmology.md#pressureless-matter) and smooth [radiation in cosmology](cosmology.md#radiation-in-cosmology), put $y=a/a_{\rm eq}$ and $C=H_0^2\Omega_{m,0}^2/\Omega_{r,0}$. The [Friedmann equation](cosmology.md#friedmann-equations) gives $\mathcal H^2=C(1+y)/y^2$, so $y'^2=C(1+y)$ and $y''=C/2$. The subhorizon [cosmological Poisson equation](linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) gives $\delta''+\mathcal H\delta'=3C\delta/(2y)$. The [chain rule](calculus.md#chain-rule) produces the displayed equation. Smoothing radiation neglects its rapid acoustic forcing after horizon entry; it is not an exact treatment of all radiation perturbations.

<h5 id="meszaros-equation-solution-basis">Mészáros equation solution basis</h5>

↑ **Parent:** [Mészáros equation](#meszaros-equation)

A [basis](vector-space.md#basis) of the [solution space of a homogeneous linear differential equation](differential-equation.md#solution-space-of-a-homogeneous-linear-differential-equation) for the [Mészáros equation](#meszaros-equation) on $y>0$ is

$$
D_+=1+\frac32y,\qquad
D_-=\left(1+\frac32y\right)\log\frac{\sqrt{1+y}+1}{\sqrt{1+y}-1}-3\sqrt{1+y}.
$$

Substitution verifies both solutions; their [Wronskian](differential-equation.md#wronskian) is $-1/[y\sqrt{1+y}]$, so they are independent. At small $y$, $D_+=1+O(y)$ and $D_-=\log(4/y)-3+O(y\log y)$. At large $y$, $D_+\sim3y/2$ and $D_-\sim4/(15y^{3/2})$. Matching the actual early-time radiation forcing determines which constant and logarithmic combination is excited.

## Matter domination

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

During matter domination in a spatially flat universe, pressureless matter controls the expansion, $a(t)\propto t^{2/3}$, and the growing linear density mode is proportional to $a$.

## Matter-era growing and decaying density modes

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

During [matter domination](#matter-domination) in a flat [FLRW metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric), the [cosmological continuity equation](cosmology.md#cosmological-continuity-equation) gives $\rho\propto a^{-3}$, and the [Friedmann equation](cosmology.md#friedmann-equations) gives $a\propto\tau^2$ and $8\pi G\rho a^2=12/\tau^2$. The [CDM density equation in a matter-radiation universe](#cdm-density-equation-in-a-matter-radiation-universe), with radiation neglected, is therefore $\delta''+2\delta'/\tau-6\delta/\tau^2=0$. Its [Euler-Cauchy equation](differential-equation.md#euler-cauchy-equation) powers satisfy $(p-2)(p+3)=0$, proving the displayed general solution. The growing [density contrast](#density-contrast) is proportional to the [scale factor](cosmology.md#scale-factor-cosmology), while the decaying mode is proportional to $a^{-3/2}$. This all-scale form uses the CDM-comoving [synchronous gauge](linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology); other density slices require their corresponding gauge transformation.

### Cosmic-time matter density modes

↑ **Parent:** [Matter-era growing and decaying density modes](#matter-era-growing-and-decaying-density-modes)

In cosmic time during matter domination, $a(t)\propto t^{2/3}$ and the pressureless density contrast obeys

$$
\ddot\delta+\frac4{3t}\dot\delta-\frac2{3t^2}\delta=0.
$$

Its growing and decaying solutions are $t^{2/3}$ and $t^{-1}$.

### Matter-era linear growth factor

↑ **Parent:** [Matter-era growing and decaying density modes](#matter-era-growing-and-decaying-density-modes)

After neglecting the decaying mode, the linear growth between conformal times $\tau_1$ and $\tau_2$ is

$$
D(\tau_2,\tau_1)=\frac{a(\tau_2)}{a(\tau_1)}
=\left(\frac{\tau_2}{\tau_1}\right)^2.
$$

## Cosmological horizon crossing

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)

A mode of comoving wavenumber $k$ and physical wavelength $2\pi a/k$ crosses a conformal horizon of physical size $ac\tau$ when

$$
\tau_H=\frac{2\pi}{kc}.
$$

### Cosmological horizon entry

↑ **Parent:** [Cosmological horizon crossing](#cosmological-horizon-crossing)

During a decelerating expansion the [comoving Hubble radius](cosmology.md#comoving-hubble-radius) grows. A fixed comoving [wavenumber](wave-equation.md#wavenumber) then passes from a [superhorizon scale](cosmic-inflation.md#superhorizon-scale) to a shorter scale when $k\simeq aH$. In [radiation domination](#radiation-domination), $aH=1/\tau$, so this occurs at $k\tau\simeq1$. Here horizon entry refers to [Hubble radius](cosmology.md#hubble-radius) crossing; a true causal horizon instead depends on a conformal-time integral.

### Horizon-crossing time across matter-radiation equality

↑ **Parent:** [Cosmological horizon crossing](#cosmological-horizon-crossing)

With $a(t_0)=1$, $k_0=2\pi/(ct_0)$, and $1+z_{\rm eq}=(t_0/t_{\rm eq})^{2/3}$,

$$
\frac{t_H}{t_0}\simeq
\begin{cases}
(k_0/k)^3,&t_H>t_{\rm eq},\\
(1+z_{\rm eq})^{-1/2}(k_0/k)^2,&t_H<t_{\rm eq}.
\end{cases}
$$

### Matter-era transfer of a horizon-crossing amplitude

↑ **Parent:** [Cosmological horizon crossing](#cosmological-horizon-crossing)

A mode crossing during matter domination acquires the growth factor $(\tau_0/\tau_H)^2$. An initial amplitude proportional to $\tau_H^2k^{1/2}$ therefore becomes proportional to $k^{1/2}$ today.

## Matter power spectrum

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matter_power_spectrum)

The density power spectrum records the squared Fourier-mode amplitude, up to the chosen statistical normalization. Scale dependence acquired from primordial amplitudes and subsequent growth determines its spectral shape.

### Eight-megaparsec density fluctuation amplitude

↑ **Parent:** [Matter power spectrum](#matter-power-spectrum)

The parameter $\sigma_8$ is the present linear rms [density contrast](#density-contrast) averaged in a spherical top-hat of comoving radius $8h^{-1}\,\mathrm{Mpc}$, with $h=H_0/(100\,\mathrm{km\,s^{-1}\,Mpc^{-1}})$. Thus $\sigma_8^2=(2\pi^2)^{-1}\int_0^\infty k^2P_m(k,0)|W(kR_8)|^2\,dk$. It specifies an amplitude on a chosen scale rather than the complete [matter power spectrum](#matter-power-spectrum); converting cluster abundance into this parameter also requires a spectral shape and background cosmology.

### Potential fluctuations per logarithmic wavenumber

↑ **Parent:** [Matter power spectrum](#matter-power-spectrum)

For $P_\delta(k)=Ak^n$, the [cosmological Poisson equation](linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) gives $P_\varphi(k)=(4\pi Ga^2\bar\rho)^2P_\delta(k)/k^4$. The contribution to variance per logarithmic [wavenumber](wave-equation.md#wavenumber) is $k^3P_\varphi(k)/(2\pi^2)$, giving the displayed expression and rms scaling $\varphi_{\rm rms}(R)\propto R^{(1-n)/2}$ for a band around $k\sim R^{-1}$. The [Harrison-Zeldovich spectrum](#harrison-peebles-zeldovich-spectrum) $n=1$ has equal potential variance per logarithmic interval. An uncut power law over all scales has divergent total potential variance for every $n$, so the scale-local amplitude must not be confused with a finite global rms.

### Band-limited linear density correlation

↑ **Parent:** [Matter power spectrum](#matter-power-spectrum)

For an isotropic [matter power spectrum](#matter-power-spectrum) $P(k)=Ak$ on $0\leq k\leq k_{\max}$ and zero elsewhere, put $K=k_{\max}r$. Angular integration of the [Fourier transform](analysis.md#fourier-transform) gives $\xi(r)=A(2\pi^2r)^{-1}\int_0^{k_{\max}}k^2\sin(kr)\,dk$, and two integrations by parts yield the displayed answer. Its apparent origin singularity is removable, with $\xi(0)=Ak_{\max}^4/(8\pi^2)$. The sharp cutoff creates oscillatory, including negative, correlations without violating positivity of the spectrum.

### Scale-free density correlation transform

↑ **Parent:** [Matter power spectrum](#matter-power-spectrum)

For a statistically isotropic three-dimensional [matter power spectrum](#matter-power-spectrum) $\mathcal P(k)=Ak^n$, the [Fourier transform](analysis.md#fourier-transform) gives $\xi(r)=A(2\pi^2)^{-1}r^{-n-3}\int_0^\infty u^{n+1}\sin u\,du$. The [improper integral](real-analysis.md#improper-integral) converges at zero precisely when $n>-3$ and at infinity when $n<-1$; it is absolutely convergent only when $n<-2$. Within this range its positive coefficient is $\Gamma(n+2)\sin[\pi(n+2)/2]$, interpreted continuously as $\pi/2$ at $n=-2$. Outside this range, cutoffs, smoothing or an explicitly stated distributional interpretation are necessary; dimensional scaling alone does not establish an ordinary positive power-law [correlation function](critical-phenomenon.md#correlation-function).

### Harrison-Peebles-Zeldovich spectrum

↑ **Parent:** [Matter power spectrum](#matter-power-spectrum)

The Harrison-Peebles-Zeldovich spectrum is the scale-invariant primordial growing-mode spectrum: in a fixed [conformal time](cosmology.md#conformal-time) slice before [cosmological horizon crossing](#cosmological-horizon-crossing), the [matter power spectrum](#matter-power-spectrum) is proportional to $\tau^4k$ in the usual growing-mode density convention. At horizon entry $\tau_H\sim k^{-1}$, its dimensionless mass [variance](variance.md) $k^3P(k,\tau_H)$ is independent of $k$. This statement fixes a spectral shape, not its amplitude. [Radiation domination](#radiation-domination) subsequently suppresses small-scale density growth through the [Mészáros effect](#meszaros-effect), producing the asymptotic [matter power spectrum](#matter-power-spectrum) $P\propto k^{-3}\ln^2(k/k_{\rm eq})$ after [matter-radiation equality](cosmology.md#matter-radiation-equality).

#### Gaussian horizon-crossing variance for a Harrison-Zeldovich spectrum

↑ **Parent:** [Harrison-Peebles-Zeldovich spectrum](#harrison-peebles-zeldovich-spectrum)

For the growing matter-era spectrum $P(k,\tau)=Ak(\tau/\tau_{\rm eq})^4$ and Gaussian Fourier window $W(kr)=e^{-(kr)^2/2}$, integration gives the displayed [smoothed matter density variance](#smoothed-matter-density-variance). A physical Hubble-radius window has $r=1/(aH)=\tau/2$, making its variance independent of crossing time. The dimensionless mode variance $k^3P/(2\pi^2)$ is likewise constant at $k\tau=2$. A pure $P\propto k$ spectrum needs ultraviolet-convergent smoothing: a real-space top-hat alone leaves a logarithmic divergence.

// Target: cosmology.bigb

### Broken matter power spectrum from horizon entry

↑ **Parent:** [Matter power spectrum](#matter-power-spectrum)

If primordial horizon-crossing perturbations satisfy $V\langle|\delta_k|^2\rangle=C/k^3$, remain frozen during radiation domination, and grow as $a$ during matter domination, then

$$
P(k)=
\begin{cases}
Ck/k_0^4,&k<k_{\rm eq},\\
Ck_{\rm eq}^4/(k^3k_0^4),&k>k_{\rm eq}.
\end{cases}
$$

## Neutrino free streaming

↑ **Parent:** [Linear cosmological density perturbation](linear-cosmological-density-perturbation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neutrino_free_streaming)

Neutrino free streaming transports neutrinos out of small-scale overdensities. Massive neutrinos therefore contribute to the homogeneous matter density while clustering inefficiently below their free-streaming scale, slowing the growth of cold-matter perturbations.

### Neutrino Boltzmann hierarchy

↑ **Parent:** [Neutrino free streaming](#neutrino-free-streaming)

For massless collisionless [neutrinos](standard-model.md#neutrino) in [Newtonian gauge in cosmology](linear-cosmological-perturbation-theory.md#newtonian-gauge), expand their temperature fluctuation as $\Theta(\mu)=\sum_{\ell\ge0}(-i)^\ell\Theta_\ell P_\ell(\mu)$, without a $(2\ell+1)$ factor. The [Legendre polynomial recurrence relation](differential-equation.md#legendre-polynomial-recurrence-relation) gives

$$
\dot\Theta_\ell+k\left(\frac{\ell+1}{2\ell+3}\Theta_{\ell+1}-\frac{\ell}{2\ell-1}\Theta_{\ell-1}\right)=\delta_{\ell0}\dot\phi+\delta_{\ell1}k\psi.
$$

The lower-neighbour term is absent at $\ell=0$. Multipoles with the more usual $(2\ell+1)$ weighting equal $\Theta_\ell/(2\ell+1)$.

## ↑ Ancestors (4)

1. [Cosmology](cosmology.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (18)

- [Bessel density modes during exponential expansion](#bessel-density-modes-during-exponential-expansion)
- [Einstein-de Sitter density-growth modes](#einstein-de-sitter-density-growth-modes)
- [Expansion-weighted derivative of a passive density perturbation](#expansion-weighted-derivative-of-a-passive-density-perturbation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-60.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#8c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-310.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4.md#9b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-346.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-312.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-310.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-310.md#3/a/solution)
- [Structure formation](cosmology.md#structure-formation)
