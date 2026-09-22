# Classical field-theory soliton

↑ **Parent:** [Quantum field theory](quantum-field-theory.md)

A classical field-theory soliton is a smooth, localized finite-energy solution that behaves as a persistent object. Stability may follow from a [topological charge](#topological-charge) or from a balance among energy terms with different scaling behavior.

**Table of contents**

- [Non-topological soliton](#non-topological-soliton)
  - [Q-ball](#q-ball)
    - [Sextic unique-vacuum Q-ball potential](#sextic-unique-vacuum-q-ball-potential)
    - [Lorentz boost of a Q-ball](#lorentz-boost-of-a-q-ball)
    - [Charge-constrained scalar-field scaling](#charge-constrained-scalar-field-scaling)
- [Breather](#breather)
- [Semiclassical soliton mass](#semiclassical-soliton-mass)
  - [One-loop soliton mass correction](#one-loop-soliton-mass-correction)
    - [Mode-number regularization of soliton masses](#mode-number-regularization-of-soliton-masses)
      - [Cutoff surface term for a Sine-Gordon kink](#cutoff-surface-term-for-a-sine-gordon-kink)
- [Vacuum-subtracted soliton mass](#vacuum-subtracted-soliton-mass)
- [Soliton time delay](#soliton-time-delay)
  - [Full S-matrix phase from a classical soliton delay](#full-s-matrix-phase-from-a-classical-soliton-delay)
  - [Pairwise additivity of soliton shifts](#pairwise-additivity-of-soliton-shifts)
- [Finite-energy field configuration](#finite-energy-field-configuration)
  - [Finite sigma-model energy need not give a limit at infinity](#finite-sigma-model-energy-need-not-give-a-limit-at-infinity)
- [Collective coordinate of a soliton](#collective-coordinate-of-a-soliton)
  - [Quantization of a periodic soliton coordinate](#quantization-of-a-periodic-soliton-coordinate)
  - [Collective-coordinate effective Lagrangian for a soliton](#collective-coordinate-effective-lagrangian-for-a-soliton)
    - [Instantaneous-boost effective action for a sine-Gordon kink](#instantaneous-boost-effective-action-for-a-sine-gordon-kink)
      - [Acceleration correction for an instantaneous boosted kink](#acceleration-correction-for-an-instantaneous-boosted-kink)
  - [Moduli-space approximation for solitons](#moduli-space-approximation-for-solitons)
    - [Collective-coordinate quantization](#collective-coordinate-quantization)
- [Topological charge](#topological-charge)
  - [Vacuum-boundary degree as a defect charge](#vacuum-boundary-degree-as-a-defect-charge)
  - [Degree and energetic stability of a field configuration](#degree-and-energetic-stability-of-a-field-configuration)
  - [Topological current](#topological-current)
    - [Pullback-volume representation of a topological current](#pullback-volume-representation-of-a-topological-current)
  - [Topological sector](#topological-sector)
- [Bright soliton of the focusing nonlinear Schrödinger equation](#bright-soliton-of-the-focusing-nonlinear-schrodinger-equation)
  - [Harmonic-trap translation of a nonlinear Schrödinger soliton](#harmonic-trap-translation-of-a-nonlinear-schrodinger-soliton)
  - [Galilean boost of a nonlinear Schrödinger soliton](#galilean-boost-of-a-nonlinear-schrodinger-soliton)
- [Derrick's theorem](#derrick-s-theorem)
  - [Two-dimensional flat-target Derrick obstruction](#two-dimensional-flat-target-derrick-obstruction)
  - [Derrick scaling](#derrick-scaling)
    - [No static finite-energy lump in three-dimensional pure Yang-Mills theory](#no-static-finite-energy-lump-in-three-dimensional-pure-yang-mills-theory)
    - [Derrick scaling of Yang-Mills-Higgs energy](#derrick-scaling-of-yang-mills-higgs-energy)
  - [Derrick virial identity](#derrick-virial-identity)
- [Scalar-field kink](#scalar-field-kink)
  - [Antikink](#antikink)
  - [Phi-four kink](#phi-four-kink)
    - [Relativistic energy and momentum of a phi-four kink](#relativistic-energy-and-momentum-of-a-phi-four-kink)
    - [Kink–antikink attraction from the stress tensor](#kink-antikink-attraction-from-the-stress-tensor)
      - [At-rest force for a symmetric phi-four pair](#at-rest-force-for-a-symmetric-phi-four-pair)
    - [Fluctuation operator of a phi-four kink](#fluctuation-operator-of-a-phi-four-kink)
    - [Translational dynamics of a phi-four kink](#translational-dynamics-of-a-phi-four-kink)
  - [Kink in a phi-six model](#kink-in-a-phi-six-model)
    - [Bogomolny classification of a rescaled phi-six kink](#bogomolny-classification-of-a-rescaled-phi-six-kink)
    - [Intermediate-vacuum obstruction to a kink](#intermediate-vacuum-obstruction-to-a-kink)
- [Gauge-theory soliton](#gauge-theory-soliton)
  - ['t Hooft-Polyakov monopole](#t-hooft-polyakov-monopole)
  - [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole)
    - [Higgs norm identity for a Bogomolny monopole](#higgs-norm-identity-for-a-bogomolny-monopole)
    - [Bogomolny monopole equations imply Yang-Mills-Higgs equations](#bogomolny-monopole-equations-imply-yang-mills-higgs-equations)
    - [Hedgehog ansatz for a monopole](#hedgehog-ansatz-for-a-monopole)
      - [Prasad-Sommerfield radial monopole solution](#prasad-sommerfield-radial-monopole-solution)
      - [Hedgehog monopole equations in radial profile variables](#hedgehog-monopole-equations-in-radial-profile-variables)
  - [Abelian Higgs model](#abelian-higgs-model)
    - [Broken-phase spectrum of the Abelian Higgs model](#broken-phase-spectrum-of-the-abelian-higgs-model)
    - [Derrick scaling of the Abelian Higgs energy](#derrick-scaling-of-the-abelian-higgs-energy)
    - [Inverse-density Abelian Higgs model](#inverse-density-abelian-higgs-model)
      - [Logarithmic equation for inverse-density Abelian Higgs vortices](#logarithmic-equation-for-inverse-density-abelian-higgs-vortices)
      - [Bogomolny bound for the inverse-density Abelian Higgs model](#bogomolny-bound-for-the-inverse-density-abelian-higgs-model)
    - [Critically coupled Abelian Higgs field equations](#critically-coupled-abelian-higgs-field-equations)
    - [Nielsen-Olesen vortex](#nielsen-olesen-vortex)
      - [Compact-core variational estimate for an Abelian Higgs vortex](#compact-core-variational-estimate-for-an-abelian-higgs-vortex)
      - [Magnetic flux quantization of an Abelian Higgs vortex](#magnetic-flux-quantization-of-an-abelian-higgs-vortex)
      - [Vortex number](#vortex-number)
      - [Abelian Higgs vortex moduli space](#abelian-higgs-vortex-moduli-space)
        - [Relative coordinate for two identical vortices](#relative-coordinate-for-two-identical-vortices)
        - [Right-angle scattering of Abelian Higgs vortices](#right-angle-scattering-of-abelian-higgs-vortices)
      - [Bogomolny vortex equation](#bogomolny-vortex-equation)
        - [Logarithmic form of a Bogomolny vortex](#logarithmic-form-of-a-bogomolny-vortex)
        - [Bogomolny square completion for an Abelian Higgs vortex](#bogomolny-square-completion-for-an-abelian-higgs-vortex)
          - [Conformal-surface vortex square completion](#conformal-surface-vortex-square-completion)
        - [Taubes equation](#taubes-equation)
          - [Prescribed-zero construction of planar Abelian Higgs vortices](#prescribed-zero-construction-of-planar-abelian-higgs-vortices)
          - [Vortex composition by conformal rescaling](#vortex-composition-by-conformal-rescaling)
          - [Bradlow bound](#bradlow-bound)
        - [Hyperbolic vortex](#hyperbolic-vortex)
          - [Hyperbolic one-vortex at curvature minus one half](#hyperbolic-one-vortex-at-curvature-minus-one-half)
          - [Witten hyperbolic vortex](#witten-hyperbolic-vortex)
  - [Yang-Mills instanton](#yang-mills-instanton)
    - [Theta-weighted instanton sectors](#theta-weighted-instanton-sectors)
    - [ADHM construction](#adhm-construction)
      - [ADHM factorization identity](#adhm-factorization-identity)
    - [BPST instanton](#bpst-instanton)
    - [Finite Yang-Mills action forbids nontrivial translation symmetry](#finite-yang-mills-action-forbids-nontrivial-translation-symmetry)
    - [Boundary winding representation of Yang-Mills topological charge](#boundary-winding-representation-of-yang-mills-topological-charge)
    - [Instanton moduli space](#instanton-moduli-space)
      - [Instanton size modulus](#instanton-size-modulus)
      - [Framed instanton moduli space](#framed-instanton-moduli-space)
    - [Self-duality implies Yang-Mills equations](#self-duality-implies-yang-mills-equations)
    - [Self-dual Yang-Mills equations](#self-dual-yang-mills-equations)
      - [Self-duality of gauge curvature](#self-duality-of-gauge-curvature)
      - [Self-dual Yang-Mills equations in temporal gauge](#self-dual-yang-mills-equations-in-temporal-gauge)
    - [Yang-Mills instanton Bogomolny bound](#yang-mills-instanton-bogomolny-bound)
    - [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations)
      - [Anti-self-duality of gauge curvature](#anti-self-duality-of-gauge-curvature)
      - [Complex potential reduction of anti-self-dual Yang-Mills](#complex-potential-reduction-of-anti-self-dual-yang-mills)
      - [Anti-self-dual Yang-Mills equations in temporal gauge](#anti-self-dual-yang-mills-equations-in-temporal-gauge)
        - [Nahm equations](#nahm-equations)
          - [Polynomial Lax representation of the Nahm equations](#polynomial-lax-representation-of-the-nahm-equations)
    - [Instanton number](#instanton-number)
      - [Instanton number as a winding number at infinity](#instanton-number-as-a-winding-number-at-infinity)
    - [Dimensional reduction of a Yang-Mills instanton to a monopole](#dimensional-reduction-of-a-yang-mills-instanton-to-a-monopole)
      - [Orientation of a monopole lift](#orientation-of-a-monopole-lift)
- [Skyrme model](#skyrme-model)
  - [Derrick dimension test for the Skyrme model](#derrick-dimension-test-for-the-skyrme-model)
    - [Commuting-current obstruction in a two-dimensional Skyrme model](#commuting-current-obstruction-in-a-two-dimensional-skyrme-model)
  - [Skyrme term](#skyrme-term)
  - [Vacuum-preserving symmetry of the Skyrme model](#vacuum-preserving-symmetry-of-the-skyrme-model)
  - [Skyrmion](#skyrmion)
    - [Skyrmion model of a nucleus](#skyrmion-model-of-a-nucleus)
    - [Skyrmion stabilizer and collective-coordinate orbit](#skyrmion-stabilizer-and-collective-coordinate-orbit)
    - [Cubic four-Skyrmion](#cubic-four-skyrmion)
    - [Tetrahedral three-Skyrmion](#tetrahedral-three-skyrmion)
    - [Toroidal two-Skyrmion](#toroidal-two-skyrmion)
    - [Topological baryon number in the Skyrme model](#topological-baryon-number-in-the-skyrme-model)
      - [Skyrme baryon number as a mapping degree](#skyrme-baryon-number-as-a-mapping-degree)
      - [Skyrme baryon density](#skyrme-baryon-density)
    - [Skyrmion hedgehog ansatz](#skyrmion-hedgehog-ansatz)
      - [Rotational quantization of a unit Skyrmion](#rotational-quantization-of-a-unit-skyrmion)
    - [Rational map approximation for Skyrmions](#rational-map-approximation-for-skyrmions)
      - [Cubic rational-map ansatz for four Skyrmions](#cubic-rational-map-ansatz-for-four-skyrmions)
      - [Angular integral in the rational map approximation](#angular-integral-in-the-rational-map-approximation)
    - [Finkelstein-Rubinstein constraints](#finkelstein-rubinstein-constraints)
      - [Collective-rotation constraints for a Skyrmion](#collective-rotation-constraints-for-a-skyrmion)

## Non-topological soliton

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-topological_soliton)

A [non-topological soliton](#non-topological-soliton) is a localized finite-energy field configuration whose existence or stability is not protected by a nontrivial [topological charge](#topological-charge). A conserved ordinary [Noether charge](quantum-field-theory.md#noether-charge) can instead obstruct its decay. A [Q-ball](#q-ball) is a standard complex-scalar example: its profile is localized while its phase rotates in time.

### Q-ball

↑ **Parent:** [Non-topological soliton](#non-topological-soliton)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Q-ball)

For a [complex scalar field](scalar-field-theory.md#complex-scalar-field) with global $U(1)$ invariance and Lagrangian $\mathcal L=\tfrac12|\partial_t\phi|^2-\tfrac12|\nabla\phi|^2-U(|\phi|)$, a [Q-ball](#q-ball) is a localized phase-rotating configuration with conserved [Noether charge](quantum-field-theory.md#noether-charge) $Q=\int\operatorname{Im}(\bar\phi\phi_t)$. At fixed charge its real profile can minimize

$$
E_Q[f]=\int\left(\frac12|\nabla f|^2+U(f)\right)+
\frac{Q^2}{2\int f^2}.
$$

Such solutions require a suitable potential and charge range; the complex nature of a field alone does not ensure existence. A common condition is $\inf_{f>0}2U(f)/f^2<U''(0)$.

#### Sextic unique-vacuum Q-ball potential

↑ **Parent:** [Q-ball](#q-ball)

This nonnegative potential has its only vacuum at $s=0$, since $U(s)=s[(s-1/2)^2+3/4]$. For the complex kinetic normalization $\tfrac12|\partial\phi|^2$, the small-amplitude mass squared is $2U'(0)=2$, whereas $\min_{s>0}2U(s)/s=3/2$. The radial [Q-ball](#q-ball) equation has a positive localized profile for frequencies $3/2<\omega^2<2$, for example in three spatial dimensions. It is a standard non-topological soliton potential: the effective profile potential $U(f^2)-\omega^2f^2/2$ is negative somewhere, while its quadratic coefficient near zero is positive. The conserved [Noether charge](quantum-field-theory.md#noether-charge), not vacuum winding, supplies the stabilization mechanism.

#### Lorentz boost of a Q-ball

↑ **Parent:** [Q-ball](#q-ball)

For a one-dimensional [Q-ball](#q-ball), the profile equation gives $\tfrac12(f')^2=U(f)-\tfrac12\omega^2f^2$. Its rest energy is therefore $M=\int[(f')^2+\omega^2f^2]$. A [Lorentz transformation](special-relativity.md#lorentz-transformation) replaces the rest coordinates by $\tau=\gamma(t-v(x-x_0))$, $\xi=\gamma(x-x_0-vt)$. The scalar solution $e^{i\omega\tau}f(\xi)$ has energy $\int[\tfrac12|\phi_t|^2+\tfrac12|\phi_x|^2+U]$ and momentum $-\int\operatorname{Re}(\bar\phi_t\phi_x)$. Substitution and $dx=d\xi/\gamma$ give the displayed values and $E^2-P^2=M^2$.

#### Charge-constrained scalar-field scaling

↑ **Parent:** [Q-ball](#q-ball)

For $f_\lambda(x)=f(\lambda x)$ in $d$ space dimensions, write $T=\tfrac12\int|\nabla f|^2$, $W=\int U(f)$ and $I=\int f^2$. Eliminating the rotation frequency by $\omega=Q/I$ gives the displayed fixed-charge scaling. The positive-power charge term can balance the gradient and potential terms even for $d\ge3$. This evades the static [Derrick theorem](#derrick-s-theorem) because the field is time-dependent and the relevant variations preserve its [Noether charge](quantum-field-theory.md#noether-charge).

## Breather

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

A [breather](#breather) is a spatially localized nonlinear-wave solution periodic in time. It does not separate into independently traveling lumps while it breathes. A [Sine-Gordon breather](integrable-systems.md#sine-gordon-breather) arises from a complex-conjugate soliton pair. In the quantum sine-Gordon model, the associated neutral kink-antikink bound particles are also called [breathers](#breather).

## Semiclassical soliton mass

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

A weak-coupling expansion of a [vacuum-subtracted soliton mass](#vacuum-subtracted-soliton-mass) begins with the classical energy and adds the [Gaussian fluctuation approximation](perturbative-quantum-field-theory.md#gaussian-fluctuation-approximation). For [Sine-Gordon theory](scalar-field-theory.md#sine-gordon-theory), $M=8m/\beta^2+\Delta M_{1\mathrm{loop}}+O(m\beta^2)$. The term of order $m$ includes both the vacuum-subtracted fluctuation frequencies and the appropriate [mass counterterm](perturbative-quantum-field-theory.md#mass-counterterm).

### One-loop soliton mass correction

↑ **Parent:** [Semiclassical soliton mass](#semiclassical-soliton-mass)

In a common finite-volume [regularization in quantum field theory](perturbative-quantum-field-theory.md#regularization-in-quantum-field-theory), the oscillator contribution is $\Delta M_{\rm osc}=\tfrac12\sum_n(\Omega_n-\Omega_n^{(0)})$, including every discrete and continuum-derived mode and treating translation as a [collective coordinate](#collective-coordinate-of-a-soliton). Physical frequencies are $\Omega_n=m\omega_n$ when coordinates are measured in units of $m^{-1}$. A [mass counterterm](perturbative-quantum-field-theory.md#mass-counterterm) is added only afterwards. The vacuum subtraction removes the extensive [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy) but can leave an [ultraviolet divergence](perturbative-quantum-field-theory.md#ultraviolet-divergence).

#### Mode-number regularization of soliton masses

↑ **Parent:** [One-loop soliton mass correction](#one-loop-soliton-mass-correction)

Compare the same total number of finite-box modes in the [soliton](integrable-systems.md#soliton) and vacuum sectors before removing the [ultraviolet cutoff](quantum-field-theory.md#ultraviolet-cutoff). A localized [bound state](quantum-mechanics.md#bound-state) replaces a continuum mode, and its contribution must be retained. For the [Sine-Gordon kink fluctuation operator](scalar-field-theory.md#sine-gordon-kink-fluctuation-operator) and the odd phase branch $\delta(k)=2\arctan(1/k)$, the bound translation mode replaces the free $k=0$ oscillator. Thus the complete oscillator correction is $-m/2-(m/2)\int dk\,\delta(k)k/[2\pi\sqrt{k^2+1}]$ in this convention. The continuum integral alone misses the finite $-m/2$ contribution.

##### Cutoff surface term for a Sine-Gordon kink

↑ **Parent:** [Mode-number regularization of soliton masses](#mode-number-regularization-of-soliton-masses)

The [scattering phase shift](quantum-mechanics.md#scattering-phase-shift) $\delta(k)=2\arctan(m/k)$ of the [Sine-Gordon kink fluctuation operator](scalar-field-theory.md#sine-gordon-kink-fluctuation-operator) gives a continuum frequency sum. In [mode-number regularization of soliton masses](#mode-number-regularization-of-soliton-masses), the zero-frequency translation mode replaces the vacuum oscillator at $k=0$. The bare difference is $-m/2-(2\pi)^{-1}\int_0^\Lambda\delta(k)k/\sqrt{k^2+m^2}\,dk$. Integration by parts cancels the lower endpoint against $-m/2$ and produces the displayed upper surface term. Although $\delta(\Lambda)$ vanishes, its product with $\omega(\Lambda)$ tends to $2m$. Vacuum [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) cancels the logarithmic bulk [ultraviolet divergence](perturbative-quantum-field-theory.md#ultraviolet-divergence), leaving this finite [one-loop soliton mass correction](#one-loop-soliton-mass-correction). Parameters and finite [counterterms](perturbative-quantum-field-theory.md#counterterm) must be fixed by a stated [renormalization condition](perturbative-quantum-field-theory.md#renormalization-condition).

## Vacuum-subtracted soliton mass

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

The rest mass of a stable [soliton](integrable-systems.md#soliton) is the lowest energy in its [topological sector](#topological-sector) minus the vacuum energy, in the infinite-volume limit. If Euclidean kernels $K_Q(\tau)$ have nonzero overlap with the sector's lowest-energy states, then $M=-\lim_{\tau\to\infty}\tau^{-1}\log[K_1(\tau)/K_0(\tau)]$, followed by the infinite-volume limit. A [Euclidean path integral](quantum-field-theory.md#euclidean-path-integral) represents these kernels, with boundary wavefunctionals included if necessary.

## Soliton time delay

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

If a labeled [soliton](integrable-systems.md#soliton) approaches $x=vt+a_-$ before a collision and $x=vt+a_+$ afterwards, its spatial shift is $\Delta x=a_+-a_-$. For $v\ne0$, define its time delay at a fixed spatial point by $\Delta t=-\Delta x/v$. Thus a positive forward shift of a right-moving [soliton](integrable-systems.md#soliton) is a negative time delay. For a stationary [soliton](integrable-systems.md#soliton), the spatial shift is well defined but this time-delay definition is not.

### Full S-matrix phase from a classical soliton delay

↑ **Parent:** [Soliton time delay](#soliton-time-delay)

A narrow outgoing energy packet has phase $-ET/\hbar+\delta(E)$, so [stationary phase](analysis.md#stationary-phase-method) gives the arrival shift $\Delta T=\hbar\delta'(E)$. For two equal-mass [solitons](integrable-systems.md#soliton) with relative [rapidity](special-relativity.md#rapidity) $\theta$, $E=2\mathcal M\cosh(\theta/2)$. The convention $S=e^{2i\delta_{\rm pw}}$ instead gives $2\hbar\delta_{\rm pw}'=\Delta T$. Classical time delays determine only the energy-dependent phase difference, not its constant branch.

### Pairwise additivity of soliton shifts

↑ **Parent:** [Soliton time delay](#soliton-time-delay)

A many-[soliton](integrable-systems.md#soliton) spatial shift is pairwise additive when $\Delta x_i=\sum_{j\ne i}\Delta x_{i|j}$. In the all-[kink](#scalar-field-kink) sector of [Sine-Gordon theory](scalar-field-theory.md#sine-gordon-theory), $\Delta x_{i|j}=-\operatorname{sgn}(v_i-v_j)\log\tanh^2[(\theta_i-\theta_j)/2]/\cosh\theta_i$. Dominant spectator exponentials in the [Sine-Gordon multisoliton tau representation](scalar-field-theory.md#sine-gordon-multisoliton-tau-representation) multiply the effective exponential of [kink](#scalar-field-kink) $i$, so their logarithms add. This is a classical signature of [factorized scattering](quantum-field-theory.md#factorized-scattering), with no independent many-body contribution to the asymptotic shift.

## Finite-energy field configuration

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

A finite-energy field configuration has integrable [energy density](statistical-physics.md#energy-density) after the vacuum energy has been subtracted. The boundary conditions used for a localized [classical field-theory soliton](classical-field-theory-soliton.md) require approaching a vacuum at spatial infinity. In one dimension the two ends may approach distinct [scalar-field vacua](quantum-field-theory.md#scalar-field-vacuum); in a gauge theory the asymptotic field can have nontrivial winding even when its local energy density tends to zero.

### Finite sigma-model energy need not give a limit at infinity

↑ **Parent:** [Finite-energy field configuration](#finite-energy-field-configuration)

For arbitrary maps $\phi:\mathbb R^2\to S^2$, integrability of the Dirichlet [energy](classical-mechanics.md#energy) does not imply continuous extension to the [one-point compactification](topology.md#alexandroff-extension). For large $r$, take

$$
\phi(r,\vartheta)=(\sin a(r),0,\cos a(r)),\qquad a(r)=\log\log r,
$$

and interpolate smoothly to a constant on a bounded disk. Its exterior [energy](classical-mechanics.md#energy) is

$$
\frac12\int_{|x|\geq R}|\nabla\phi|^2\,d^2x
=\pi\int_R^\infty\frac{dr}{r\log^2r}=\frac{\pi}{\log R}<\infty.
$$

The field has no limit because $a(r)$ keeps winding. A continuous extension at the point at infinity instead requires $\phi(x)\to\phi_\infty$ uniformly outside sufficiently large disks. This fixed-limit boundary condition is standard for a [sigma-model lump](quantum-field-theory.md#sigma-model-lump), but is extra information beyond finite [energy](classical-mechanics.md#energy) for arbitrary fields.

## Collective coordinate of a soliton

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

A collective coordinate parametrizes a family of static [classical field-theory solitons](classical-field-theory-soliton.md), for example their position or internal orientation. Derivatives with respect to these parameters are [zero modes in field theory](relativistic-quantum-field.md#zero-mode-in-field-theory) when the family has constant energy. Slowly varying coordinates describe low-energy motion, provided the excluded modes and radiation are negligible; gauge variations must first be removed in a [gauge-theory soliton](#gauge-theory-soliton).

### Quantization of a periodic soliton coordinate

↑ **Parent:** [Collective coordinate of a soliton](#collective-coordinate-of-a-soliton)

The conjugate [momentum](classical-mechanics.md#momentum) to a periodic internal soliton angle generates shifts of that angle. Single-valued wavefunctions, or [Bohr-Sommerfeld quantization](quantum-mechanics.md#bohr-sommerfeld-quantization) with zero [Maslov index](symplectic-geometry.md#maslov-index), quantize this [canonical momentum](classical-mechanics.md#canonical-momentum). A theta term can shift the relation between [canonical momentum](classical-mechanics.md#canonical-momentum) and mechanical charge without changing integer canonical labels.

### Collective-coordinate effective Lagrangian for a soliton

↑ **Parent:** [Collective coordinate of a soliton](#collective-coordinate-of-a-soliton)

A collective-coordinate approximation substitutes a finite-parameter soliton ansatz into the field action and integrates over space. Its Euler-Lagrange equations approximate the slow motion of the soliton parameters.

#### Instantaneous-boost effective action for a sine-Gordon kink

↑ **Parent:** [Collective-coordinate effective Lagrangian for a soliton](#collective-coordinate-effective-lagrangian-for-a-soliton)

Substitute the instantaneous [Sine-Gordon kink](scalar-field-theory.md#sine-gordon-kink) profile $\theta_K(\gamma(x-X))$ and prescribed velocity $-\gamma\dot X\theta_K'$ with $\gamma=(1-\dot X^2)^{-1/2}$ into the field density. For $A_1=0$, $A_0=xf(t)$, the integrals $\int(\theta_K')^2=8$ and $\int\theta_K'=2\pi$ give the displayed [collective-coordinate effective Lagrangian](#collective-coordinate-effective-lagrangian-for-a-soliton). Its equation is $d(8\gamma\dot X)/dt=-2\pi f$. This is relativistic particle motion with mass $8$ and topological coupling charge $2\pi$. When $\gamma$ varies, the prescribed velocity omits a width-change contribution; [acceleration correction for an instantaneous boosted kink](#acceleration-correction-for-an-instantaneous-boosted-kink) describes the exact chain-rule distinction.

##### Acceleration correction for an instantaneous boosted kink

↑ **Parent:** [Instantaneous-boost effective action for a sine-Gordon kink](#instantaneous-boost-effective-action-for-a-sine-gordon-kink)

The actual derivative of $\theta_K(\gamma(t)(x-X(t)))$ is $[\dot\gamma(x-X)-\gamma\dot X]\theta_K'$. The omitted contribution is first order in acceleration. Its cross term with the translation velocity integrates to zero because $\int y(\theta_K'(y))^2dy=0$. The square adds $\dot\gamma^2\int y^2(\theta_K')^2dy/(2\gamma^3)=\pi^2\dot\gamma^2/(3\gamma^3)$ to the spatially integrated density, since $\theta_K'=2\operatorname{sech}y$ and $\int y^2(\theta_K')^2dy=2\pi^2/3$. Thus the [instantaneous-boost effective action for a sine-Gordon kink](#instantaneous-boost-effective-action-for-a-sine-gordon-kink) is an adiabatic truncation rather than the exact action restricted to that accelerating configuration-space profile.

### Moduli-space approximation for solitons

↑ **Parent:** [Collective coordinate of a soliton](#collective-coordinate-of-a-soliton)

Substitute a static soliton family with slowly time-dependent [collective coordinates](#collective-coordinate-of-a-soliton) into the action. The kinetic energy induces a [Riemannian metric](differential-geometry.md#riemannian-metric) $g$ on the family, after imposing any [Gauss law constraint in gauge theory](relativistic-quantum-field.md#gauss-law-constraint-in-gauge-theory) constraint and projecting out gauge directions. If its static energy is constant, the [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) are the [geodesic](riemannian-geometry.md#geodesic) equations of $g$. An approximately flat family instead carries a potential $V(q)$. This approximation neglects excitations of the other field modes and is justified only when their effects are small on the time and energy scales studied.

#### Collective-coordinate quantization

↑ **Parent:** [Moduli-space approximation for solitons](#moduli-space-approximation-for-solitons)

Quantizing a [moduli-space approximation](#moduli-space-approximation-for-solitons) gives wavefunctions with measure $\sqrt{\det g}\,d^dq$ and, under the minimal scalar ordering, the [Hamiltonian operator](quantum-mechanics.md#hamiltonian-quantum-mechanics) $-\hbar^2\Delta_g/2+V$, where $\Delta_g$ is the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator). Global identifications, statistics and regularity supply additional restrictions on wavefunctions. Curvature-dependent ordering terms or quantum corrections are extra choices, not determined by the classical kinetic energy alone.

## Topological charge

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_charge)

A topological charge is an integer or other discrete invariant determined by the homotopy class or characteristic class of a field configuration. Continuous finite-energy deformations cannot change it without crossing a singular or forbidden configuration.

### Vacuum-boundary degree as a defect charge

↑ **Parent:** [Topological charge](#topological-charge)

A normalized vacuum field on a sphere surrounding a core can define $S^{d-1}\to S^{d-1}$ with integer [topological degree](geometry-and-topology.md#topological-degree). Nonzero degree obstructs its extension through the enclosed ball while staying in the [vacuum manifold](quantum-field-theory.md#vacuum-manifold). This accounts for the [winding number](complex-analysis.md#winding-number) of a [vortex](critical-phenomenon.md#phase-vortex) and the spherical degree of a [magnetic monopole](physics.md#magnetic-monopole), with the appropriate vacuum targets.

### Degree and energetic stability of a field configuration

↑ **Parent:** [Topological charge](#topological-charge)

A nonzero [topological degree](geometry-and-topology.md#topological-degree) obstructs smooth unwinding with fixed boundary data, but does not by itself give a stable finite size. In three dimensions a two-derivative energy scales as $R$ and can decrease as a configuration shrinks at fixed degree. The four-derivative [Skyrme term](#skyrme-term) scales as $R^{-1}$ and can balance this tendency. [Derrick theorem](#derrick-s-theorem) addresses the energetic issue; a singular limiting configuration can evade smooth [homotopy](algebraic-topology.md#homotopy) conservation.

### Topological current

↑ **Parent:** [Topological charge](#topological-charge)

A local current whose conservation follows from field geometry rather than requiring the field equation. For [Skyrmions](#skyrmion), pulling back the closed volume form on the target three-sphere gives the current associated with [topological baryon number in the Skyrme model](#topological-baryon-number-in-the-skyrme-model). Its spatial integral is a [topological charge](#topological-charge), unchanged by smooth evolution with the prescribed boundary behaviour.

#### Pullback-volume representation of a topological current

↑ **Parent:** [Topological current](#topological-current)

A closed target $d$-form $\omega$ pulls back under a spacetime field $\phi$ to a closed form $\alpha=\phi^*\omega$. Its dual defines an identically conserved [topological current](#topological-current). For a compact oriented spatial $d$-manifold and an equally dimensional oriented target with $\int\omega=1$, the spatial integral is the [topological degree](geometry-and-topology.md#topological-degree). Conservation follows without the field equations; changing boundary flux can change the charge.

### Topological sector

↑ **Parent:** [Topological charge](#topological-charge)

A connected component, or homotopy class, of admissible field configurations with fixed asymptotic conditions. Distinct [topological sectors](#topological-sector) cannot be joined by a continuous deformation within that configuration space. A nonzero [topological charge](#topological-charge) labels a sector, but a stable finite-size energy minimum also depends on the energy functional.

<h2 id="bright-soliton-of-the-focusing-nonlinear-schrodinger-equation">Bright soliton of the focusing nonlinear Schrödinger equation</h2>

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

For negative frequency $E$, the one-dimensional focusing nonlinear Schrödinger equation has the localized stationary profile

$$
f_E(x)=\sqrt{2|E|}\operatorname{sech}(\sqrt{2|E|}x).
$$

Galilean boosts generate moving profiles with a translational collective coordinate and constant velocity.

<h3 id="harmonic-trap-translation-of-a-nonlinear-schrodinger-soliton">Harmonic-trap translation of a nonlinear Schrödinger soliton</h3>

↑ **Parent:** [Bright soliton of the focusing nonlinear Schrödinger equation](#bright-soliton-of-the-focusing-nonlinear-schrodinger-equation)

Let a real localized profile satisfy $Ef=-f''/2-f^3+y^2f/2$. Then $\psi(x,t)=e^{i\Theta(x,t)}f(x-X(t))$ solves the cubic [focusing nonlinear Schrodinger equation](integrable-systems.md#focusing-nonlinear-schrodinger-equation) in the potential $x^2/2$ with the displayed phase and any harmonic-oscillator trajectory $X$. Imaginary terms require $\Theta_x=\dot X$; real terms require $\ddot X=-X$ and the remaining time-dependent phase. The translation is exact and causes no profile deformation, unlike a generic [collective-coordinate effective Lagrangian](#collective-coordinate-effective-lagrangian-for-a-soliton) approximation.

<h3 id="galilean-boost-of-a-nonlinear-schrodinger-soliton">Galilean boost of a nonlinear Schrödinger soliton</h3>

↑ **Parent:** [Bright soliton of the focusing nonlinear Schrödinger equation](#bright-soliton-of-the-focusing-nonlinear-schrodinger-equation)

For $i\psi_t=-\psi_{xx}/2-|\psi|^2\psi$, translation of a solution at velocity $u$ must be accompanied by the displayed phase. Direct differentiation cancels the terms proportional to $\partial_x\psi_0$, leaving the original equation. A standing profile of frequency $E=-\kappa^2/2$ thus gives $\kappa\operatorname{sech}(\kappa(x-ut-X_0))e^{iux-i(u^2/2+E)t+i\theta_0}$. Its centre travels uniformly, while its [L2 norm](real-analysis.md#l2-norm) is unchanged.

<h2 id="derrick-s-theorem">Derrick's theorem</h2>

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Derrick's_theorem)

Derrick's scaling argument tests a static field configuration by rescaling space. A soliton can be stationary only if energy terms with opposite scaling powers balance at the original scale.

### Two-dimensional flat-target Derrick obstruction

↑ **Parent:** [Derrick's theorem](#derrick-s-theorem)

For smooth fields into $\mathbb R^l$ with nonnegative differentiable potential and finite energy, [Derrick scaling](#derrick-scaling) in two spatial dimensions forces the potential integral to vanish. Thus the field takes values where $U=0$ and $\nabla U=0$, so its static field equation makes every component harmonic. Each first derivative is an entire harmonic function in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space); the mean-value inequality on arbitrarily large balls forces it to vanish. Hence the field is constant. The scale identity alone does not exclude a pure-gradient model; this additional argument uses the flat unconstrained target. Curved-target [harmonic maps](differential-geometry.md#harmonic-map), for example the [O3 nonlinear sigma model](quantum-field-theory.md#o3-nonlinear-sigma-model), can instead have finite-energy nonconstant solutions.

### Derrick scaling

↑ **Parent:** [Derrick's theorem](#derrick-s-theorem)

Under Derrick scaling, an energy term containing $m$ spatial derivatives and homogeneous of degree $m$ in those derivatives scales as $\lambda^{m-D}$ in $D$ spatial dimensions.

#### No static finite-energy lump in three-dimensional pure Yang-Mills theory

↑ **Parent:** [Derrick scaling](#derrick-scaling)

For a smooth [gauge field](relativistic-quantum-field.md#gauge-field) on $\mathbb R^3$ with finite positive magnetic [energy](classical-mechanics.md#energy), dilate its [connection one-form](fiber-bundle.md#connection-one-form) by $A_i^{(s)}(x)=sA_i(sx)$. Its [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) scales as $F_{ij}^{(s)}(x)=s^2F_{ij}(sx)$, so the energy scales as $s^4s^{-3}E=sE$. A static stationary configuration must have zero derivative at $s=1$, forcing $E=0$ and hence $F=0$. This [Derrick scaling](#derrick-scaling) argument assumes the dilation preserves the boundary conditions and that boundary terms vanish. It does not exclude four-dimensional [Yang-Mills instantons](#yang-mills-instanton), whose Euclidean action is scale invariant.

#### Derrick scaling of Yang-Mills-Higgs energy

↑ **Parent:** [Derrick scaling](#derrick-scaling)

In three space dimensions, rescale $A_i(x)$ to $\lambda A_i(\lambda x)$ and $\Phi(x)$ to $\Phi(\lambda x)$. The [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) then scales with two derivatives, and the [adjoint covariant derivative](relativistic-quantum-field.md#adjoint-covariant-derivative) of the [Higgs field](standard-model.md#higgs-field) with one. Magnetic, Higgs-gradient and potential energies give the displayed formula. Stationarity requires $V_B=V_D+3V_U$, which permits nonzero energies. In the [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole) limit $V_U=0$, the [Bogomolny equations](quantum-field-theory.md#bogomolny-equations) give $V_B=V_D$.

### Derrick virial identity

↑ **Parent:** [Derrick's theorem](#derrick-s-theorem)

Stationarity of a static solution under [Derrick scaling](#derrick-scaling) requires $dE(\lambda)/d\lambda|_{\lambda=1}=0$. This necessary relation among the separately scaling energy terms is the Derrick virial identity.

## Scalar-field kink

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

A scalar-field kink is a one-dimensional finite-energy static solution approaching different vacua as $x\to-\infty$ and $x\to+\infty$. Its boundary values define a topological sector.

### Antikink

↑ **Parent:** [Scalar-field kink](#scalar-field-kink)

An [antikink](#antikink) is a [scalar-field kink](#scalar-field-kink) with the opposite orientation of its vacuum boundary values. If $\phi_K(x)$ joins vacua $\phi_-$ to $\phi_+$, then $\phi_K(-x)$ joins $\phi_+$ to $\phi_-$. For an even double-well potential and an odd centered [phi-four kink](#phi-four-kink), the centered [antikink](#antikink) is $-\phi_K(x)$. With $Q=[\phi(+\infty)-\phi(-\infty)]/(\phi_+-\phi_-)$, a [kink](#scalar-field-kink) has $Q=1$ and an [antikink](#antikink) has $Q=-1$. Their localized energies coincide by spatial reflection.

### Phi-four kink

↑ **Parent:** [Scalar-field kink](#scalar-field-kink)

For the static energy

$$
E[\phi]=\frac12\int_{-\infty}^{\infty}
\left[\phi'^2+(c^2-\phi^2)^2\right]dx,
$$

the kink joining the vacua $-c$ and $c$ is

$$
\phi(x)=c\tanh(c(x-x_0)).
$$

It saturates the [Bogomolny bound](quantum-field-theory.md#bogomolny-bound) $E\geq4c^3/3$ by satisfying the first-order equation $\phi'=c^2-\phi^2$.

#### Relativistic energy and momentum of a phi-four kink

↑ **Parent:** [Phi-four kink](#phi-four-kink)

For the real [scalar field](quantum-field-theory.md#scalar-field) with metric $(+,-)$ and potential $U=\kappa^2(\phi^2-1)^2/2$, the static [phi-four kink](#phi-four-kink) is $\phi_0(x)=\tanh(\kappa x)$ and satisfies $\phi_0'^2=2U(\phi_0)$. Its mass is $M=\int\phi_0'^2dx=4\kappa/3$. A [Lorentz boost](special-relativity.md#lorentz-boost) gives $\phi(t,x)=\phi_0(\gamma(x-vt))$. The [stress-energy tensor](general-relativity.md#stress-energy-tensor) gives $P=-\int\phi_t\phi_xdx=\gamma v\int\phi_0'^2dx=\gamma Mv$. Similarly, $E=\tfrac12[\gamma(1+v^2)+\gamma^{-1}]M=\gamma M$, proving the [energy–momentum relation](special-relativity.md#energy-momentum-relation) $E^2-P^2=M^2$.

<h4 id="kink-antikink-attraction-from-the-stress-tensor">Kink–antikink attraction from the stress tensor</h4>

↑ **Parent:** [Phi-four kink](#phi-four-kink)

For $V(\phi)=\lambda(m^2-\phi^2)^2$ with $\lambda,m>0$, set $\kappa=\sqrt{2\lambda}m$. A well-separated [kink](#scalar-field-kink)–[antikink](#antikink) pair at $-d/2,d/2$ is approximated by $\phi=m\tanh\kappa(x+d/2)-m\tanh\kappa(x-d/2)-m$. At its midpoint, $\phi_x=0$ and $\phi=m-4m e^{-\kappa d}+O(e^{-2\kappa d})$. The static [stress-energy tensor](general-relativity.md#stress-energy-tensor) component $T^{11}=\phi_x^2/2-V$ is therefore negative there. [Momentum](classical-mechanics.md#momentum) conservation gives the force on the left half-line as $T^{11}(-\infty)-T^{11}(0)$, which is positive. Its leading magnitude is $F\sim32m^2\kappa^2e^{-2\kappa d}$. Thus the pair attracts. This is a controlled leading-tail estimate at large separation, not an exact superposed solution or a theorem about all subsequent collision outcomes.

##### At-rest force for a symmetric phi-four pair

↑ **Parent:** [Kink–antikink attraction from the stress tensor](#kink-antikink-attraction-from-the-stress-tensor)

For the initial field $\phi(x)=\tanh(x+c)-\tanh(x-c)-1$ and zero initial time derivative, evaluate the [scalar-field momentum flux](quantum-field-theory.md#scalar-field-momentum-flux) at the midpoint: $\phi_x(0)=0$ and $\phi(0)=2\tanh c-1$. The force on the left [kink](#scalar-field-kink) is the displayed positive value, attractive toward the right [antikink](#antikink). This exact initial expression has the large-separation asymptotic $32e^{-2d}$ for $d=2c$. If the initial velocity at the cut is $\psi(0)$, subtract $\psi(0)^2/2$.

#### Fluctuation operator of a phi-four kink

↑ **Parent:** [Phi-four kink](#phi-four-kink)

Linearizing about the [phi-four kink](#phi-four-kink) gives the displayed one-dimensional [Schrödinger operator](physics.md#schrodinger-operator) in unit kinetic normalization. Its translational [zero mode in field theory](relativistic-quantum-field.md#zero-mode-in-field-theory) is proportional to $\operatorname{sech}^2(cx)$. The localized shape eigenfunction $\operatorname{sech}(cx)\tanh(cx)$ has squared frequency $3c^2$, while the continuum starts at $4c^2$. Substitution verifies both bound-state eigenfunctions. The [Pöschl-Teller potential](quantum-mechanics.md#poschl-teller-potential) permits a short completeness argument for the bound modes. In $y=cx$ let $A_\ell=\partial_y+\ell\tanh y$. Then $H_K/c^2=A_2^\dagger A_2$, its partner is $A_2A_2^\dagger=A_1^\dagger A_1+3$, and $A_1A_1^\dagger=-\partial_y^2+1$. The last operator has no bound states. The kernels of $A_1$ and $A_2$ give the two stated modes, while the partner spectra exclude any further normalizable bound modes.

#### Translational dynamics of a phi-four kink

↑ **Parent:** [Phi-four kink](#phi-four-kink)

For $\phi_K(x-X)=c\tanh(c(x-X))$ in the unit kinetic normalization, $\int(\phi_K')^2dx=M=4c^3/3$. Substitution of $X(t)$ therefore gives the free-particle [collective-coordinate effective Lagrangian](#collective-coordinate-effective-lagrangian-for-a-soliton) $-M+M\dot X^2/2$. Its quantization has [momentum](classical-mechanics.md#momentum) $p$ and energy $M+p^2/(2M)$ to this order. The exact uniformly moving classical kink is a [Lorentz boost](special-relativity.md#lorentz-boost) of the static one, with energy $M/\sqrt{1-v^2}$.

### Kink in a phi-six model

↑ **Parent:** [Scalar-field kink](#scalar-field-kink)

Kinks in a phi-six model commonly arise from a nonnegative degree-six potential with three degenerate vacua. For the unit-vacuum normalization

$$
U(\phi)=\frac12\phi^2(1-\phi^2)^2,
$$

the kink joining $0$ to $1$ is

$$
\phi(x)=\frac1{\sqrt{1+e^{-2(x-x_0)}}}
$$

and has mass $1/4$. A rescaled model with $U(\phi)=\phi^2(\phi^2-4)^2$ has the elementary kink

$$
\phi(x)=\frac2{\sqrt{1+e^{-8\sqrt2(x-x_0)}}},
$$

and its mass is $4\sqrt2$ in the normalization $E=\int[(\phi')^2/2+U]dx$.

#### Bogomolny classification of a rescaled phi-six kink

↑ **Parent:** [Kink in a phi-six model](#kink-in-a-phi-six-model)

For $U=\phi^2(\phi^2-b^2)^2/2$ and $b>0$, the three [scalar-field vacua](quantum-field-theory.md#scalar-field-vacuum) are $-b,0,b$. The static first integral is $\phi_x^2=2U$. In either adjacent interval, $y=\phi^2/b^2$ obeys $y_x=\pm2b^2y(1-y)$, giving the displayed four oriented [kink](#scalar-field-kink) profiles with $\sigma,\eta\in\{1,-1\}$. Each has rest [energy](classical-mechanics.md#energy) $b^4/4$. The [intermediate-vacuum obstruction to a kink](#intermediate-vacuum-obstruction-to-a-kink) excludes a direct static connection from $-b$ to $b$: reaching zero would give zero derivative, and uniqueness of the smooth second-order field equation forces the zero solution. A [Lorentz boost](special-relativity.md#lorentz-boost) replaces $x-x_0$ by $(x-vt-x_0)/\sqrt{1-v^2}$.

// Destination: relativistic-quantum-field.bigb

#### Intermediate-vacuum obstruction to a kink

↑ **Parent:** [Kink in a phi-six model](#kink-in-a-phi-six-model)

If a proposed kink must cross a third degenerate vacuum, its first integral makes both the field derivative and potential vanish there. ODE uniqueness prevents it from crossing at finite distance, so the two elementary kink sectors can be joined only at infinite separation.

## Gauge-theory soliton

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)

A gauge-theory soliton is a finite-energy localized classical field configuration stabilized by topology or a balance among differently scaling energy terms.

### 't Hooft-Polyakov monopole

↑ **Parent:** [Gauge-theory soliton](#gauge-theory-soliton)

A smooth finite-energy monopole in an $SU(2)$ [Yang-Mills theory](relativistic-quantum-field.md#yang-mills-theory) with an adjoint [Higgs field](standard-model.md#higgs-field) uses the normalized Higgs direction at infinity to define a map $S^2_\infty\to S^2$. Its nonzero degree supplies the magnetic topological sector. Unlike a singular Abelian Dirac monopole, the non-Abelian gauge and Higgs fields can have a regular core. In the zero-potential limit the [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole) equations are $B_i=\pm D_i\Phi$.

### Bogomolny-Prasad-Sommerfield monopole

↑ **Parent:** [Gauge-theory soliton](#gauge-theory-soliton)

A Bogomolny-Prasad-Sommerfield monopole is a finite-energy Yang-Mills-Higgs configuration satisfying $B_i=\pm D_i\Phi$. Its magnetic charge is the degree of the normalized Higgs field at spatial infinity.

#### Higgs norm identity for a Bogomolny monopole

↑ **Parent:** [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole)

For the trace [inner product](linear-algebra.md#inner-product) and [adjoint covariant derivative](relativistic-quantum-field.md#adjoint-covariant-derivative), compatibility gives $\Delta|\Phi|^2=2|D\Phi|^2+2\langle\Phi,D_iD_i\Phi\rangle$. The [gauge-theory Bianchi identity](relativistic-quantum-field.md#gauge-theory-bianchi-identity) and $B_i=\pm D_i\Phi$ imply $D_iD_i\Phi=0$. Therefore $\Delta|\Phi|^2=2|D\Phi|^2$, equal to the energy density $|B|^2+|D\Phi|^2$ on a [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole). If the energy density is instead defined with an overall factor $1/2$, this Laplacian is twice that density.

#### Bogomolny monopole equations imply Yang-Mills-Higgs equations

↑ **Parent:** [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole)

For zero scalar potential, the static field equations are $D_iD_i\Phi=0$ and $D_iF_{ij}=[\Phi,D_j\Phi]$. If $B_i=-D_i\Phi$, the [gauge-theory Bianchi identity](relativistic-quantum-field.md#gauge-theory-bianchi-identity) gives the first equation. For the second,

$$
D_iF_{ij}=-\frac12\epsilon_{ijk}[F_{ik},\Phi]
=[B_j,\Phi]=[\Phi,D_j\Phi],
$$

using $F_{ik}=\epsilon_{ik\ell}B_\ell$ and $\epsilon_{ijk}\epsilon_{ik\ell}=-2\delta_{j\ell}$. Thus the first-order equations imply the full second-order equations locally, independently of the radial ansatz.

#### Hedgehog ansatz for a monopole

↑ **Parent:** [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole)

A spherically symmetric SU(2) monopole can be written with the internal Higgs direction aligned with the spatial radial direction and the gauge field built from the invariant tensor $\epsilon_{aij}$.

##### Prasad-Sommerfield radial monopole solution

↑ **Parent:** [Hedgehog ansatz for a monopole](#hedgehog-ansatz-for-a-monopole)

For a [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole), the dimensionless radial [Bogomolny equations](quantum-field-theory.md#bogomolny-equations) are $dK/d\rho=-KH$ and $dH/d\rho=(1-K^2)/\rho^2$. The displayed profiles solve both equations: differentiating $\rho/\sinh\rho$ gives $K(1/\rho-\coth\rho)=-KH$, while differentiating $H$ gives $1/\rho^2-\operatorname{csch}^2\rho=(1-K^2)/\rho^2$. At the origin $K=1-\rho^2/6+O(\rho^4)$ and $H=\rho/3+O(\rho^3)$, giving a regular core. At infinity $K$ decays exponentially and $H=1-1/\rho+O(e^{-2\rho})$, giving the vacuum Higgs magnitude and a long-range Abelian magnetic field.

##### Hedgehog monopole equations in radial profile variables

↑ **Parent:** [Hedgehog ansatz for a monopole](#hedgehog-ansatz-for-a-monopole)

For $\Phi^a=f(r)x^a/r$ and $A_i^a=\epsilon_{iaj}x^j\alpha(r)$ with $[e_a,e_b]=\epsilon_{abc}e_c$, set $K=1+r^2\alpha$. The equation $B=-D\Phi$ equates radial coefficients to give $f'=-2\alpha-r^2\alpha^2$ and transverse coefficients to give $r\alpha'+2\alpha=-f/r-r\alpha f$. These are exactly the displayed two radial equations. The sign depends on the chosen orientation and on the order of indices in the gauge ansatz.

### Abelian Higgs model

↑ **Parent:** [Gauge-theory soliton](#gauge-theory-soliton)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abelian_Higgs_model)

The Abelian Higgs model couples a complex scalar field to a $U(1)$ gauge field and permits magnetic vortex solitons in two spatial dimensions.

#### Broken-phase spectrum of the Abelian Higgs model

↑ **Parent:** [Abelian Higgs model](#abelian-higgs-model)

For $|D\Phi|^2-\lambda(|\Phi|^2-\eta^2)^2/4$, write $\Phi=(\eta+h/\sqrt2)e^{i\theta}$ and absorb $\partial\theta/e$ into the vector field. The quadratic Lagrangian has a real scalar of mass $m_h=\sqrt\lambda\eta$ and a vector of mass $m_A=\sqrt2e\eta$. The two scalar plus two massless-vector polarizations in the symmetric phase become one radial scalar plus three massive-vector polarizations. The removed phase supplies the longitudinal mode; local vortices retain global winding and quantized flux.

// Target: cosmology.bigb

#### Derrick scaling of the Abelian Higgs energy

↑ **Parent:** [Abelian Higgs model](#abelian-higgs-model)

In two dimensions, scale $\Phi_\lambda(x)=\Phi(\lambda x)$ and $A_{j,\lambda}(x)=\lambda A_j(\lambda x)$. The [magnetic field](electromagnetism.md#magnetic-field) has scaling weight two, the [gauge covariant derivative](relativistic-quantum-field.md#gauge-covariant-derivative) of the [Higgs field](standard-model.md#higgs-field) has weight one, and the potential has weight zero. Their integrated energies therefore have the powers shown. Stationarity gives $E_B=E_P$, a [Derrick virial identity](#derrick-virial-identity). This balance allows a planar [Abelian Higgs vortex](#nielsen-olesen-vortex) to have finite size even though a scalar-gradient-plus-nonnegative-potential model has no comparable magnetic term.

#### Inverse-density Abelian Higgs model

↑ **Parent:** [Abelian Higgs model](#abelian-higgs-model)

This planar [Abelian Higgs model](#abelian-higgs-model) replaces the usual magnetic energy by $B^2/h$. Use $D_i=\partial_i-iA_i$ and $B=\partial_1A_2-\partial_2A_1$. The magnetic term is singular at a zero of the [Higgs field](standard-model.md#higgs-field), so the admissible class must have finite energy; formal field equations are first derived where $h>0$. Its positive-flux [Bogomolny equations](quantum-field-theory.md#bogomolny-equations) are $(D_1+iD_2)\Phi=0$ and $B=h(1-h)/2$. On those solutions $B/h=(1-h)/2$ extends regularly across zeros.

##### Logarithmic equation for inverse-density Abelian Higgs vortices

↑ **Parent:** [Inverse-density Abelian Higgs model](#inverse-density-abelian-higgs-model)

Write $\Phi=e^{u/2+i\chi}$ away from its zeros and use the oriented planar [Hodge star](differential-form.md#hodge-star-operator) with $*dx^1=dx^2$. The first [Bogomolny equation](quantum-field-theory.md#bogomolny-equations) gives $A=d\chi-\tfrac12*du$. A zero of multiplicity $n_j$ contributes $u=2n_j\log|x-p_j|+\text{smooth}$ and phase winding $2\pi n_j$. Combining the smooth magnetic field with these delta sources gives the displayed equation and the topological boundary condition $u\to0$. Prescribed zero positions and multiplicities reduce multi-vortex construction to this scalar elliptic problem; a regular solution reconstructs both smooth fields.

##### Bogomolny bound for the inverse-density Abelian Higgs model

↑ **Parent:** [Inverse-density Abelian Higgs model](#inverse-density-abelian-higgs-model)

Let $j_i=\operatorname{Im}(\bar\Phi D_i\Phi)$. The identity

$$
|D\Phi|^2=|(D_1+iD_2)\Phi|^2+Bh+\partial_1j_2-\partial_2j_1
$$

and [completing the square](polynomial.md#completing-the-square) give, when the current boundary integral vanishes,

$$
V=\frac12\int\left[
|(D_1+iD_2)\Phi|^2+
\frac{(B-\tfrac12h(1-h))^2}{h}\right]+\frac12\int B.
$$

For flux $2\pi N>0$, the lower bound is $\pi N$, saturated by the two first-order [Bogomolny equations](quantum-field-theory.md#bogomolny-equations). Division by $h$ is interpreted in the finite-energy sense at its zeros.

#### Critically coupled Abelian Higgs field equations

↑ **Parent:** [Abelian Higgs model](#abelian-higgs-model)

Use metric $(+--)$, $D_\mu=\partial_\mu-ia_\mu$ and Lagrangian $-f_{\mu\nu}f^{\mu\nu}/4+\overline{D_\mu\phi}D^\mu\phi/2-(1-|\phi|^2)^2/8$. The [Euler-Lagrange field equations](quantum-field-theory.md#euler-lagrange-field-equation) are $D_\mu D^\mu\phi+(|\phi|^2-1)\phi/2=0$ and $\partial_\mu f^{\mu\nu}=\operatorname{Im}(\bar\phi D^\nu\phi)$. Varying $\bar\phi$ gives a kinetic contribution $-D_\mu D^\mu\phi/2$ and potential contribution $(1-|\phi|^2)\phi/4$; variation of $a_\nu$ gives $\partial_\mu f^{\mu\nu}-\operatorname{Im}(\bar\phi D^\nu\phi)$. For static fields in [temporal gauge](relativistic-quantum-field.md#temporal-gauge) $a_0=0$, the positive [Bogomolny vortex equations](#bogomolny-vortex-equation) imply the scalar equation because $(D_1-iD_2)(D_1+iD_2)=D_1^2+D_2^2+B$. They imply the spatial gauge equations because $\operatorname{Im}(\bar\phi D_1\phi)=-\partial_2|\phi|^2/2$ and $\operatorname{Im}(\bar\phi D_2\phi)=\partial_1|\phi|^2/2$, while $B=(1-|\phi|^2)/2$. The Gauss equation then vanishes identically.

#### Nielsen-Olesen vortex

↑ **Parent:** [Abelian Higgs model](#abelian-higgs-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nielsen–Olesen_vortex)

An Abelian Higgs vortex has quantized magnetic flux and a Higgs field whose phase winds at spatial infinity. Its vortex number is $N=(2\pi)^{-1}\int F$ under the convention $D=d-iA$.

##### Compact-core variational estimate for an Abelian Higgs vortex

↑ **Parent:** [Nielsen-Olesen vortex](#nielsen-olesen-vortex)

For a unit [Abelian Higgs vortex](#nielsen-olesen-vortex), the piecewise profiles $h=r/R$ and $a=(r/R)^2$ inside $r=R$, with both equal to one outside, are continuous finite-energy trial fields. In the normalization $E=\int[B^2/2+|D\phi|^2/2+(1-|\phi|^2)^2/8]$, their radial energy is the displayed function. Its minimum has $R^4=48$ and $E=\pi(2/3+1/\sqrt3)$, an upper-bound estimate above the exact [Bogomolny bound](quantum-field-theory.md#bogomolny-bound) $\pi$. Derivative jumps at the matching radius are allowed in the variational energy space; the trial profile is not an exact solution.

##### Magnetic flux quantization of an Abelian Higgs vortex

↑ **Parent:** [Nielsen-Olesen vortex](#nielsen-olesen-vortex)

When $|\Phi|\to1$ and its [gauge covariant derivative](relativistic-quantum-field.md#gauge-covariant-derivative) decays fast enough, on a large circle write $\Phi=\rho e^{i\chi}$ locally. The tangential derivative gives $A=d\chi-\operatorname{Im}(\overline\Phi D\Phi)/\rho^2$. The integrated error tends to zero, so [Stokes theorem](calculus.md#stokes-theorem) turns total [magnetic flux](electromagnetism.md#magnetic-flux) into the phase change $2\pi N$. This integer is the [winding number](complex-analysis.md#winding-number) of the normalized [Higgs field](standard-model.md#higgs-field) on the circle. For positive [Bogomolny vortex equations](#bogomolny-vortex-equation) it is the total zero multiplicity.

##### Vortex number

↑ **Parent:** [Nielsen-Olesen vortex](#nielsen-olesen-vortex)

The vortex number is the total multiplicity of the zeros of the Higgs field, equivalently its phase winding at infinity or its magnetic flux divided by $2\pi$ in the standard normalization.

##### Abelian Higgs vortex moduli space

↑ **Parent:** [Nielsen-Olesen vortex](#nielsen-olesen-vortex)

At critical coupling, the Abelian Higgs vortex moduli space is the space of gauge-equivalence classes of static $N$-vortex solutions. Vortex positions provide complex coordinates, and the field-theory kinetic energy induces an $L^2$ Riemannian metric whose geodesics approximate slow vortex motion.

###### Relative coordinate for two identical vortices

↑ **Parent:** [Abelian Higgs vortex moduli space](#abelian-higgs-vortex-moduli-space)

Interchanging two [Abelian Higgs vortices](#nielsen-olesen-vortex) replaces $q=z_1-z_2$ by $-q$. Thus $w=q^2$ is a single-valued relative coordinate on the unordered [Abelian Higgs vortex moduli space](#abelian-higgs-vortex-moduli-space). Coincidence is smooth in $w$; a geodesic crossing from positive real $w$ to negative real $w$ changes the line of separation by $\pi/2$, explaining [right-angle scattering of Abelian Higgs vortices](#right-angle-scattering-of-abelian-higgs-vortices). The asymptotic cone in the $q$ coordinate has angular period $\pi$ and must not be treated as a singularity of the actual coincidence metric.

###### Right-angle scattering of Abelian Higgs vortices

↑ **Parent:** [Abelian Higgs vortex moduli space](#abelian-higgs-vortex-moduli-space)

A head-on geodesic through the smooth coincidence point of the two-vortex moduli space emerges along the orthogonal axis. Two identical critically coupled vortices therefore scatter through $90^\circ$ in the slow-motion approximation.

##### Bogomolny vortex equation

↑ **Parent:** [Nielsen-Olesen vortex](#nielsen-olesen-vortex)

At critical coupling on a surface with conformal metric $g=\Omega dzd\bar z$, the vortex equations are

$$
D_{\bar z}\phi=0,
\qquad
B=\frac\Omega2(1-|\phi|^2).
$$

###### Logarithmic form of a Bogomolny vortex

↑ **Parent:** [Bogomolny vortex equation](#bogomolny-vortex-equation)

Away from zeros of the [Higgs field](standard-model.md#higgs-field), write $\phi=e^{u+i\chi}$ with $u=\log|\phi|$. The [Bogomolny vortex equation](#bogomolny-vortex-equation) $(D_1+iD_2)\phi=0$ gives $a_1=\chi_1+u_2$ and $a_2=\chi_2-u_1$. Consequently $\mathbf a=\nabla\chi-J\nabla u$, where $J(v_1,v_2)=(-v_2,v_1)$, and $B=-\Delta u$ on a regular phase patch. If the contours of $u$ and $\chi$ are orthogonal, then $\nabla u\cdot\nabla\chi=0$, so $\mathbf a\cdot\nabla u=0$: the [gauge potential](relativistic-quantum-field.md#gauge-field) is tangent to constant-amplitude contours. This does not imply that it is curl-free. At a vortex zero, $u\to-\infty$ and the phase is only locally defined. Including phase winding distributionally gives $\Delta u+(1-e^{2u})/2=2\pi\sum_jn_j\delta^{(2)}(x-X_j)$. The usual [Taubes equation](#taubes-equation) uses $2u=\log|\phi|^2$, so its delta coefficients double.

###### Bogomolny square completion for an Abelian Higgs vortex

↑ **Parent:** [Bogomolny vortex equation](#bogomolny-vortex-equation)

With $D_i=\partial_i-iA_i$ and $B=\partial_1A_2-\partial_2A_1$, use the critical-coupling energy $E=\int[B^2/2+|D_i\phi|^2/2+(1-|\phi|^2)^2/8]d^2x$. For positive [vortex number](#vortex-number), integration by parts gives

$$
E=\int\left[\frac12|(D_1+iD_2)\phi|^2+\frac12\left(B-\frac{1-|\phi|^2}{2}\right)^2\right]d^2x+\frac12\int B\,d^2x.
$$

The boundary divergence vanishes for the usual decaying vortex fields, and [magnetic flux](electromagnetism.md#magnetic-flux) is $2\pi N$. The two squares vanish exactly at the [Bogomolny vortex equations](#bogomolny-vortex-equation). Reversing both signs treats negative $N$. Energy coefficients and the numerical bound change together under other normalizations.

###### Conformal-surface vortex square completion

↑ **Parent:** [Bogomolny square completion for an Abelian Higgs vortex](#bogomolny-square-completion-for-an-abelian-higgs-vortex)

For metric $g=\Omega(dx^2+dy^2)$, set $F_{12}=\partial_xA_y-\partial_yA_x$ and use the physical [magnetic field](electromagnetism.md#magnetic-field) $B=F_{12}/\Omega$. At critical coupling, define $j_i=\operatorname{Im}(\bar\Phi D_i\Phi)$. The identity $|D_x\Phi|^2+|D_y\Phi|^2=|(D_x+iD_y)\Phi|^2+F_{12}|\Phi|^2+\partial_xj_y-\partial_yj_x$ completes the energy into nonnegative squares plus half the [magnetic flux](electromagnetism.md#magnetic-flux) and half the current boundary integral. For unit-magnitude vacuum boundary data, the combined boundary contribution is $\tfrac12\oint(A+j)=\pi N$, since $j=d\arg\Phi-A$ there. In the more restrictive covariantly decaying sector the current integral separately vanishes and the flux is $2\pi N$. Equality for positive $N$ requires $(D_x+iD_y)\Phi=0$ and $B=(1-|\Phi|^2)/2$. The factor $\Omega$ appears instead if the symbol $B$ denotes the coordinate component $F_{12}$.

###### Taubes equation

↑ **Parent:** [Bogomolny vortex equation](#bogomolny-vortex-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taubes_equation)

For $u=\log|\phi|^2$ and zeros of multiplicities $N_r$ at $z_r$, the Taubes equation is

$$
\Delta u+\Omega(1-e^u)=4\pi\sum_rN_r\delta^{(2)}(z-z_r).
$$

###### Prescribed-zero construction of planar Abelian Higgs vortices

↑ **Parent:** [Taubes equation](#taubes-equation)

Choose positions $z_a$ and positive integer multiplicities $m_a$. Solve the [Taubes equation](#taubes-equation) with $h\to0$ at infinity and $h=2m_a\log|z-z_a|+O(1)$ near each position. The planar existence theorem supplies such a solution for every finite multiset of positions; see [the original existence theorem](https://doi.org/10.1007/BF01197552). Set $\chi=\sum_am_a\arg(z-z_a)$, $\Phi=e^{h/2+i\chi}$ and $A=\nabla\chi-J\nabla h/2$, with $J(v_1,v_2)=(-v_2,v_1)$. The singular terms cancel in $A$, while $\Phi$ has precisely the selected zeros. These fields satisfy the [Bogomolny vortex equations](#bogomolny-vortex-equation), with $B=(1-|\Phi|^2)/2$. Their [vortex number](#vortex-number) is $\sum_am_a$. Complex conjugation of $\Phi$ together with $A\mapsto-A$ gives antivortices.

###### Vortex composition by conformal rescaling

↑ **Parent:** [Taubes equation](#taubes-equation)

If $u$ solves the Taubes equation for a metric $g$ and $\widetilde u$ solves it for $e^ug$, then $u+\widetilde u$ solves it for $g$. The vortex divisors add, so the total vortex number is $N+\widetilde N$.

###### Bradlow bound

↑ **Parent:** [Taubes equation](#taubes-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bradlow_bound)

Integrating the Taubes equation on a compact surface of area $A$ gives $A\geq4\pi N$. A nontrivial vortex with nonzero Higgs field requires the strict inequality $A>4\pi N$.

###### Hyperbolic vortex

↑ **Parent:** [Bogomolny vortex equation](#bogomolny-vortex-equation)

At the integrable curvature scale on the Poincare disc, the vortex Taubes equation reduces to the Liouville equation. Holomorphic self-maps of the disc then generate explicit vortex solutions.

###### Hyperbolic one-vortex at curvature minus one half

↑ **Parent:** [Hyperbolic vortex](#hyperbolic-vortex)

For metric $8|dz|^2/(1-|z|^2)^2$, these smooth fields satisfy the [Bogomolny vortex equations](#bogomolny-vortex-equation) with one simple zero at the origin. Their curvature coefficient is $F_{12}=4/(1+|z|^2)^2$, and their physical [magnetic field](electromagnetism.md#magnetic-field) is $(1-|z|^2)^2/[2(1+|z|^2)^2]=(1-|\Phi|^2)/2$. The [magnetic flux](electromagnetism.md#magnetic-flux) is $2\pi$, and the critically coupled energy in the [conformal-surface vortex square completion](#conformal-surface-vortex-square-completion) normalization is $\pi$.

###### Witten hyperbolic vortex

↑ **Parent:** [Hyperbolic vortex](#hyperbolic-vortex)

For the disc metric $8|dz|^2/(1-|z|^2)^2$ and a holomorphic map $g:D\to D$, the Higgs magnitude

$$
|\Phi|=\frac{(1-|z|^2)|g'(z)|}{1-|g(z)|^2}
$$

solves the critically coupled vortex equations. Choosing $g(z)=z^{N+1}$ gives a radial vortex of winding $N$.

### Yang-Mills instanton

↑ **Parent:** [Gauge-theory soliton](#gauge-theory-soliton)

A Yang-Mills instanton is a finite-action Euclidean gauge field with self-dual or anti-self-dual curvature. On $\mathbb R^4$, its asymptotic pure gauge defines a map $S^3_\infty\to SU(2)$ whose degree is the instanton number.

It is a gauge-field [instanton](quantum-field-theory.md#instanton) solving the Euclidean [Yang-Mills equations](relativistic-quantum-field.md#yang-mills-equations), with additional finite-action and duality conditions.

#### Theta-weighted instanton sectors

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

For integer [instanton number](#instanton-number) $k$, a topological angle can weight each Euclidean gauge-field sector by $e^{ik\vartheta}$ in a stated convention. The sector sum is then $2\pi$-periodic in $\vartheta$. In temporal gauge, the same integer describes a change in the vacuum winding or [Chern-Simons number](geometry-and-topology.md#chern-simons-number-of-a-gauge-field), with compatible orientation conventions. Classical instanton action fixes exponential suppression, while determinants and collective-coordinate integrals supply prefactors.

#### ADHM construction

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ADHM_construction)

Take $V=\mathbb C^k$, $W=\mathbb C^N$, $B_1,B_2\in\operatorname{End}(V)$, $I:W\to V$, and $J:V\to W$, satisfying

$$
[B_1,B_2]+IJ=0,\qquad [B_1,B_1^\dagger]+[B_2,B_2^\dagger]+II^\dagger-J^\dagger J=0.
$$

Regular data modulo $U(k)$ construct framed [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations) solutions of charge magnitude $k$. The [ADHM factorization identity](#adhm-factorization-identity) gives an explicit [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) proof. The two complex [matrices](vector-space.md#matrix) and the two rectangular maps have $4k^2+4kN$ real parameters; three real [matrix](vector-space.md#matrix) constraints remove $3k^2$, and quotient by $U(k)$ removes another $k^2$, giving dimension $4kN$ at regular points. Degenerate data can describe zero-size singular limits rather than smooth [instantons](quantum-field-theory.md#instanton).

##### ADHM factorization identity

↑ **Parent:** [ADHM construction](#adhm-construction)

With $z_1=x^1+ix^2$, $z_2=x^3+ix^4$, form

$$
\mathcal D_z=\begin{pmatrix}B_2-z_2&B_1-z_1&I\\-B_1^\dagger+\bar z_1&B_2^\dagger-\bar z_2&J^\dagger\end{pmatrix}.
$$

The two [ADHM construction](#adhm-construction) constraints say that $\mathcal D_z\mathcal D_z^\dagger$ has zero off-diagonal blocks and equal diagonal blocks, so it equals $1_2\otimes f^{-1}$. Assume it is invertible everywhere. Choose an orthonormal kernel [bundle frame](fiber-bundle.md#frame-of-a-vector-bundle) $\Psi$, so $\mathcal D_z\Psi=0$ and $\Psi^\dagger\Psi=1_N$, and set $A=\Psi^\dagger d\Psi$. The orthogonal complement projector is $1-\Psi\Psi^\dagger=\mathcal D_z^\dagger(1_2\otimes f)\mathcal D_z$. Differentiating the kernel equation gives

$$
F=\Psi^\dagger d\mathcal D_z^\dagger(1_2\otimes f)\wedge d\mathcal D_z\Psi.
$$

Its space-time [differential two-form](differential-form.md#2-form) entries are combinations of $dz_1\wedge d\bar z_1-dz_2\wedge d\bar z_2$, $dz_1\wedge d\bar z_2$, and $d\bar z_1\wedge dz_2$, all anti-self-dual. Thus the constructed [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) satisfies the [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations).

#### BPST instanton

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/BPST_instanton)

With [Skew-Hermitian](linear-operator-theory.md#skew-hermitian-matrix) $SU(2)$ generators obeying $[T_a,T_b]=\epsilon_{abc}T_c$ and $\operatorname{tr}(T_aT_b)=-\delta_{ab}/2$, put

$$
A_\mu^a=\frac{2\eta^a_{\mu\nu}(x-a)^\nu}{|x-a|^2+\rho^2},\qquad
F_{\mu\nu}^a=-\frac{4\rho^2\eta^a_{\mu\nu}}{(|x-a|^2+\rho^2)^2}.
$$

The [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) is self-dual. The identity $\sum_{a,\mu,\nu}(\eta^a_{\mu\nu})^2=12$ gives $F^2=192\rho^4/(|x-a|^2+\rho^2)^4$. Radial integration yields action $8\pi^2/g^2$ and charge one with $k=-(8\pi^2)^{-1}\int\operatorname{tr}(F\wedge F)$. The parameters are center $a\in\mathbb R^4$, size $\rho>0$, and global gauge orientation in a framed description. Replacing $\eta$ by $\bar\eta$ reverses duality and charge.

#### Finite Yang-Mills action forbids nontrivial translation symmetry

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

A smooth [gauge field](relativistic-quantum-field.md#gauge-field) of finite positive Euclidean [Yang-Mills action](relativistic-quantum-field.md#yang-mills-action) cannot be invariant under a nonzero translation, even up to [gauge transformation](electromagnetism.md#gauge-transformation). The positive gauge-invariant action density would be periodic along that translation. A ball on which the density is bounded below by a positive constant has infinitely many disjoint translated copies, making the action infinite. Continuous translation invariance is a special case. Consequently a nonflat translation-invariant field satisfying the [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations) on $\mathbb R^3\times\mathbb R$ is not a finite-action [Yang-Mills instanton](#yang-mills-instanton). Flat connections are the zero-action exception. Translations still act on instanton moduli, sending a localized instanton to a distinct centered configuration.

#### Boundary winding representation of Yang-Mills topological charge

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

For an anti-Hermitian [SU(2)](topological-group.md#su-2-group) connection on $\mathbb R^4$ tending to $g^{-1}dg$ at infinity, the [Chern-Simons 3-form](geometry-and-topology.md#chern-simons-3-form) and [Maurer-Cartan equation](lie-theory.md#maurer-cartan-equation) give $(8\pi^2)^{-1}\int\operatorname{tr}(F\wedge F)=-(24\pi^2)^{-1}\int_{S^3}\operatorname{tr}(g^{-1}dg)^3=\deg g$. This is the second-Chern convention with the boundary orientation. Defining instanton charge with the opposite trace sign reverses this integer.

#### Instanton moduli space

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

For a fixed [principal bundle](fiber-bundle.md#principal-bundle), orientation and instanton sign, quotient the [Yang-Mills instanton](#yang-mills-instanton) solutions by [gauge equivalence of principal connections](fiber-bundle.md#gauge-equivalence-of-principal-connections). Boundary or framing conditions determine the gauge group $\mathcal G$ on a noncompact base. At an anti-self-dual solution, infinitesimal deformations obey $P_+D_Aa=0$ modulo $a\mapsto a+D_A\varepsilon$. Combining this with $D_A^*a=0$ gives an elliptic deformation operator. This description does not assert that every quotient is a smooth manifold: reducible connections can have nontrivial stabilizers.

##### Instanton size modulus

↑ **Parent:** [Instanton moduli space](#instanton-moduli-space)

The scale $\rho>0$ in a [BPST instanton](#bpst-instanton) changes the width of its action density while leaving total action unchanged. This reflects conformal invariance of four-dimensional classical [Yang-Mills action](relativistic-quantum-field.md#yang-mills-action). As $\rho\to0$, [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) concentrates at the center and the smooth family approaches a bubbling boundary, not another smooth zero-size [instanton](quantum-field-theory.md#instanton).

##### Framed instanton moduli space

↑ **Parent:** [Instanton moduli space](#instanton-moduli-space)

Fix a trivialization at infinity and divide smooth finite-action [instantons](quantum-field-theory.md#instanton) only by [gauge transformations](electromagnetism.md#gauge-transformation) tending to the identity there. Global gauge orientations remain genuine parameters. For regular $SU(2)$ [instantons](quantum-field-theory.md#instanton) of charge magnitude $k$, the real dimension is $8k$ by the [ADHM construction](#adhm-construction). Forgetting the framing divides by the three-dimensional global [group action](group-theory.md#group-action) of $SU(2)$, giving $8k-3$ on the irreducible locus. For one [instanton](quantum-field-theory.md#instanton) the framed parameters are four center coordinates, one positive size, and three orientation coordinates.

#### Self-duality implies Yang-Mills equations

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

Both the [self-dual Yang-Mills equations](#self-dual-yang-mills-equations) and the [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations) imply the second-order [Yang-Mills equations](relativistic-quantum-field.md#yang-mills-equations) because the [Bianchi identity](fiber-bundle.md#bianchi-identity) holds for every [principal connection](fiber-bundle.md#connection-principal-bundle). Finite action is additionally required to call the solution a [Yang-Mills instanton](#yang-mills-instanton); the implication itself is a local differential identity.

#### Self-dual Yang-Mills equations

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

The self-dual [Yang-Mills equations](relativistic-quantum-field.md#yang-mills-equations) require a [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) two-form to have positive [Hodge star operator](differential-form.md#hodge-star-operator) eigenvalue on an oriented Riemannian four-manifold. By the [Bianchi identity](fiber-bundle.md#bianchi-identity), they imply the full second-order [Yang-Mills equations](relativistic-quantum-field.md#yang-mills-equations). Smooth finite-action solutions saturate the [Yang-Mills instanton Bogomolny bound](#yang-mills-instanton-bogomolny-bound). Reversing orientation exchanges this equation with the [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations).

##### Self-duality of gauge curvature

↑ **Parent:** [Self-dual Yang-Mills equations](#self-dual-yang-mills-equations)

In oriented Euclidean four-space, gauge curvature is self-dual when $F=*F$. The Hodge star squares to one on two-forms, so this picks its positive eigenspace; the negative eigenspace is [anti-self-duality of gauge curvature](#anti-self-duality-of-gauge-curvature). The [Bianchi identity](fiber-bundle.md#bianchi-identity) then implies the [Yang-Mills equations](relativistic-quantum-field.md#yang-mills-equations), and the action saturates the positive-charge [Yang-Mills instanton Bogomolny bound](#yang-mills-instanton-bogomolny-bound).

##### Self-dual Yang-Mills equations in temporal gauge

↑ **Parent:** [Self-dual Yang-Mills equations](#self-dual-yang-mills-equations)

With orientation $dx^1\wedge dx^2\wedge dx^3\wedge dt$, $\epsilon_{123}=1$, and [temporal gauge](relativistic-quantum-field.md#temporal-gauge) $A_t=0$, the mixed [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) is $F_{ti}=\partial_tA_i$. The [self-dual Yang-Mills equations](#self-dual-yang-mills-equations) then have the displayed form. Placing $dt$ first in the orientation reverses the sign, so the metric alone does not specify it.

#### Yang-Mills instanton Bogomolny bound

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

For $k=-(8\pi^2)^{-1}\int\operatorname{Tr}(F\wedge F)$ and positive Euclidean action, decomposition into self-dual and anti-self-dual curvature gives

$$
S_{\rm YM}\geq\frac{8\pi^2}{g_{\rm YM}^2}|k|.
$$

Equality holds for a self-dual or anti-self-dual connection.

#### Anti-self-dual Yang-Mills equations

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

The anti-self-dual Yang-Mills equations require the curvature of a connection on an oriented Euclidean four-manifold to satisfy $F=-*F$. In complex coordinates $(w,z)$ they can be written

$$
F_{wz}=F_{\bar w\bar z}=0,
\qquad
F_{w\bar w}+F_{z\bar z}=0.
$$

##### Anti-self-duality of gauge curvature

↑ **Parent:** [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations)

Anti-self-dual gauge curvature obeys $F=-*F$ in oriented Euclidean four-space. In the corresponding two-spinor convention it has vanishing symmetric primed curvature spinor. A matrix-valued two-form which is both self-dual and anti-self-dual is zero, because adding the two equations gives $2F=0$.

##### Complex potential reduction of anti-self-dual Yang-Mills

↑ **Parent:** [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations)

Locally, the [ASDYM equations](#anti-self-dual-yang-mills-equations) permit a complex gauge with $A_w=A_z=0$. The trace equation then gives $A_{\bar w}=K_z$ and $A_{\bar z}=-K_w$. The remaining curvature equation is $K_{w\bar w}+K_{z\bar z}-[K_w,K_z]=0$. A complex gauge generally makes $K$ valued in the [complexification of a Lie algebra](lie-algebra.md#complexification-of-a-lie-algebra); reconstructing a real connection requires its inherited reality condition. The gauge/potential construction is local and need not preserve prescribed behaviour at infinity.

##### Anti-self-dual Yang-Mills equations in temporal gauge

↑ **Parent:** [Anti-self-dual Yang-Mills equations](#anti-self-dual-yang-mills-equations)

With orientation $dx^1\wedge dx^2\wedge dx^3\wedge d\tau$ and $A_\tau=0$, one anti-self-duality convention becomes

$$
\partial_\tau A_i=\frac12\epsilon_{ijk}F_{jk}.
$$

###### Nahm equations

↑ **Parent:** [Anti-self-dual Yang-Mills equations in temporal gauge](#anti-self-dual-yang-mills-equations-in-temporal-gauge)

For three Lie-algebra-valued functions of one variable, the [Nahm equations](#nahm-equations) are

$$
\dot A_a=\frac12\epsilon_{abc}[A_b,A_c].
$$

They arise by taking a solution of the [ASDYM equations](#anti-self-dual-yang-mills-equations) with orientation $dx^1\wedge dx^2\wedge dx^3\wedge dt$, imposing independence of $x^1,x^2,x^3$, and setting $A_t=0$ by a local [Yang-Mills gauge transformation](relativistic-quantum-field.md#yang-mills-gauge-transformation). Then $F_{ab}=[A_a,A_b]$, $F_{a t}=-\dot A_a$, and [anti-self-duality of gauge curvature](#anti-self-duality-of-gauge-curvature) gives the displayed equations. The opposite orientation reverses their sign.

###### Polynomial Lax representation of the Nahm equations

↑ **Parent:** [Nahm equations](#nahm-equations)

Put $P=A_1+iA_2$, $Q=A_1-iA_2$ and $R=A_3$, and define

$$
L(\lambda)=P+2R\lambda-Q\lambda^2,\qquad
M(\lambda)=-iR+iQ\lambda.
$$

Direct expansion gives $[L,M]=-i[P,R]+i[P,Q]\lambda+i[R,Q]\lambda^2$. The [Nahm equations](#nahm-equations) imply $\dot P=-i[P,R]$, $2\dot R=i[P,Q]$ and $-\dot Q=i[R,Q]$, so $\dot L=[L,M]$. In any finite-dimensional [matrix](vector-space.md#matrix) representation, cyclicity of the [matrix trace](linear-algebra.md#matrix-trace) gives

$$
\frac d{dt}\operatorname{Tr}L^p
=p\operatorname{Tr}(L^{p-1}[L,M])=0\qquad(p=1,2,\ldots).
$$

Thus every coefficient of the degree-at-most-$2p$ [matrix trace](linear-algebra.md#matrix-trace) polynomial is conserved. At projective infinity the polynomial is interpreted as a section of $\mathcal O(2p)$, not a globally [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) scalar function on the [complex projective line](algebraic-topology.md#complex-projective-line).

#### Instanton number

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

For an $SU(2)$ connection under a standard trace convention,

$$
k=\frac1{8\pi^2}\int\operatorname{Tr}(F\wedge F)\in\mathbb Z.
$$

Its sign depends on orientation and on whether the instanton is self-dual or anti-self-dual.

##### Instanton number as a winding number at infinity

↑ **Parent:** [Instanton number](#instanton-number)

For a finite-action $SU(2)$ connection on $\mathbb R^4$ that approaches $A=-dg\,g^{-1}$ at infinity,

$$
k=\frac1{24\pi^2}\int_{S^3_\infty}
\operatorname{Tr}\left[(dg\,g^{-1})^{\wedge3}\right]
$$

under the convention $k=(8\pi^2)^{-1}\int\operatorname{Tr}(F\wedge F)$. This integer is the [degree of a map between oriented manifolds](homology.md#degree-of-a-map-between-oriented-manifolds) $g:S^3_\infty\to SU(2)\cong S^3$; orientation and trace conventions may reverse its sign.

#### Dimensional reduction of a Yang-Mills instanton to a monopole

↑ **Parent:** [Yang-Mills instanton](#yang-mills-instanton)

If a four-dimensional Euclidean connection is independent of one coordinate and that connection component is renamed $\Phi$, the self-dual Yang-Mills equation reduces to the three-dimensional [Bogomolny-Prasad-Sommerfield monopole](#bogomolny-prasad-sommerfield-monopole) equation $B_i=\pm D_i\Phi$.

##### Orientation of a monopole lift

↑ **Parent:** [Dimensional reduction of a Yang-Mills instanton to a monopole](#dimensional-reduction-of-a-yang-mills-instanton-to-a-monopole)

Use $\epsilon_{123}=1$ and orientation $d\tau\wedge dx^1\wedge dx^2\wedge dx^3$. A $\tau$-independent [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) has mixed component $\mathcal F_{i\tau}=D_i\Phi$. If $B_i=D_i\Phi$, its two-form is $\sum_{\rm cyclic}B_i(dx^j\wedge dx^k-d\tau\wedge dx^i)$. The [Hodge star operator](differential-form.md#hodge-star-operator) interchanges the two displayed basis forms, so $*\mathcal F=-\mathcal F$. With orientation $dx^1\wedge dx^2\wedge dx^3\wedge d\tau$ the same lift is self-dual; changing the sign of its $d\tau$ component instead recovers anti-self-duality. Orientation must therefore accompany any stated sign in this reduction.

## Skyrme model

↑ **Parent:** [Classical field-theory soliton](classical-field-theory-soliton.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skyrme_model)

The Skyrme model is a nonlinear sigma model for an $SU(2)$-valued field supplemented by a four-derivative term that evades Derrick collapse. Its topological degree is baryon number, and finite-energy solitons are Skyrmions.

### Derrick dimension test for the Skyrme model

↑ **Parent:** [Skyrme model](#skyrme-model)

For a spatially dilated [Skyrme model](#skyrme-model) field $U_L(x)=U(x/L)$, the quadratic and quartic derivative energies scale as shown. A static stationary field must satisfy $(d-2)E_2+(d-4)E_4=0$. In three spatial dimensions this permits $E_2=E_4$ and a positive second variation along scale. In two dimensions it requires $E_4=0$, and in four or more it forces a constant finite-energy smooth field. In one dimension the commutator term vanishes identically. [Derrick scaling](#derrick-scaling) tests a necessary variational condition, not existence or stability under all deformations.

#### Commuting-current obstruction in a two-dimensional Skyrme model

↑ **Parent:** [Derrick dimension test for the Skyrme model](#derrick-dimension-test-for-the-skyrme-model)

For a smooth finite-energy static planar [Skyrme model](#skyrme-model) field, [Derrick scaling](#derrick-scaling) gives zero quartic energy, hence $[R_1,R_2]=0$ pointwise. The quartic first variation then vanishes, leaving the sigma-model equation $\partial_iR_i=0$. The right-current [Maurer-Cartan equation](lie-theory.md#maurer-cartan-equation) gives $\partial_1R_2-\partial_2R_1=[R_1,R_2]=0$. Each current component is therefore harmonic on the plane and square-integrable. The mean-value estimate on expanding disks makes each component zero, so $U$ is constant. This excludes smooth finite-energy planar static solutions of this potential-free SU(2) model, without misapplying the same conclusion to a pure curved-target sigma model.

### Skyrme term

↑ **Parent:** [Skyrme model](#skyrme-model)

The particular quartic-derivative interaction in the [Skyrme model](#skyrme-model), with $L_\mu=U^\dagger\partial_\mu U$. Its static energy is positive and scales inversely with soliton size, opposing collapse under [Derrick scaling](#derrick-scaling). It is one choice of four-derivative mesonic interaction, not the whole general fourth-order [chiral perturbation theory](standard-model.md#chiral-perturbation-theory) Lagrangian.

### Vacuum-preserving symmetry of the Skyrme model

↑ **Parent:** [Skyrme model](#skyrme-model)

The massless derivative [Skyrme model](#skyrme-model) has [chiral symmetry](standard-model.md#chiral-symmetry) $U\mapsto LUR^\dagger$. For the fixed finite-energy boundary condition $U(\infty)=1$, a transformation preserves the same vacuum exactly when $LR^\dagger=1$, or $L=R$. This leaves conjugation $U\mapsto AUA^\dagger$, the [isospin](standard-model.md#isospin) action. Since $A$ and $-A$ act identically, its effective group is $SO(3)$. Together with spatial translations and rotations it generates the localized zero-mode orbit of a [Skyrmion](#skyrmion). Independent axial rotations change the massless vacuum and are not additional normalizable rigid orientation modes in that fixed-vacuum sector. A usual positive pion-mass term preserves only conjugation even before the boundary condition is imposed.

### Skyrmion

↑ **Parent:** [Skyrme model](#skyrme-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skyrmion)

A Skyrmion is a finite-energy topological soliton of the [Skyrme model](#skyrme-model). Its baryon number is the degree of the compactified spatial map $S^3\to SU(2)\simeq S^3$.

#### Skyrmion model of a nucleus

↑ **Parent:** [Skyrmion](#skyrmion)

A charge-$A$ multi-[Skyrmion](#skyrmion) provides an intrinsic field configuration for an [atomic nucleus](physics.md#atomic-nucleus) with mass number $A$. Its spatial and [isospin](standard-model.md#isospin) collective coordinates must be quantized, with [Finkelstein-Rubinstein constraints](#finkelstein-rubinstein-constraints), before assigning physical nuclear states. A classical intrinsic shape is distinct from rotationally invariant observables in a spin-zero state.

#### Skyrmion stabilizer and collective-coordinate orbit

↑ **Parent:** [Skyrmion](#skyrmion)

For a centered static [Skyrmion](#skyrmion) $U_0$, the effective rotation-isorotation group is $G=SO(3)_{\rm space}\times SO(3)_{\rm iso}$. Its [stabilizer subgroup](group-theory.md#stabilizer-subgroup) $H$ consists of pairs obeying $A U_0(R^{-1}x)A^\dagger=U_0(x)$. Thus distinct rigid orientations form the [homogeneous space](lie-theory.md#homogeneous-space) $G/H$, by the [orbit-stabilizer theorem](group-theory.md#orbit-stabilizer-theorem). The unit hedgehog has diagonal $SO(3)$ stabilizer and three orientation coordinates; the toroidal two-Skyrmion has a one-dimensional continuous stabilizer and five; the tetrahedral and cubic cases have discrete stabilizers and six. Adding three translations gives zero-mode orbit dimensions 6, 8, 9, 9. These are symmetry-generated low-energy coordinates, not a claim that non-Bogomolny multi-Skyrmion solutions possess an exact flat moduli space of arbitrary separations.

#### Cubic four-Skyrmion

↑ **Parent:** [Skyrmion](#skyrmion)

The familiar low-energy $B=4$ [Skyrmion](#skyrmion) has a cubic baryon-density shell with six face-hole directions and full density symmetry $O_h$, the [symmetry group of a cube](group-theory.md#symmetry-group-of-a-cube). The proper subgroup is $O\cong S_4$, the [rotational symmetry group of a cube](group-theory.md#rotational-symmetry-group-of-a-cube); its field invariance includes compensating [isorotations](standard-model.md#isorotation). A useful [rational map approximation for Skyrmions](#rational-map-approximation-for-skyrmions) has $R(z)=(z^4+2i\sqrt3z^2+1)/(z^4-2i\sqrt3z^2+1)$. The relation $R(iz)=1/R(z)$ pairs a spatial quarter-turn with a target half-turn. Its branch directions are $z=0,\infty,\pm1,\pm i$, corresponding to the six coordinate-axis directions. The map gives an approximate field, not an exact analytic energy-minimizing solution.

#### Tetrahedral three-Skyrmion

↑ **Parent:** [Skyrmion](#skyrmion)

The familiar low-energy $B=3$ [Skyrmion](#skyrmion) has tetrahedral baryon-density symmetry $T_d$. Proper rotations form the [tetrahedral symmetry](finite-group-theory.md#tetrahedral-symmetry) group $T\cong A_4$, acting on the field with compensating [isorotations](standard-model.md#isorotation). An angular approximation is $R(z)=(i\sqrt3z^2-1)/(z^3-i\sqrt3z)$. Its [Wronskian of a rational map](isolated-singularity.md#wronskian-of-a-rational-map) is proportional to $z^4+2i\sqrt3z^2+1$. The four branch directions are the face-hole directions of a tetrahedral shell. A [rational map](isolated-singularity.md#rational-map-complex-analysis) and a variational radial profile approximate the actual field, and baryon-density symmetry must be distinguished from invariance of the [pion](standard-model.md#pion) field under an unaccompanied spatial rotation.

#### Toroidal two-Skyrmion

↑ **Parent:** [Skyrmion](#skyrmion)

The standard low-energy $B=2$ [Skyrmion](#skyrmion) in the ordinary [Skyrme model](#skyrme-model) has a toroidal baryon-density shape, with axial density symmetry $D_{\infty h}$. Its proper combined field symmetries have an $O(2)$-type stabilizer. The angular ansatz $R(z)=z^2$ in the [rational map approximation for Skyrmions](#rational-map-approximation-for-skyrmions) explains the axial relation $R(e^{i\theta}z)=e^{2i\theta}R(z)$: spatial rotation through $\theta$ is accompanied by [isorotation](standard-model.md#isorotation) through $2\theta$. The angular density vanishes at the two axial directions, yielding the toroidal hole. This describes the familiar minimal branch and a useful approximate field; it is not an assertion that every degree-two field is toroidal.

#### Topological baryon number in the Skyrme model

↑ **Parent:** [Skyrmion](#skyrmion)

For a smooth [Skyrme model](#skyrme-model) field $U:\mathbb R^3\to SU(2)$ with $U(\infty)=1$, compactification gives a map $S^3\to S^3$. With $L_i=U^\dagger\partial_iU$, its [degree of a map between oriented manifolds](homology.md#degree-of-a-map-between-oriented-manifolds) is $B=-(24\pi^2)^{-1}\int\epsilon_{ijk}\operatorname{tr}(L_iL_jL_k)d^3x$, with sign chosen so the standard decreasing hedgehog profile has $B=1$. The integrand is the pullback of the normalized volume form on $SU(2)$. Hence it is integer-valued and unchanged by smooth finite-energy [homotopies](algebraic-topology.md#homotopy). In the [rational map approximation for Skyrmions](#rational-map-approximation-for-skyrmions), a degree-$N$ angular map and profile $f(0)=\pi,f(\infty)=0$ give $B=-(2N/\pi)\int f'\sin^2f\,dr=N$. This is a topological conservation law, not the [Noether charge](quantum-field-theory.md#noether-charge) of [isospin](standard-model.md#isospin).

##### Skyrme baryon number as a mapping degree

↑ **Parent:** [Topological baryon number in the Skyrme model](#topological-baryon-number-in-the-skyrme-model)

Under [SU(2) as the three-sphere](topological-group.md#su-2-as-the-three-sphere), a [Skyrme model](#skyrme-model) field with $U\to I$ at infinity defines $S^3\to S^3$. Choose $T_i=-i\tau_i$ and positive left [volume form](differential-form.md#volume-form) $\theta^1\wedge\theta^2\wedge\theta^3$. The normalized form is $-(24\pi^2)^{-1}\operatorname{tr}(U^{-1}dU)^3$, so the [topological baryon number in the Skyrme model](#topological-baryon-number-in-the-skyrme-model) equals $\deg U$. Generator and orientation conventions fix the sign.

##### Skyrme baryon density

↑ **Parent:** [Topological baryon number in the Skyrme model](#topological-baryon-number-in-the-skyrme-model)

The local [Skyrme baryon density](#skyrme-baryon-density) is $\mathcal B(x)=-\epsilon_{ijk}\operatorname{tr}(L_iL_jL_k)/(24\pi^2)$, with $L_i=U^\dagger\partial_iU$ and $B=\int\mathcal B\,d^3x$. It is invariant under global [isorotations](standard-model.md#isorotation) and transforms as a scalar under proper spatial rotations, so its contours reveal the geometric shape of a [Skyrmion](#skyrmion). For the [rational map approximation for Skyrmions](#rational-map-approximation-for-skyrmions), $\mathcal B=-f'\sin^2f\,J_R/(2\pi^2r^2)$, where $J_R$ is the [angular Jacobian of a rational map](isolated-singularity.md#angular-jacobian-of-a-rational-map). Integrating $J_R$ over the sphere gives $4\pi\deg R$, recovering the integer total charge. A decreasing profile and holomorphic angular map give a nonnegative density, but a general field may have regions of negative density; positivity is not a general topological theorem. The density is different from the [energy density](statistical-physics.md#energy-density).

#### Skyrmion hedgehog ansatz

↑ **Parent:** [Skyrmion](#skyrmion)

The unit [Skyrmion](#skyrmion) has a spherically symmetric ansatz with [Pauli matrices](algebra.md#pauli-matrices) $\boldsymbol\sigma$, $f(0)=\pi$ and $f(\infty)=0$. The [baryon number](standard-model.md#baryon-number) is

$$
B=-\frac2\pi\int_0^\infty f'\sin^2f\,dr=1.
$$

The radial profile is obtained from the [Skyrme model](#skyrme-model) variational equation. Spatial rotations and [isospin](standard-model.md#isospin) rotations act on the same hedgehog orientation, leaving only three independent rotational [collective coordinates](#collective-coordinate-of-a-soliton).

##### Rotational quantization of a unit Skyrmion

↑ **Parent:** [Skyrmion hedgehog ansatz](#skyrmion-hedgehog-ansatz)

Write $U=A U_0 A^{-1}$, $A\in SU(2)$, and $A^{-1}\dot A=i\boldsymbol\omega\cdot\boldsymbol\sigma/2$. The rotational kinetic energy is $\Lambda|\boldsymbol\omega|^2/2$. Since $A$ and $-A$ give the same classical field, the physical orientation space is $SO(3)$, covered by $SU(2)$. For fermionic unit baryons the [Finkelstein-Rubinstein constraints](#finkelstein-rubinstein-constraints) require $\Psi(-A)=-\Psi(A)$. The [SU(2) representations](representation-theory.md#representation-theory-of-su-2) then give half-integer $j$, with [spin angular momentum](quantum-mechanics.md#spin) and [isospin](standard-model.md#isospin) both of magnitude $j$. The rigid-rotor energies are $M+j(j+1)\hbar^2/(2\Lambda)$; the lowest multiplets model the [nucleon](physics.md#nucleon) and [Delta baryon](physics.md#delta-baryon). Large rotational energies can excite deformation and radiation, beyond the rigid approximation.

#### Rational map approximation for Skyrmions

↑ **Parent:** [Skyrmion](#skyrmion)

The rational map approximation writes the angular dependence of a Skyrmion using a rational map $R:S^2\to S^2$ and determines a radial profile variationally. The degree of $R$ equals the baryon number, while zeros of its Wronskian mark directions of vanishing angular baryon density.

##### Cubic rational-map ansatz for four Skyrmions

↑ **Parent:** [Rational map approximation for Skyrmions](#rational-map-approximation-for-skyrmions)

This degree-four [rational map](isolated-singularity.md#rational-map-complex-analysis) obeys $R(iz)=1/R(z)$ and $R((iz+1)/(1-iz))=e^{2\pi i/3}R(z)$. These pair the generators of the [rotational symmetry group of a cube](group-theory.md#rotational-symmetry-group-of-a-cube) with target rotations, giving combined spatial-isospin symmetry in the [Skyrme model](#skyrme-model). Its spatial half-turn kernel is a [Klein four-group](finite-group-theory.md#klein-four-group). The map gives a [cubic four-Skyrmion](#cubic-four-skyrmion) approximation; preserving only its Wronskian zero set does not guarantee the same rotational symmetry.

##### Angular integral in the rational map approximation

↑ **Parent:** [Rational map approximation for Skyrmions](#rational-map-approximation-for-skyrmions)

For a degree-$N$ [rational map](isolated-singularity.md#rational-map-complex-analysis), the [angular Jacobian of a rational map](isolated-singularity.md#angular-jacobian-of-a-rational-map) has average $N$, so the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\mathcal I\geq N^2$. In dimensionless [Skyrme model](#skyrme-model) units the radial energy within the rational-map ansatz is

$$
E=4\pi\int_0^\infty\left[r^2f'^2+2N(f'^2+1)\sin^2f+\mathcal I\frac{\sin^4f}{r^2}\right]dr.
$$

First minimize $\mathcal I$ over admissible maps, then minimize over profiles with $f(0)=\pi$, $f(\infty)=0$. This gives a restricted variational approximation and an upper bound on the unrestricted minimum in that topological sector, not an exact multi-Skyrmion solution. Houghton, Manton and Sutcliffe developed this construction in [https://arxiv.org/abs/hep-th/9705151.](https://arxiv.org/abs/hep-th/9705151.)

#### Finkelstein-Rubinstein constraints

↑ **Parent:** [Skyrmion](#skyrmion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finkelstein-Rubinstein_constraints)

Finkelstein-Rubinstein constraints impose the allowed signs under combined spatial and isospin rotations of a quantized [Skyrmion](#skyrmion). They encode the fermionic or bosonic exchange behavior of topological solitons.

##### Collective-rotation constraints for a Skyrmion

↑ **Parent:** [Finkelstein-Rubinstein constraints](#finkelstein-rubinstein-constraints)

A rigid [Skyrmion](#skyrmion) orientation is quantized on a cover of its [Skyrmion collective-coordinate orbit](#skyrmion-stabilizer-and-collective-coordinate-orbit). A lifted combined rotation in the static field's [stabilizer subgroup](group-theory.md#stabilizer-subgroup) identifies the same classical field and imposes $\widehat D^J(R)\widehat D^I(A)\Psi=\chi_{\rm FR}\Psi$, where the sign is the chosen [Finkelstein-Rubinstein constraints](#finkelstein-rubinstein-constraints) character of that configuration-space loop. Choosing the nontrivial character models unit baryons as fermions. A $2\pi$ spatial rotation or [isorotation](standard-model.md#isorotation) of charge $B$ then has sign $(-1)^B$: deforming the field to separated unit lumps adds the unit-lump loop classes in the [fundamental group](algebraic-topology.md#fundamental-group) $\mathbb Z_2$, while the labelled orbital paths can be contracted in three dimensions. The resulting [Finkelstein-Rubinstein constraints](#finkelstein-rubinstein-constraints) sign is the product of the unit-lump signs. Hence spin and [isospin](standard-model.md#isospin) are half-integer for odd $B$ and integer for even $B$. Further stabilizer constraints restrict which pairs $(J,I)$ and which body-fixed states occur. The [energy](classical-mechanics.md#energy) operator comes from the [inertia tensors](classical-mechanics.md#inertia-tensor) on the orbit; symmetry selects allowed states but does not by itself determine their energies. A bosonic choice of the trivial topological character is mathematically possible but does not model a fermionic [nucleon](physics.md#nucleon).

## ↑ Ancestors (4)

1. [Quantum field theory](quantum-field-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (10)

- [Collective coordinate of a soliton](#collective-coordinate-of-a-soliton)
- [Finite-energy field configuration](#finite-energy-field-configuration)
- [Lorentz boost](special-relativity.md#lorentz-boost)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-70.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-52.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-56.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-47.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-313.md#1/a/solution)
- [Scalar-field vacuum](quantum-field-theory.md#scalar-field-vacuum)
- [Sigma-model lump](quantum-field-theory.md#sigma-model-lump)
