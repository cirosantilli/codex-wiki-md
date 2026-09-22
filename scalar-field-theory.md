# Scalar field theory

↑ **Parent:** [Quantum field theory](quantum-field-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scalar_field_theory)

A scalar field theory describes one or more [Lorentz scalar](special-relativity.md#lorentz-scalar) fields through an [action](classical-mechanics.md#action). The displayed [Lagrangian density](quantum-field-theory.md#lagrangian-density) is a common classical normalization for a [real scalar field](#real-scalar-field); a [complex scalar field](#complex-scalar-field) has two real components. [Canonical quantization](quantum-mechanics.md#canonical-quantization) turns these classical degrees of freedom into operators. The free [real scalar field](#real-scalar-field) gives spin-zero particles, while interactions arise from the potential $V$.

**Table of contents**

- [Stability of a two-scalar quartic potential](#stability-of-a-two-scalar-quartic-potential)
- [Nonrelativistic particle field](#nonrelativistic-particle-field)
- [Real scalar field](#real-scalar-field)
  - [Massless scalar field](#massless-scalar-field)
    - [Minimally coupled massless scalar field](#minimally-coupled-massless-scalar-field)
  - [Real scalar triplet](#real-scalar-triplet)
  - [Sine-Gordon theory](#sine-gordon-theory)
    - [Sine-Gordon breather spectrum at reflectionless couplings](#sine-gordon-breather-spectrum-at-reflectionless-couplings)
      - [Unwrapped reflectionless sine-Gordon transmission phase](#unwrapped-reflectionless-sine-gordon-transmission-phase)
      - [Sine-Gordon breather fusion amplitude](#sine-gordon-breather-fusion-amplitude)
        - [Crossed-channel lightest-breather exchange](#crossed-channel-lightest-breather-exchange)
    - [Sine-Gordon Bäcklund transformation](#sine-gordon-backlund-transformation)
      - [Light-cone normalization of the sine-Gordon Bäcklund transformation](#light-cone-normalization-of-the-sine-gordon-backlund-transformation)
      - [Bianchi permutability for sine-Gordon Bäcklund transformations](#bianchi-permutability-for-sine-gordon-backlund-transformations)
      - [Bäcklund generating current for sine-Gordon conserved charges](#backlund-generating-current-for-sine-gordon-conserved-charges)
        - [Local conserved-charge hierarchy of sine-Gordon theory](#local-conserved-charge-hierarchy-of-sine-gordon-theory)
    - [Sine-Gordon vacuum tadpole counterterm](#sine-gordon-vacuum-tadpole-counterterm)
    - [Sine-Gordon multisoliton tau representation](#sine-gordon-multisoliton-tau-representation)
    - [Sine-Gordon kink](#sine-gordon-kink)
      - [Electromagnetic coupling of a sine-Gordon topological current](#electromagnetic-coupling-of-a-sine-gordon-topological-current)
      - [Sine-Gordon kink-antikink scattering solution](#sine-gordon-kink-antikink-scattering-solution)
        - [Sine-Gordon threshold kink-antikink solution](#sine-gordon-threshold-kink-antikink-solution)
      - [Sine-Gordon two-kink solution](#sine-gordon-two-kink-solution)
        - [Sine-Gordon two-kink time advance](#sine-gordon-two-kink-time-advance)
      - [Sine-Gordon kink fluctuation operator](#sine-gordon-kink-fluctuation-operator)
        - [Translational zero mode of a sine-Gordon kink](#translational-zero-mode-of-a-sine-gordon-kink)
  - [Scalar field configuration eigenstate](#scalar-field-configuration-eigenstate)
  - [Scalar propagator](#scalar-propagator)
    - [Källén–Lehmann spectral representation](#kallen-lehmann-spectral-representation)
      - [Källén–Lehmann spectral density](#kallen-lehmann-spectral-density)
        - [Canonical scalar spectral sum rule](#canonical-scalar-spectral-sum-rule)
    - [Smooth-cutoff scalar propagator](#smooth-cutoff-scalar-propagator)
    - [Shell-restricted scalar propagator](#shell-restricted-scalar-propagator)
  - [Nonminimally coupled scalar field](#nonminimally-coupled-scalar-field)
  - [Internal rotation symmetry of two real scalar fields](#internal-rotation-symmetry-of-two-real-scalar-fields)
    - [Charged oscillator basis of a scalar doublet](#charged-oscillator-basis-of-a-scalar-doublet)
  - [Canonical quantization of a real scalar field](#canonical-quantization-of-a-real-scalar-field)
    - [Covariant oscillator Hamiltonian of a real scalar field](#covariant-oscillator-hamiltonian-of-a-real-scalar-field)
    - [Free real scalar Hamiltonian in oscillator variables](#free-real-scalar-hamiltonian-in-oscillator-variables)
    - [Scalar field oscillator inversion](#scalar-field-oscillator-inversion)
  - [Quartic interaction](#quartic-interaction)
    - [External-leg factorial cancellation at a quartic scalar vertex](#external-leg-factorial-cancellation-at-a-quartic-scalar-vertex)
    - [Six-point amplitudes in phi-fourth theory](#six-point-amplitudes-in-phi-fourth-theory)
    - [One-loop massive phi-fourth counterterms](#one-loop-massive-phi-fourth-counterterms)
      - [Wick-rotated cutoff tadpole mass shift](#wick-rotated-cutoff-tadpole-mass-shift)
    - [One-loop proper vertices of massless phi-fourth theory](#one-loop-proper-vertices-of-massless-phi-fourth-theory)
    - [One-loop quartic scalar beta function](#one-loop-quartic-scalar-beta-function)
      - [Gaussian infrared limit of positive four-dimensional quartic coupling](#gaussian-infrared-limit-of-positive-four-dimensional-quartic-coupling)
      - [Quartic running coupling below four dimensions](#quartic-running-coupling-below-four-dimensions)
    - [Renormalized quartic scalar vertex](#renormalized-quartic-scalar-vertex)
  - [Phi cubed theory](#phi-cubed-theory)
    - [One-loop two-point divergence in six-dimensional cubic scalar theory](#one-loop-two-point-divergence-in-six-dimensional-cubic-scalar-theory)
      - [Minimal-subtraction two-point counterterms in cubic scalar theory](#minimal-subtraction-two-point-counterterms-in-cubic-scalar-theory)
    - [Six-dimensional cubic scalar field theory](#six-dimensional-cubic-scalar-field-theory)
      - [Momentum-cutoff two-point function in six-dimensional cubic scalar theory](#momentum-cutoff-two-point-function-in-six-dimensional-cubic-scalar-theory)
      - [Perturbative renormalizability of cubic scalar theory in six dimensions](#perturbative-renormalizability-of-cubic-scalar-theory-in-six-dimensions)
      - [Cubic scalar box contribution to a quartic coupling](#cubic-scalar-box-contribution-to-a-quartic-coupling)
      - [Scalar shell integral in six dimensions](#scalar-shell-integral-in-six-dimensions)
    - [Four-point tree amplitude in phi cubed theory](#four-point-tree-amplitude-in-phi-cubed-theory)
    - [Five-point tree amplitude in phi cubed theory](#five-point-tree-amplitude-in-phi-cubed-theory)
  - [Phi-six theory](#phi-six-theory)
- [Complex scalar field](#complex-scalar-field)
  - [Complex scalar quartic contact vertex](#complex-scalar-quartic-contact-vertex)
  - [Complex sine-Gordon theory](#complex-sine-gordon-theory)
    - [Charged complex sine-Gordon soliton](#charged-complex-sine-gordon-soliton)
      - [Singular charge endpoint of a complex sine-Gordon soliton](#singular-charge-endpoint-of-a-complex-sine-gordon-soliton)
        - [Integer-level charge identification in complex sine-Gordon theory](#integer-level-charge-identification-in-complex-sine-gordon-theory)
  - [Canonical quantization of a complex scalar field](#canonical-quantization-of-a-complex-scalar-field)
    - [Complex scalar mode inversion](#complex-scalar-mode-inversion)
    - [Complex scalar charge operator](#complex-scalar-charge-operator)
      - [Vacuum subtraction of a complex scalar charge](#vacuum-subtraction-of-a-complex-scalar-charge)
    - [Normal-ordered Hamiltonian of a free complex scalar field](#normal-ordered-hamiltonian-of-a-free-complex-scalar-field)
  - [Global phase symmetry of a complex scalar field](#global-phase-symmetry-of-a-complex-scalar-field)
    - [Noether charge of a complex scalar field](#noether-charge-of-a-complex-scalar-field)

## Stability of a two-scalar quartic potential

↑ **Parent:** [Scalar field theory](scalar-field-theory.md)

For [real scalar fields](#real-scalar-field) with quartic [potential energy](classical-mechanics.md#potential-energy) density $V_4=\lambda(\phi_1^4+\phi_2^4)+2\mu\phi_1^2\phi_2^2$, nonnegativity in every direction is equivalent to the displayed conditions. Necessity follows on an axis and on $\phi_1=\phi_2$. Sufficiency follows by writing $V_4=\lambda(\phi_1^2-\phi_2^2)^2+2(\lambda+\mu)\phi_1^2\phi_2^2$. With a positive quadratic mass term, equality cases still give a stable isolated [classical vacuum](quantum-field-theory.md#classical-vacuum) at the origin. The quartic alone is strictly positive away from the origin precisely when $\lambda>0$ and $\mu>-\lambda$. Rotation symmetry additionally requires $\mu=\lambda$.

## Nonrelativistic particle field

↑ **Parent:** [Scalar field theory](scalar-field-theory.md)

This first-order-in-time field theory has an annihilation-field expansion $\Psi=\int a_{\mathbf p}e^{-i\mathbf p^2t/(2m)+i\mathbf p\cdot\mathbf x}\,d^3p/(2\pi)^3$. Its adjoint creates particles; an [antiparticle](relativistic-quantum-field.md#antiparticle) creation term is not required by a relativistic [mass shell](special-relativity.md#mass-shell) or Lorentz-invariant [microcausality](relativistic-quantum-field.md#microcausality). It is often an effective low-energy sector of a relativistic charged theory after the [antiparticle](relativistic-quantum-field.md#antiparticle) sector is omitted. This does not mean that antimatter cannot be treated nonrelativistically: one may introduce a separate nonrelativistic field for that species.

## Real scalar field

↑ **Parent:** [Scalar field theory](scalar-field-theory.md)

A free real scalar field obeys the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation) and creates neutral spin-zero particles.

### Massless scalar field

↑ **Parent:** [Real scalar field](#real-scalar-field)

A free real [scalar field](quantum-field-theory.md#scalar-field) with zero [mass](classical-mechanics.md#mass) has the displayed wave equation in [Minkowski spacetime](special-relativity.md#minkowski-spacetime). In curved spacetime its dynamics also depend on curvature coupling: a [minimally coupled massless scalar field](#minimally-coupled-massless-scalar-field) and a [conformally coupled scalar field](quantum-field-theory.md#conformally-coupled-scalar-field) need not have the same cosmological modes.

#### Minimally coupled massless scalar field

↑ **Parent:** [Massless scalar field](#massless-scalar-field)

The displayed [action functional](classical-mechanics.md#action) contains no [mass](classical-mechanics.md#mass) term and no $R\phi^2$ curvature coupling. Its [Euler-Lagrange field equation](quantum-field-theory.md#euler-lagrange-field-equation) is $\partial_\mu(\sqrt{-g}\,g^{\mu\nu}\partial_\nu\phi)=0$. In a flat [FLRW metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric), a [Fourier mode](fourier-analysis.md#fourier-mode) obeys $\phi_k''+2(a'/a)\phi_k'+k^2\phi_k=0$ in four dimensions. The expansion can therefore freeze these modes; the curvature term of a [conformally coupled scalar field](quantum-field-theory.md#conformally-coupled-scalar-field) changes that conclusion.

### Real scalar triplet

↑ **Parent:** [Real scalar field](#real-scalar-field)

A [real scalar triplet](#real-scalar-triplet) groups three real scalar components into a vector under [SO(3)](linear-algebra.md#so-3-group). Equivalently it is the three-dimensional [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra) of [SU(2)](topological-group.md#su-2-group), whose center acts trivially. Its rotationally invariant quadratic and quartic potentials depend on $\Phi\cdot\Phi$. A nonzero vacuum direction leaves rotations around that direction unbroken.

### Sine-Gordon theory

↑ **Parent:** [Real scalar field](#real-scalar-field)

A relativistic [real scalar field](#real-scalar-field) theory with a periodic cosine potential. In physical coordinates $y^\mu$, one normalization is $\mathcal L=\tfrac12\partial_\mu\varphi\partial^\mu\varphi-m^2(1-\cos\beta\varphi)/\beta^2$. With $\phi=\beta\varphi$ and $x^\mu=my^\mu$, its [action](classical-mechanics.md#action) is $S=\beta^{-2}\int d^2x[\tfrac12(\partial\phi)^2+\cos\phi-1]$. Its [Euler-Lagrange field equation](quantum-field-theory.md#euler-lagrange-field-equation) is the [Sine-Gordon equation](integrable-systems.md#sine-gordon-equation). Distinct [scalar-field vacua](quantum-field-theory.md#scalar-field-vacuum) differ by $2\pi$ in $\phi$, permitting a [Sine-Gordon kink](#sine-gordon-kink).

#### Sine-Gordon breather spectrum at reflectionless couplings

↑ **Parent:** [Sine-Gordon theory](#sine-gordon-theory)

At renormalized coupling $\gamma=8\pi/n$, the kink-antikink transmission [poles](isolated-singularity.md#pole) lie at $\vartheta=i\pi(1-k/n)$. The [relativistic bound-state mass from a rapidity pole](quantum-mechanics.md#relativistic-bound-state-mass-from-a-rapidity-pole) gives the displayed increasing [breather](classical-field-theory-soliton.md#breather) [masses](classical-mechanics.md#mass). The [kink](classical-field-theory-soliton.md#scalar-field-kink) [mass](classical-mechanics.md#mass) is $M=mn/\pi$, and $k=n$ is an excluded threshold state. No [breathers](classical-field-theory-soliton.md#breather) occur at $n=1$; scattering involving a physical second [breather](classical-field-theory-soliton.md#breather) requires $n\geq3$.

##### Unwrapped reflectionless sine-Gordon transmission phase

↑ **Parent:** [Sine-Gordon breather spectrum at reflectionless couplings](#sine-gordon-breather-spectrum-at-reflectionless-couplings)

For the transmitting product with factors $\cosh[(\theta-i\pi j/N)/2]/\cosh[(\theta+i\pi j/N)/2]$ and prefactor $(-1)^N$, the continuous phase on $\theta\geq0$ is $\pi N-2\sum_{j=1}^{N-1}\arctan[\tanh(\theta/2)\tan(\pi j/(2N))]$. Its derivative is $-\sum_j\sin(\pi j/N)/[\cosh\theta+\cos(\pi j/N)]$. A [Riemann sum](real-analysis.md#riemann-sum) at fixed positive [rapidity](special-relativity.md#rapidity) gives $(2N/\pi)\log\tanh(\theta/2)$ at leading order. The endpoints depend on the stated unwrapped branch; setting the high-energy value to zero silently changes the constant.

##### Sine-Gordon breather fusion amplitude

↑ **Parent:** [Sine-Gordon breather spectrum at reflectionless couplings](#sine-gordon-breather-spectrum-at-reflectionless-couplings)

The second [breather](classical-field-theory-soliton.md#breather) is a bound pair of first [breathers](classical-field-theory-soliton.md#breather) with constituent shifts $\pm ia$. The [bound-state fusion of factorized S-matrices](quantum-field-theory.md#bound-state-fusion-of-factorized-s-matrices) gives $S_{2,1}=S_{1,1}(\vartheta+ia)S_{1,1}(\vartheta-ia)$, which factors as displayed. The nearest physical-strip [pole](isolated-singularity.md#pole) at $\vartheta=ia$ is a crossed-channel exchange of the first [breather](classical-field-theory-soliton.md#breather). At $n=3$ the more distant center [pole](isolated-singularity.md#pole) is double, without changing that nearest-pole interpretation.

###### Crossed-channel lightest-breather exchange

↑ **Parent:** [Sine-Gordon breather fusion amplitude](#sine-gordon-breather-fusion-amplitude)

At the closest physical-strip [pole](isolated-singularity.md#pole) of $S_{2,1}$, the difference of the analytically continued external momenta has squared [mass](classical-mechanics.md#mass) $m_1^2$. Using $m_2=2m_1\cos a$ makes the identity immediate. Thus the exchanged [t-channel](special-relativity.md#scattering-t-channel) one-particle state is the lightest [Sine-Gordon breather](integrable-systems.md#sine-gordon-breather), not a new member of the spectrum.

<h4 id="sine-gordon-backlund-transformation">Sine-Gordon Bäcklund transformation</h4>

↑ **Parent:** [Sine-Gordon theory](#sine-gordon-theory)

For the angular field $u=\beta\phi$ and coordinates $\xi=m(x+t)/2$, $\eta=m(x-t)/2$, let $w=(v+u)/2$ and $d=(v-u)/2$. The displayed relations imply $u_{\xi\eta}=\sin u$ and $v_{\xi\eta}=\sin v$. They define a [Bäcklund transformation](integrable-systems.md#backlund-transformation) with the reciprocal parameter convention used in the [Bianchi permutability for sine-Gordon Bäcklund transformations](#bianchi-permutability-for-sine-gordon-backlund-transformations). Physical-field trigonometric arguments include the coupling $\beta$.

<h5 id="light-cone-normalization-of-the-sine-gordon-backlund-transformation">Light-cone normalization of the sine-Gordon Bäcklund transformation</h5>

↑ **Parent:** [Sine-Gordon Bäcklund transformation](#sine-gordon-backlund-transformation)

For $\tau=x+t$, $\rho=x-t$, the unit-mass [Sine-Gordon equation](integrable-systems.md#sine-gordon-equation) is $\phi_{\tau\rho}=\tfrac14\sin\phi$. An auto-[Bäcklund transformation](integrable-systems.md#backlund-transformation) with these coordinates is

$$
(\phi_1-\phi_0)_\rho=b\sin\frac{\phi_1+\phi_0}{2},\qquad
(\phi_1+\phi_0)_\tau=b^{-1}\sin\frac{\phi_1-\phi_0}{2}.
$$

Differentiate each relation in the other coordinate and add or subtract; the sine addition formula gives $\phi_{j,\tau\rho}=\tfrac14\sin\phi_j$ for $j=0,1$. Doubling both right-hand sides instead gives $\phi_{j,\tau\rho}=\sin\phi_j$, hence a sine-Gordon equation with mass squared four. Those doubled coefficients are appropriate for the half-scaled coordinates $(x+t)/2,(x-t)/2$.

<h5 id="bianchi-permutability-for-sine-gordon-backlund-transformations">Bianchi permutability for sine-Gordon Bäcklund transformations</h5>

↑ **Parent:** [Sine-Gordon Bäcklund transformation](#sine-gordon-backlund-transformation)

Two compatible Bäcklund steps commute after integration constants are matched. The displayed superposition relation constructs their common output algebraically from the seed and the two one-step outputs, in the reciprocal-parameter convention of the [Sine-Gordon Bäcklund transformation](#sine-gordon-backlund-transformation). It uses the angular field $u=\beta\phi$. Smooth inverse-tangent branch continuation is required to retain the correct vacuum labels.

<h5 id="backlund-generating-current-for-sine-gordon-conserved-charges">Bäcklund generating current for sine-Gordon conserved charges</h5>

↑ **Parent:** [Sine-Gordon Bäcklund transformation](#sine-gordon-backlund-transformation)

Write the transformed angular field as $v=u+2d$. The [Sine-Gordon Bäcklund transformation](#sine-gordon-backlund-transformation) gives $\sin d=a(u_\xi+d_\xi)$, determining $d$ as a formal local derivative expansion in $a$. The displayed exact current identity yields a [conservation law](physics.md#conservation-law) at each order. Formal convergence is unnecessary because each coefficient obeys an exact identity on solutions.

###### Local conserved-charge hierarchy of sine-Gordon theory

↑ **Parent:** [Bäcklund generating current for sine-Gordon conserved charges](#backlund-generating-current-for-sine-gordon-conserved-charges)

The Bäcklund expansion produces local differential-polynomial currents. In the coordinates $\xi=m(x+t)/2$, $\eta=m(x-t)/2$, their charges are $\int(P_j+Q_j)dx$ with vanishing boundary flux. Derivative improvements contribute no new charge. The first nontrivial higher current can be written $P=u_{\xi\xi}^2-u_\xi^4/4$, $Q=\cos u\,u_\xi^2$. Continuing, and exchanging light-cone directions, produces the infinite higher-spin hierarchy characterizing [classical integrability](integrable-systems.md#classical-integrability).

#### Sine-Gordon vacuum tadpole counterterm

↑ **Parent:** [Sine-Gordon theory](#sine-gordon-theory)

With canonical field $\varphi=\phi/\beta$, the quartic interaction has coupling $-m^2\beta^2$. Cancelling the vacuum [tadpole diagram](perturbative-quantum-field-theory.md#tadpole-diagram) requires the divergent [mass counterterm](perturbative-quantum-field-theory.md#mass-counterterm) $\delta m^2=(m^2\beta^2/4)\int_{-\Lambda}^{\Lambda}dk/[2\pi\sqrt{k^2+1}]$. Its [kink](classical-field-theory-soliton.md#scalar-field-kink) energy is $\Delta M_{\rm ct}=4\delta m^2/(m\beta^2)$ because $\int(1-\cos\phi_K)dx=4$. This cancels the logarithmic [ultraviolet divergence](perturbative-quantum-field-theory.md#ultraviolet-divergence) in the [one-loop soliton mass correction](classical-field-theory-soliton.md#one-loop-soliton-mass-correction). Finite parts depend on the [renormalization condition](perturbative-quantum-field-theory.md#renormalization-condition).

#### Sine-Gordon multisoliton tau representation

↑ **Parent:** [Sine-Gordon theory](#sine-gordon-theory)

For real parameters with $\kappa_i^2-b_i^2=1$, set $E_i=e^{\kappa_i x-b_i t+\gamma_i}$ and $a_{ij}=[(\kappa_i-\kappa_j)^2-(b_i-b_j)^2]/[(\kappa_i+\kappa_j)^2-(b_i+b_j)^2]$. Sum $\prod_i E_i^{\mu_i}\prod_{i<j}a_{ij}^{\mu_i\mu_j}$ over binary vectors of even parity for $f$ and odd parity for $g$. The [Sine-Gordon equation](integrable-systems.md#sine-gordon-equation) solution is the continuous field $4\arg(f+ig)$. In the all-[kink](classical-field-theory-soliton.md#scalar-field-kink) sector, $\kappa_i=\cosh\theta_i$, $b_i=\sinh\theta_i$ and $a_{ij}=-\tanh^2[(\theta_i-\theta_j)/2]$. Treating these coefficients as positive would change the solution. Distinct [rapidities](special-relativity.md#rapidity) give separated incoming and outgoing [solitons](integrable-systems.md#soliton).

#### Sine-Gordon kink

↑ **Parent:** [Sine-Gordon theory](#sine-gordon-theory)

The static [kink](classical-field-theory-soliton.md#scalar-field-kink) $\phi_K(x)=4\arctan e^{x-a}$ joins adjacent [scalar-field vacua](quantum-field-theory.md#scalar-field-vacuum) $0$ and $2\pi$. It obeys $\phi_K'=2\operatorname{sech}(x-a)$ and has [topological charge](classical-field-theory-soliton.md#topological-charge) $Q=[\phi(+\infty)-\phi(-\infty)]/(2\pi)=1$. In the [Sine-Gordon theory](#sine-gordon-theory) normalization with physical mass scale $m$ and coupling $\beta$, its classical [mass](classical-mechanics.md#mass) is $8m/\beta^2$. A [Lorentz boost](special-relativity.md#lorentz-boost) gives $\phi_K=4\arctan\exp[(x-vt-a)/\sqrt{1-v^2}]$. Spatial reflection gives an [antikink](classical-field-theory-soliton.md#antikink).

##### Electromagnetic coupling of a sine-Gordon topological current

↑ **Parent:** [Sine-Gordon kink](#sine-gordon-kink)

The identically conserved [topological current](classical-field-theory-soliton.md#topological-current) $j$ couples to an external electromagnetic [gauge potential](relativistic-quantum-field.md#gauge-field) through $-A_\mu j^\mu=-A_0\theta_x+A_1\theta_t$. A [gauge transformation](electromagnetism.md#gauge-transformation) changes this coupling only by a divergence. The [Euler-Lagrange field equation](quantum-field-theory.md#euler-lagrange-field-equation) becomes $\theta_{tt}-\theta_{xx}+\sin\theta+E=0$, with $E=\partial_tA_1-\partial_xA_0$. A unit [Sine-Gordon kink](#sine-gordon-kink) has unnormalized charge $Q=2\pi$ and mass $8$. For spatially uniform forcing, its field momentum balance is $\dot P=QE$ when the boundary stress contributions cancel.

##### Sine-Gordon kink-antikink scattering solution

↑ **Parent:** [Sine-Gordon kink](#sine-gordon-kink)

This localized two-soliton field has zero net winding and describes an elastic kink-antikink collision for $0<v<1$. Two reciprocal positive Bäcklund parameters produce it from the vacuum. Analytic continuation of $v$ to an imaginary value gives a real [Sine-Gordon breather](integrable-systems.md#sine-gordon-breather). The overall field sign and spacetime translations change conventions, not the field equation.

###### Sine-Gordon threshold kink-antikink solution

↑ **Parent:** [Sine-Gordon kink-antikink scattering solution](#sine-gordon-kink-antikink-scattering-solution)

The zero-relative-speed limit of the [Sine-Gordon kink-antikink scattering solution](#sine-gordon-kink-antikink-scattering-solution) is a [separatrix](dynamical-systems.md#separatrix) at twice the rest-kink energy. A [Sine-Gordon Bäcklund transformation](#sine-gordon-backlund-transformation) of the static [kink](classical-field-theory-soliton.md#scalar-field-kink) with equal parameter gives $p_x=-p\tanh x$, $p_t=\operatorname{sech}x$ for $p=\tan(\phi/4)$, hence the displayed solution. The two asymptotic transitions separate logarithmically in time and their speeds tend to zero; this is not a finite-period [Sine-Gordon breather](integrable-systems.md#sine-gordon-breather).

##### Sine-Gordon two-kink solution

↑ **Parent:** [Sine-Gordon kink](#sine-gordon-kink)

For $0<v<1$ and $\Gamma=(1-v^2)^{-1/2}$, this real two-soliton solution has angular winding $4\pi$. Its separated [kink](classical-field-theory-soliton.md#scalar-field-kink) velocities are $\pm v$. At large times the centers satisfy $|m\Gamma x|=|m\Gamma vt|-\log v+o(1)$, giving a right-moving shift $-2\log v/(m\Gamma)$. It follows from [Bianchi permutability for sine-Gordon Bäcklund transformations](#bianchi-permutability-for-sine-gordon-backlund-transformations) with oppositely signed seed parameters.

###### Sine-Gordon two-kink time advance

↑ **Parent:** [Sine-Gordon two-kink solution](#sine-gordon-two-kink-solution)

For two equal-charge [Sine-Gordon kinks](#sine-gordon-kink) with speeds $\pm v$, $0<v<1$, the positive spatial transition satisfies $X_+(T)=v|T|-\log v/(m\gamma)+o(1)$, where $\gamma=(1-v^2)^{-1/2}$. Labeling a [soliton](integrable-systems.md#soliton) by its preserved [rapidity](special-relativity.md#rapidity), the right-moving incoming and outgoing intercepts differ by $-2\log v/(m\gamma)$. The [soliton time delay](classical-field-theory-soliton.md#soliton-time-delay) at a fixed distant location is minus this shift divided by $v$, giving the displayed negative value. Reversing the entire field gives two [antikinks](classical-field-theory-soliton.md#antikink) with the same shifts. The sign means an advance relative to extrapolation of the incoming line; labels tied to left and right positions instead exchange [velocities](classical-mechanics.md#velocity) during reflection.

##### Sine-Gordon kink fluctuation operator

↑ **Parent:** [Sine-Gordon kink](#sine-gordon-kink)

The [second variation](calculus-of-variations.md#second-variation) of the [Sine-Gordon theory](#sine-gordon-theory) action about its static [kink](classical-field-theory-soliton.md#scalar-field-kink) gives $\Delta_x=-\partial_x^2+1-2\operatorname{sech}^2x$. Let $A=\partial_x+\tanh x$. Then $\Delta_x=A^\dagger A$ and $AA^\dagger=-\partial_x^2+1$. Thus $\Delta_x$ is nonnegative, with its [translational zero mode of a sine-Gordon kink](#translational-zero-mode-of-a-sine-gordon-kink) and a continuum at $\omega^2=k^2+1$. The construction is the [supersymmetric factorization of the one-soliton potential](quantum-mechanics.md#supersymmetric-factorization-of-the-one-soliton-potential).

###### Translational zero mode of a sine-Gordon kink

↑ **Parent:** [Sine-Gordon kink fluctuation operator](#sine-gordon-kink-fluctuation-operator)

The normalized [eigenfunction](linear-operator-theory.md#eigenfunction) $\psi_0(x)=\operatorname{sech}x/\sqrt2$ has zero [eigenvalue](linear-operator-theory.md#eigenvalue) under the [Sine-Gordon kink fluctuation operator](#sine-gordon-kink-fluctuation-operator). It is proportional to $\partial_x\phi_K$ and comes from shifting the [collective coordinate](classical-field-theory-soliton.md#collective-coordinate-of-a-soliton) of the [kink](classical-field-theory-soliton.md#scalar-field-kink). Its frequency is zero, so it contributes no oscillator [zero-point energy](quantum-mechanics.md#zero-point-energy); it must be handled separately from a Gaussian [functional determinant](quantum-field-theory.md#functional-determinant).

### Scalar field configuration eigenstate

↑ **Parent:** [Real scalar field](#real-scalar-field)

A [scalar field configuration eigenstate](#scalar-field-configuration-eigenstate) assigns eigenvalues of the equal-time field operator at every spatial point. These generalized states play the role of position eigenstates for a system of infinitely many coordinates. Inserting their regulated completeness relations on time slices constructs the [scalar field path integral](quantum-field-theory.md#scalar-field-path-integral).

### Scalar propagator

↑ **Parent:** [Real scalar field](#real-scalar-field)

For a free massive scalar in a [Euclidean path integral](quantum-field-theory.md#euclidean-path-integral), inversion of the quadratic kernel gives $\Delta_E(p)=1/(p^2+m^2)$. The Minkowski version follows by [Wick rotation](perturbative-quantum-field-theory.md#wick-rotation).

<h4 id="kallen-lehmann-spectral-representation">Källén–Lehmann spectral representation</h4>

↑ **Parent:** [Scalar propagator](#scalar-propagator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Källén–Lehmann_spectral_representation)

For a Hermitian [scalar field](quantum-field-theory.md#scalar-field) in a positive-norm [Hilbert space](hilbert-space.md) with a Lorentz-invariant vacuum, the [spectrum condition](quantum-field-theory.md#spectrum-condition) and completeness give the connected vacuum two-point function as a superposition of free mass-shell functions. Define the [Källén–Lehmann spectral density](#kallen-lehmann-spectral-density) by $\widetilde W(p)=2\pi\theta(p^0)\rho(p^2)$, where $W(x)=\langle0|\phi(x)\phi(0)|0\rangle$ and its [vacuum expectation value](quantum-field-theory.md#vacuum-expectation-value) has been subtracted if nonzero. Squared intermediate-state matrix elements make $\rho$ a nonnegative measure supported on nonnegative mass squared. Applying [time ordering](perturbative-quantum-field-theory.md#time-ordering) to each free mass shell gives the displayed [Feynman propagator](quantum-field-theory.md#feynman-propagator) representation, using $i\Delta=\langle T\phi\phi\rangle$ and signature $(+---)$. Its positivity does not automatically extend to gauge-variant fields in an indefinite auxiliary space.

<h5 id="kallen-lehmann-spectral-density">Källén–Lehmann spectral density</h5>

↑ **Parent:** [Källén–Lehmann spectral representation](#kallen-lehmann-spectral-representation)

The [Källén–Lehmann spectral density](#kallen-lehmann-spectral-density) is the nonnegative invariant-mass measure in a scalar vacuum two-point function. With complete intermediate states it satisfies $2\pi\theta(p^0)\rho(p^2)=(2\pi)^4\sum_\alpha|\langle\alpha|\phi(0)|0\rangle|^2\delta^4(p-p_\alpha)$, with continuous state measures included in the sum. A stable one-particle state of mass $m$, with covariant normalization and squared field overlap $Z$, contributes $Z\delta(\sigma-m^2)$. Other particles and multiparticle states contribute additional nonnegative weight. The isolated pole of the [scalar propagator](#scalar-propagator) then has residue $Z$.

###### Canonical scalar spectral sum rule

↑ **Parent:** [Källén–Lehmann spectral density](#kallen-lehmann-spectral-density)

For a [real scalar field](#real-scalar-field) with [canonical field normalization](perturbative-quantum-field-theory.md#canonical-field-normalization), impose $[\dot\phi(t,\mathbf x),\phi(t,\mathbf y)]=-i\delta^3(\mathbf x-\mathbf y)$. The [Källén–Lehmann spectral representation](#kallen-lehmann-spectral-representation) also represents its vacuum commutator as the weighted sum of free commutators. The equal-time derivative of each free commutator is $-i\delta^3(\mathbf x-\mathbf y)$ independently of mass. Comparison therefore gives the displayed sum rule, whenever the canonical commutator and spectral integral admit this distributional limit. Since the measure is nonnegative, an isolated one-particle weight obeys $0\leq Z\leq1$, and is strictly positive if the field couples to that particle. Arbitrary rescaling of the field rescales the total spectral weight, so positivity alone does not imply this normalization or upper bound.

#### Smooth-cutoff scalar propagator

↑ **Parent:** [Scalar propagator](#scalar-propagator)

A [smooth-cutoff scalar propagator](#smooth-cutoff-scalar-propagator) is the inverse of a positive regulated quadratic kernel. It agrees with the unregulated [scalar propagator](#scalar-propagator) at low [momentum](classical-mechanics.md#momentum) and decreases rapidly at high [momentum](classical-mechanics.md#momentum). Smooth suppression is not identical to vanishing support. Its cutoff derivative is the line weight in an exact [renormalization-group flow](critical-phenomenon.md#renormalization-group-flow).

#### Shell-restricted scalar propagator

↑ **Parent:** [Scalar propagator](#scalar-propagator)

The Gaussian contraction used while integrating out a momentum shell. Its Fourier support lies entirely in that shell. In particular, convolution with a purely low-momentum field is zero. This distinguishes shell [Feynman diagrams](perturbative-quantum-field-theory.md#feynman-diagram) from unrestricted loop diagrams.

### Nonminimally coupled scalar field

↑ **Parent:** [Real scalar field](#real-scalar-field)

A nonminimal scalar coupling includes an interaction between the field and spacetime curvature, such as $-\xi R\Phi^2$ in the [Lagrangian density](quantum-field-theory.md#lagrangian-density). The [Euler-Lagrange field equation](quantum-field-theory.md#euler-lagrange-field-equation) for $\mathcal L=-\frac12(\nabla\Phi)^2-\xi R\Phi^2$ is $\Box\Phi-2\xi R\Phi=0$. The coefficient is convention dependent: an action written with $-\frac12\xi R\Phi^2$ has $\xi$ instead of $2\xi$.

### Internal rotation symmetry of two real scalar fields

↑ **Parent:** [Real scalar field](#real-scalar-field)

For two free [real scalar fields](#real-scalar-field), the internal rotation $\delta\phi_1=\theta\phi_2$, $\delta\phi_2=-\theta\phi_1$ is a symmetry precisely when their squared masses agree. Its [Noether current](quantum-field-theory.md#noether-current) is $j^\mu=\phi_2\partial^\mu\phi_1-\phi_1\partial^\mu\phi_2$. Without mass degeneracy, $\partial_\mu j^\mu=(m_2^2-m_1^2)\phi_1\phi_2$.

#### Charged oscillator basis of a scalar doublet

↑ **Parent:** [Internal rotation symmetry of two real scalar fields](#internal-rotation-symmetry-of-two-real-scalar-fields)

For the [internal rotation symmetry of two real scalar fields](#internal-rotation-symmetry-of-two-real-scalar-fields) with $\delta\phi_1=\alpha\phi_2$ and $\delta\phi_2=-\alpha\phi_1$, the [Noether charge](quantum-field-theory.md#noether-charge) is $Q=i\int(a_1^\dagger a_2-a_2^\dagger a_1)d^3p/(2\pi)^3$. Its [commutators](lie-algebra.md#commutator) satisfy $[Q,b_\pm^\dagger]=\pm b_\pm^\dagger$, so these [creation operators](quantum-mechanics.md#creation-operator) produce charge [eigenstates](quantum-mechanics.md#eigenstate) in the [one-particle state](quantum-field-theory.md#one-particle-state) sector. Substitution gives $Q=N_+-N_-$, converting the rotation of real components into opposite charges in a complex basis.

### Canonical quantization of a real scalar field

↑ **Parent:** [Real scalar field](#real-scalar-field)

The equal-time [canonical commutation relation](quantum-mechanics.md#canonical-commutation-relation) is $[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^3(\mathbf x-\mathbf y)$ in units $\hbar=1$, with the two field-field and momentum-momentum commutators zero. The quadratic [Hamiltonian operator](quantum-mechanics.md#hamiltonian-quantum-mechanics) gives $\dot\phi=\pi$ and $\dot\pi=\nabla^2\phi-m^2\phi$, hence the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation) as an operator identity.

#### Covariant oscillator Hamiltonian of a real scalar field

↑ **Parent:** [Canonical quantization of a real scalar field](#canonical-quantization-of-a-real-scalar-field)

With $d\Pi_p=d^3p/[(2\pi)^3 2E_p]$, a free [real scalar field](#real-scalar-field) has [mode expansion of a free field](quantum-field-theory.md#mode-expansion-of-a-free-field) $\phi=\int d\Pi_p(ae^{-ipx}+a^\dagger e^{ipx})$ and [commutator](lie-algebra.md#commutator) $[a(p),a^\dagger(q)]=(2\pi)^3 2E_p\delta^3(\mathbf p-\mathbf q)$. Substitution into the quadratic [Hamiltonian density](quantum-field-theory.md#hamiltonian-density) gives $H=\frac12\int d\Pi_p E_p(a^\dagger a+aa^\dagger)$. The terms with two [annihilation operators](quantum-mechanics.md#annihilation-operator) or two [creation operators](quantum-mechanics.md#creation-operator) cancel by $E_p^2=\mathbf p^2+m^2$. [Normal ordering](perturbative-quantum-field-theory.md#normal-ordering) removes the constant [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy). The [commutators](lie-algebra.md#commutator) $[H,a(p)]=-E_pa(p)$ and $[H,a^\dagger(p)]=E_pa^\dagger(p)$ give the [boson](quantum-mechanics.md#boson) energy without changing under this subtraction. Replacing $a(p)$ by $\sqrt{2E_p}\,c(p)$ recovers the noncovariant normalization $[c(p),c^\dagger(q)]=(2\pi)^3\delta^3(\mathbf p-\mathbf q)$.

#### Free real scalar Hamiltonian in oscillator variables

↑ **Parent:** [Canonical quantization of a real scalar field](#canonical-quantization-of-a-real-scalar-field)

Insert the [real scalar field](#real-scalar-field) mode expansion into its quadratic [Hamiltonian density](quantum-field-theory.md#hamiltonian-density) and use the [Fourier representation of the Dirac delta function](distribution-theory.md#fourier-representation-of-the-dirac-delta-function). The two-annihilator and two-creator terms cancel by $E_{\mathbf p}^2=\mathbf p^2+m^2$. The remaining symmetric expression is $H=\frac12\int d^3p\,E_{\mathbf p}(a^\dagger a+aa^\dagger)/(2\pi)^3$. [Normal ordering](perturbative-quantum-field-theory.md#normal-ordering) removes its constant [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy), yielding the displayed operator. The [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) give $[:H:,a_{\mathbf p}]=-E_{\mathbf p}a_{\mathbf p}$ and $[:H:,a^\dagger_{\mathbf p}]=E_{\mathbf p}a^\dagger_{\mathbf p}$.

#### Scalar field oscillator inversion

↑ **Parent:** [Canonical quantization of a real scalar field](#canonical-quantization-of-a-real-scalar-field)

For the [real scalar field](#real-scalar-field) expansion $\phi=\int d^3p\,[a_{\mathbf p}e^{-ipx}+a^\dagger_{\mathbf p}e^{ipx}]/((2\pi)^3\sqrt{2E_{\mathbf p}})$, the equal-time fields extract $a_{\mathbf p}=e^{iEt}\int d^3x\,e^{-i\mathbf p\cdot\mathbf x}[\sqrt{E/2}\,\phi+i\pi/\sqrt{2E}]$. The two mixed [canonical commutation relation](quantum-mechanics.md#canonical-commutation-relation) terms yield $[a_{\mathbf p},a^\dagger_{\mathbf q}]=(2\pi)^3\delta^3(\mathbf p-\mathbf q)$, while the other oscillator [commutators](lie-algebra.md#commutator) vanish. This verifies the normalization of the mode expansion directly from the canonical fields.

### Quartic interaction

↑ **Parent:** [Real scalar field](#real-scalar-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quartic_interaction)

Phi-fourth theory has a scalar interaction $-\lambda\phi^4/4!$. In four dimensions its coupling is classically marginal, and its one-loop four-point function receives bubble corrections in the three Mandelstam channels.

#### External-leg factorial cancellation at a quartic scalar vertex

↑ **Parent:** [Quartic interaction](#quartic-interaction)

For a real [scalar field](quantum-field-theory.md#scalar-field) with interaction $-\lambda\phi^4/4!$, the first [Dyson series](perturbative-quantum-field-theory.md#dyson-series) term is $-i\lambda\int\phi^4d^4x/4!$. Four labeled external legs can attach to the four fields in $4!$ ways, or in $\binom42\,2!\,2!=24$ ways after separating incoming and outgoing legs. The factorial cancels and spacetime integration supplies the [four-momentum conservation](special-relativity.md#four-momentum-conservation) delta function. This gives the connected tree [scattering amplitude](quantum-mechanics.md#scattering-amplitude) $-\lambda$. The separate [identical final-state symmetry factor](quantum-mechanics.md#identical-particle-factor-in-a-final-state-phase-space-integral) belongs in the event phase-space integral and is not another vertex factor.

#### Six-point amplitudes in phi-fourth theory

↑ **Parent:** [Quartic interaction](#quartic-interaction)

For a connected six-external-leg [Feynman diagram](perturbative-quantum-field-theory.md#feynman-diagram) made from quartic vertices, $4V=6+2I$ and $L=I-V+1$ give $V=L+2$, $I=2L+1$. A tree therefore has two vertices and one internal line; partitioning six labelled external legs into two triples gives ten tree channels. A one-loop triangle has three vertices, three internal lines and two external legs at each vertex. With external labels fixed, that triangle has [symmetry factor](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) one. Other one-loop topologies also contribute to the full amplitude.

#### One-loop massive phi-fourth counterterms

↑ **Parent:** [Quartic interaction](#quartic-interaction)

With interaction $-\mu^\epsilon\lambda\phi^4/4!$ and $d=4-\epsilon$, the two-point [tadpole diagram](perturbative-quantum-field-theory.md#tadpole-diagram) has [symmetry factor](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) $1/2$. The [Euclidean massive loop integral](perturbative-quantum-field-theory.md#euclidean-massive-loop-integral) gives its pole through $I_{d,1}=-m^2/(8\pi^2\epsilon)+O(1)$. The three four-point [bubble diagrams](perturbative-quantum-field-theory.md#bubble-diagram) each have symmetry factor $1/2$, and the [massive scalar bubble pole in four dimensions](perturbative-quantum-field-theory.md#massive-scalar-bubble-pole-in-four-dimensions) gives the quartic counterterm. The tadpole is independent of external [momentum](classical-mechanics.md#momentum), so no one-loop [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization) is required. A vacuum-energy counterterm is additionally needed if vacuum diagrams are retained.

##### Wick-rotated cutoff tadpole mass shift

↑ **Parent:** [One-loop massive phi-fourth counterterms](#one-loop-massive-phi-fourth-counterterms)

With interaction $-\lambda_0\phi^4/4!$, the [tadpole diagram](perturbative-quantum-field-theory.md#tadpole-diagram) has [symmetry factor](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) one half. After [Wick rotation](perturbative-quantum-field-theory.md#wick-rotation) and a rotationally invariant Euclidean cutoff, its [self-energy](perturbative-quantum-field-theory.md#self-energy) is $(\lambda_0/2)\int_{|k|<\Lambda}d^4k\,(2\pi)^{-4}(k^2+m_0^2)^{-1}$. The sphere area $2\pi^2$ and radial integral $\int_0^\Lambda k^3dk/(k^2+m_0^2)=\tfrac12[\Lambda^2-m_0^2\log(1+\Lambda^2/m_0^2)]$ give the displayed shift. It is independent of external momentum, so no one-loop momentum-dependent [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization) arises from this graph. Different regulator schemes can treat power divergences differently while defining the same chosen [pole mass](perturbative-quantum-field-theory.md#pole-mass).

#### One-loop proper vertices of massless phi-fourth theory

↑ **Parent:** [Quartic interaction](#quartic-interaction)

The [interaction vertex](perturbative-quantum-field-theory.md#interaction-vertex) $-i\lambda$ and [scalar propagator](#scalar-propagator) $-i/(p^2-i\epsilon)$ give one four-point [bubble diagram](perturbative-quantum-field-theory.md#bubble-diagram) for each of three [momentum](classical-mechanics.md#momentum) channels, each with [Feynman-diagram symmetry factor](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) $1/2$. The two-point [tadpole diagram](perturbative-quantum-field-theory.md#tadpole-diagram) is zero as a scaleless integral in [dimensional regularization](perturbative-quantum-field-theory.md#dimensional-regularization). If full proper vertices include the free quadratic kernel, $\widehat\tau_2^{(0)}=-p^2$; the interaction self-energy convention instead starts at zero.

#### One-loop quartic scalar beta function

↑ **Parent:** [Quartic interaction](#quartic-interaction)

With interaction $\lambda\phi^4/4!$ for one real scalar, the three one-loop four-point bubble channels give the four-dimensional [renormalization-group beta function](perturbative-quantum-field-theory.md#beta-function-physics) $\beta(\lambda)=3\lambda^2/(16\pi^2)+O(\lambda^3)$. Its positive sign for $\lambda>0$ excludes [asymptotic freedom](perturbative-quantum-field-theory.md#asymptotic-freedom) and produces a perturbative [Landau pole](perturbative-quantum-field-theory.md#landau-pole) on extrapolation.

##### Gaussian infrared limit of positive four-dimensional quartic coupling

↑ **Parent:** [One-loop quartic scalar beta function](#one-loop-quartic-scalar-beta-function)

For a positive weak [quartic scalar field theory](#quartic-interaction) coupling in four dimensions, the one-loop [renormalization-group beta function](perturbative-quantum-field-theory.md#beta-function-physics) is $\beta=a\lambda^2$, $a=3/(16\pi^2)>0$. Integration gives the displayed inverse-coupling law, so $\lambda$ tends to zero logarithmically as $\mu\to0$ and grows toward the ultraviolet. The interacting [Wilson-Fisher fixed point](critical-phenomenon.md#wilson-fisher-fixed-point) of $4-\epsilon$ dimensions merges with the [Gaussian fixed point](critical-phenomenon.md#gaussian-fixed-point) at $\epsilon=0$. This describes the quartic direction in the massless or critically tuned infrared regime, not disappearance of every finite-energy interaction in a massive theory. The ultraviolet [Landau pole](perturbative-quantum-field-theory.md#landau-pole) signals breakdown of that perturbative extrapolation; one loop alone does not prove a nonperturbative triviality theorem.

##### Quartic running coupling below four dimensions

↑ **Parent:** [One-loop quartic scalar beta function](#one-loop-quartic-scalar-beta-function)

At quadratic order, $\mu\,d\lambda/d\mu=-\epsilon\lambda+3\lambda^2/(16\pi^2)$ for $\epsilon>0$. Solving the linear equation for $1/\lambda$ gives the displayed expression. If $0<\lambda(\mu_0)<\lambda_*$, the ultraviolet limit is zero and the infrared limit is $\lambda_*$. Initial data above $\lambda_*$ reach a [Landau pole](perturbative-quantum-field-theory.md#landau-pole) at a finite ultraviolet scale. The interacting value is the [Wilson-Fisher fixed point](critical-phenomenon.md#wilson-fisher-fixed-point) along the quartic coupling direction; the full scalar theory also has a [thermal relevant direction at the Wilson-Fisher fixed point](critical-phenomenon.md#thermal-relevant-direction-at-the-wilson-fisher-fixed-point), so a critical infrared limit requires mass tuning.

#### Renormalized quartic scalar vertex

↑ **Parent:** [Quartic interaction](#quartic-interaction)

### Phi cubed theory

↑ **Parent:** [Real scalar field](#real-scalar-field)

Phi cubed theory has interaction $-g\phi^3/3!$, giving a cubic vertex $-ig$. In four spacetime dimensions the scalar field has mass dimension one and $g$ has mass dimension one.

#### One-loop two-point divergence in six-dimensional cubic scalar theory

↑ **Parent:** [Phi cubed theory](#phi-cubed-theory)

The two-vertex cubic bubble in $d=6-\epsilon$ dimensions has the displayed amputated pole. A [Feynman parameter](perturbative-quantum-field-theory.md#feynman-parameter) gives mass $m^2+x(1-x)k^2$, and $\Gamma(-1+\epsilon/2)$ supplies the pole. The full propagator receives $D_0^2 I$, while its inverse receives $-I$. This sign distinguishes a two-point insertion from an inverse-propagator correction.

##### Minimal-subtraction two-point counterterms in cubic scalar theory

↑ **Parent:** [One-loop two-point divergence in six-dimensional cubic scalar theory](#one-loop-two-point-divergence-in-six-dimensional-cubic-scalar-theory)

With additive [counterterms](perturbative-quantum-field-theory.md#counterterm) $\tfrac12\delta Z(\partial\phi)^2+\tfrac12\delta m^2\phi^2$, their Euclidean propagator insertion is $-(\delta Zk^2+\delta m^2)$. These [minimal subtraction scheme](perturbative-quantum-field-theory.md#minimal-subtraction-scheme) coefficients cancel the cubic bubble insertion. A bare mass shift also subtracts $m^2\delta Z$ after [wavefunction renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization); it is not the same coefficient as the additive mass counterterm.

#### Six-dimensional cubic scalar field theory

↑ **Parent:** [Phi cubed theory](#phi-cubed-theory)

A canonically normalized [real scalar field](#real-scalar-field) in six dimensions has [mass dimension](perturbative-quantum-field-theory.md#mass-dimension) two. The cubic coupling is classically a [marginal coupling](perturbative-quantum-field-theory.md#marginal-coupling), whereas a local quartic coupling has [mass dimension](perturbative-quantum-field-theory.md#mass-dimension) minus two. This theory is perturbatively renormalizable by [power counting in quantum field theory](perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory), but a real cubic Euclidean potential is unbounded below. Its expansion about a massive Gaussian theory is therefore formal perturbation theory, not a convergent positive functional integral at nonzero real $g$.

##### Momentum-cutoff two-point function in six-dimensional cubic scalar theory

↑ **Parent:** [Six-dimensional cubic scalar field theory](#six-dimensional-cubic-scalar-field-theory)

The [self-energy](perturbative-quantum-field-theory.md#self-energy) [bubble diagram](perturbative-quantum-field-theory.md#bubble-diagram) at [loop order](perturbative-quantum-field-theory.md#loop-order) one in [six-dimensional cubic scalar field theory](#six-dimensional-cubic-scalar-field-theory) has [Feynman-diagram symmetry factor](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) two. With positive Euclidean [scalar propagators](#scalar-propagator), its [amputated Green's function](critical-phenomenon.md#amputated-connected-correlation-function) is the displayed integral. Its [superficial degree of divergence](perturbative-quantum-field-theory.md#superficial-degree-of-divergence) is two. Expanding at large internal momentum and taking the angular average shows that its divergent part is a constant plus a multiple of $p^2$, precisely the [mass counterterm](perturbative-quantum-field-theory.md#mass-counterterm) and [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization) structures.

For a spherical [ultraviolet cutoff](quantum-field-theory.md#ultraviolet-cutoff) $|k|\leq\Lambda$ and $m^2>0$, its value at $p=0$ is

$$
B_\Lambda=\frac{g^2}{256\pi^3}\left[\Lambda^2-2m^2\log\left(1+\frac{\Lambda^2}{m^2}\right)+\frac{m^2\Lambda^2}{\Lambda^2+m^2}\right].
$$

The divergent $p^2$ coefficient is $-g^2\log(\Lambda^2/m^2)/(768\pi^3)$. Finite terms depend on the [regularization](statistical-learning.md#regularization) convention. [Tadpole diagram](perturbative-quantum-field-theory.md#tadpole-diagram) insertions are excluded from the [one-particle-irreducible Feynman diagram](perturbative-quantum-field-theory.md#one-particle-irreducible-feynman-diagram), and are removed from the connected [two-point function](critical-phenomenon.md#two-point-correlation-function) by imposing a vanishing [one-point function](critical-phenomenon.md#one-point-correlation-function).

##### Perturbative renormalizability of cubic scalar theory in six dimensions

↑ **Parent:** [Six-dimensional cubic scalar field theory](#six-dimensional-cubic-scalar-field-theory)

For a cubic graph with $E$ external legs, $3V=2I+E$ and $L=I-V+1$. Its [superficial degree of divergence](perturbative-quantum-field-theory.md#superficial-degree-of-divergence) is therefore $6L-2I=6-2E$. Divergences in vacuum, one-, two-, and three-point functions can be absorbed into vacuum energy, a linear term, mass, [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization), and cubic-coupling [counterterms](perturbative-quantum-field-theory.md#counterterm). Higher-point proper diagrams are superficially convergent after subtraction of divergent subgraphs. This establishes perturbative renormalizability, without asserting a nonperturbative positive measure for the unstable real cubic potential.

##### Cubic scalar box contribution to a quartic coupling

↑ **Parent:** [Six-dimensional cubic scalar field theory](#six-dimensional-cubic-scalar-field-theory)

In a [six-dimensional cubic scalar field theory](#six-dimensional-cubic-scalar-field-theory), three labelled [box Feynman diagrams](perturbative-quantum-field-theory.md#box-feynman-diagram) give the one-loop local quartic vertex at zero external momentum. With an effective-action term $g_4\phi^4/4!$, their contribution is $\delta g_4=-3g^4I_4$. To check its sign and multiplicity, expand the [one-loop scalar effective action](perturbative-quantum-field-theory.md#one-loop-scalar-effective-action) as $\tfrac12\operatorname{Tr}\log(D+g\phi)$, where $D=-\partial^2+m^2$. Its fourth-order term is $-g^4\operatorname{Tr}(D^{-1}\phi)^4/8$, giving the stated coefficient. The associated amputated connected diagram insertion has the opposite sign.

##### Scalar shell integral in six dimensions

↑ **Parent:** [Six-dimensional cubic scalar field theory](#six-dimensional-cubic-scalar-field-theory)

For $m>0$ and $0<\Lambda<\Lambda_0$, define

$$
I_r=\int_{\Lambda<|q|<\Lambda_0}\frac{d^6q}{(2\pi)^6}(q^2+m^2)^{-r}=\frac1{64\pi^3}\int_\Lambda^{\Lambda_0}\frac{q^5\,dq}{(q^2+m^2)^r}.
$$

The radial formula uses the area $\pi^3$ of the unit five-sphere. Its [mass dimension](perturbative-quantum-field-theory.md#mass-dimension) is $6-2r$. As $\Lambda_0\to\infty$, $I_1$ diverges quartically, $I_2$ quadratically, $I_3$ logarithmically, and $I_r$ is ultraviolet finite for $r\ge4$ at fixed $\Lambda,m$. This follows directly by comparison with $q^{5-2r}$.

#### Four-point tree amplitude in phi cubed theory

↑ **Parent:** [Phi cubed theory](#phi-cubed-theory)

The four-point [tree-level Feynman diagram](perturbative-quantum-field-theory.md#tree-level-feynman-diagram) has two cubic vertices joined by one propagator. The three ways to divide four labeled external legs into vertex pairs give the $s$, $t$, and $u$ channels. For interaction $+\lambda\phi^3/3!$, the amplitude is $\mathcal M=-\lambda^2[(s-m^2)^{-1}+(t-m^2)^{-1}+(u-m^2)^{-1}]$, with the [Feynman i-epsilon prescription](quantum-field-theory.md#feynman-i-epsilon-prescription) understood. All channels interfere in its modulus squared.

#### Five-point tree amplitude in phi cubed theory

↑ **Parent:** [Phi cubed theory](#phi-cubed-theory)

A connected five-point tree in phi cubed theory has three cubic vertices and two internal propagators. For labeled external legs there are fifteen diagrams: choose the leg attached to the middle vertex and partition the other four legs into two unordered pairs.

### Phi-six theory

↑ **Parent:** [Real scalar field](#real-scalar-field)

Phi-six theory has scalar interaction $-\lambda\phi^6/6!$. In four spacetime dimensions its coupling has mass dimension $-2$, and a six-valent vertex contributes the momentum-space factor $-i\lambda$.

## Complex scalar field

↑ **Parent:** [Scalar field theory](scalar-field-theory.md)

A complex scalar field has distinct particle and antiparticle excitations and a global phase symmetry.

### Complex scalar quartic contact vertex

↑ **Parent:** [Complex scalar field](#complex-scalar-field)

For the connected tree [scattering amplitude](quantum-mechanics.md#scattering-amplitude) of one particle and one [antiparticle](relativistic-quantum-field.md#antiparticle) of a [complex scalar field](#complex-scalar-field), the [Dyson series](perturbative-quantum-field-theory.md#dyson-series) inserts $-i\lambda\phi^{\dagger 2}\phi^2/4$. There are $2!$ assignments of the particle and antiparticle external attachments to each pair of identical field factors, giving $2!2!=4$ and hence the displayed [Feynman vertex](perturbative-quantum-field-theory.md#interaction-vertex). With [relativistic normalization of a one-particle state](quantum-field-theory.md#relativistic-normalization-of-a-one-particle-state), integrating the vertex position gives $i\mathcal T(2\pi)^4\delta^4(p_1+q_1-p_2-q_2)$ with $\mathcal T=-\lambda$. [Vacuum diagrams](perturbative-quantum-field-theory.md#vacuum-feynman-diagram) and one-particle [self-energy](perturbative-quantum-field-theory.md#self-energy) insertions are separate disconnected contributions; [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) eliminates the single-vertex vacuum and tadpole contractions.

### Complex sine-Gordon theory

↑ **Parent:** [Complex scalar field](#complex-scalar-field)

A nonlinear [complex scalar field](#complex-scalar-field) theory with a global phase symmetry and a curved target-space kinetic coefficient. In physical coordinates its classical density is displayed above; dimensionless coordinates measured in $M^{-1}$ put a common $M^2$ outside the reduced density. Its regular coordinate domain is $\lambda^2|\psi|^2<1$. Rotating localized solutions are [charged complex sine-Gordon solitons](#charged-complex-sine-gordon-soliton). The local classical density does not by itself specify the treatment of the singular coordinate boundary or a global quantum completion.

#### Charged complex sine-Gordon soliton

↑ **Parent:** [Complex sine-Gordon theory](#complex-sine-gordon-theory)

The rest-frame field $\psi=\cos\alpha\,e^{i\sin\alpha\,t}/[\lambda\cosh(\cos\alpha\,x)]$ has [mass](classical-mechanics.md#mass) $4M\cos\alpha/\lambda^2$ and charge $4[\operatorname{sgn}(\alpha)\pi/2-\alpha]/\lambda^2$, for the generator $\delta\psi=i\psi$ and $\alpha\ne0$. The conserved phase angle is a [collective coordinate](classical-field-theory-soliton.md#collective-coordinate-of-a-soliton) with momentum $Q$. [Quantization of a periodic soliton coordinate](classical-field-theory-soliton.md#quantization-of-a-periodic-soliton-coordinate) gives integer $Q$ in units $\hbar=1$ and the displayed leading [mass](classical-mechanics.md#mass) formula. On the regular branch $0<|Q|<2\pi/\lambda^2$, its concave increasing sine law prevents fragmentation into smaller like-charge states.

##### Singular charge endpoint of a complex sine-Gordon soliton

↑ **Parent:** [Charged complex sine-Gordon soliton](#charged-complex-sine-gordon-soliton)

At zero rotation the field reaches $\lambda^2|\psi|^2=1$ at its center. Its energy remains finite, but its charge expression is singular and has the two displayed one-sided limits. The regular local branch excludes this endpoint. A global completion must say whether and how these two limiting charge labels represent a physical state.

###### Integer-level charge identification in complex sine-Gordon theory

↑ **Parent:** [Singular charge endpoint of a complex sine-Gordon soliton](#singular-charge-endpoint-of-a-complex-sine-gordon-soliton)

An additional integer-level completion identifies the charge labels modulo $k$ and has $k-1$ nonzero sectors. For even $k$, the two maximal labels describe one self-conjugate sector. This interpretation is specified in [Dorey and Hollowood, section 2](https://arxiv.org/pdf/hep-th/9410140); it is additional to the local classical density.

### Canonical quantization of a complex scalar field

↑ **Parent:** [Complex scalar field](#complex-scalar-field)

A free [complex scalar field](#complex-scalar-field) has independent particle and [antiparticle](relativistic-quantum-field.md#antiparticle) mode operators. With $d\Pi_p=d^3\mathbf p/[(2\pi)^3 2E_p]$, the expansion $\phi=\int d\Pi_p(ae^{-ipx}+b^\dagger e^{ipx})$ and its adjoint reproduce equal-time [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) when $[a(\mathbf p),a^\dagger(\mathbf q)]=[b(\mathbf p),b^\dagger(\mathbf q)]=(2\pi)^3 2E_p\delta^{(3)}(\mathbf p-\mathbf q)$ and cross commutators vanish. The [canonical momenta](classical-mechanics.md#canonical-momentum) are $\pi=\dot\phi^\dagger$, $\pi^\dagger=\dot\phi$. An overall phase on $b$ can reverse the sign of the [antiparticle](relativistic-quantum-field.md#antiparticle) term without changing the theory.

#### Complex scalar mode inversion

↑ **Parent:** [Canonical quantization of a complex scalar field](#canonical-quantization-of-a-complex-scalar-field)

With the invariant measure $d\Pi_p=d^3p/[(2\pi)^3 2E_p]$, a free [complex scalar field](#complex-scalar-field) has particle and [antiparticle](relativistic-quantum-field.md#antiparticle) modes. At any fixed time the displayed inverse and $b^\dagger(p)=\int d^3x\,e^{-ip\cdot x}(E_p\phi-i\dot\phi)$ project onto its positive- and negative-frequency components. The equal-time [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) then give $[a(p),a^\dagger(q)]=[b(p),b^\dagger(q)]=(2\pi)^3 2E_p\delta^3(\mathbf p-\mathbf q)$; cross terms vanish because their [coefficient](vector-space.md#coefficient) contains $E_p-E_q$ on the [momentum](classical-mechanics.md#momentum) delta function.

#### Complex scalar charge operator

↑ **Parent:** [Canonical quantization of a complex scalar field](#canonical-quantization-of-a-complex-scalar-field)

For the global phase transformation $\delta\phi=-i\alpha\phi$, the [Noether current](quantum-field-theory.md#noether-current) is $j^\mu=i(\phi^\dagger\partial^\mu\phi-\partial^\mu\phi^\dagger\,\phi)$. The [Klein-Gordon equation](wave-equation.md#klein-gordon-equation) gives $\partial_\mu j^\mu=0$. With zero vacuum charge, its [normal-ordered](perturbative-quantum-field-theory.md#normal-ordering) charge is $Q=\int d\Pi_p(a^\dagger a-b^\dagger b)$. Thus $[Q,a^\dagger]=a^\dagger$, $[Q,b^\dagger]=-b^\dagger$ and $[Q,\phi]=-\phi$. Particle and [antiparticle](relativistic-quantum-field.md#antiparticle) creation carry opposite charges while both increase energy.

##### Vacuum subtraction of a complex scalar charge

↑ **Parent:** [Complex scalar charge operator](#complex-scalar-charge-operator)

Substituting the free [complex scalar field](#complex-scalar-field) modes into $i\int(\phi^\dagger\dot\phi-\dot\phi^\dagger\phi)d^3x$ gives the formally ordered expression $Q_{\rm bare}=\int d\Pi_p(a^\dagger a-bb^\dagger)$. Its divergent vacuum constant is removed by [normal ordering](perturbative-quantum-field-theory.md#normal-ordering), equivalently by choosing $Q|0\rangle=0$. The resulting [complex scalar charge operator](#complex-scalar-charge-operator) has $[Q,a^\dagger]=a^\dagger$ and $[Q,b^\dagger]=-b^\dagger$. Subtracting the constant changes neither its action on fields nor current conservation, but it is essential when identifying the vacuum charge and the charges of one-particle states.

#### Normal-ordered Hamiltonian of a free complex scalar field

↑ **Parent:** [Canonical quantization of a complex scalar field](#canonical-quantization-of-a-complex-scalar-field)

Spatial integration of the free [Hamiltonian density](quantum-field-theory.md#hamiltonian-density) cancels particle-[antiparticle](relativistic-quantum-field.md#antiparticle) pair terms through $E_p^2-\mathbf p^2-m^2=0$. The raw [Hamiltonian](classical-mechanics.md#hamiltonian) is $\int d\Pi_p E_p(a^\dagger a+bb^\dagger)$. [Normal ordering](perturbative-quantum-field-theory.md#normal-ordering) removes the field-independent [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy) and gives $H=\int d\Pi_p E_p(a^\dagger a+b^\dagger b)$. Both [creation operators](quantum-mechanics.md#creation-operator) increase the energy by $E_p$, so a negative-frequency field mode represents a positive-energy [antiparticle](relativistic-quantum-field.md#antiparticle), not a negative-energy state.

### Global phase symmetry of a complex scalar field

↑ **Parent:** [Complex scalar field](#complex-scalar-field)

For $\mathcal L=\partial_\mu\psi^*\partial^\mu\psi-V(|\psi|^2)$, constant $\alpha$ preserves both terms. This is an [internal symmetry of a classical field theory](quantum-field-theory.md#internal-symmetry-of-a-classical-field-theory) with [circle group](lie-theory.md#circle-group) $U(1)$. A spacetime-dependent phase would introduce derivative terms, so the ordinary-derivative density has only the global symmetry. The associated current is the [Noether charge of a complex scalar field](#noether-charge-of-a-complex-scalar-field) construction; the orientation $e^{-i\alpha}$ fixes its overall sign.

#### Noether charge of a complex scalar field

↑ **Parent:** [Global phase symmetry of a complex scalar field](#global-phase-symmetry-of-a-complex-scalar-field)

For the [global phase symmetry of a complex scalar field](#global-phase-symmetry-of-a-complex-scalar-field) oriented as $\delta\psi=-i\varepsilon\psi$, the [Noether current](quantum-field-theory.md#noether-current) is $j^\mu=i(\psi^*\partial^\mu\psi-\psi\partial^\mu\psi^*)$. The [Euler-Lagrange field equations](quantum-field-theory.md#euler-lagrange-field-equation) $\Box\psi+V'(|\psi|^2)\psi=0$ and its [complex conjugate](complex-analysis.md#complex-conjugate) give $\partial_\mu j^\mu=i(\psi^*\Box\psi-\psi\Box\psi^*)=0$ for a real differentiable potential. Integrating $j^0$ gives $Q$ when boundary flux vanishes. A charged [scalar](vector-space.md#scalar) coupled to electromagnetism has [electric charge](electromagnetism.md#electric-charge) $qQ$ with the chosen charge normalization; without that physical identification it is an internal charge.

## ↑ Ancestors (4)

1. [Quantum field theory](quantum-field-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (6)

- [Asymptotic scalar field](perturbative-quantum-field-theory.md#asymptotic-scalar-field)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-48.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-48.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-49.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-47.md#1/solution)
- [Scalar graph power-counting identity](perturbative-quantum-field-theory.md#scalar-graph-power-counting-identity)
