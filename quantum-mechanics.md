# Quantum mechanics

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_mechanics)

Quantum mechanics models states by wavefunctions and observables by operators.

**Table of contents**

- [Circular infinite quantum well](#circular-infinite-quantum-well)
- [Hegerfeldt theorem](#hegerfeldt-theorem)
- [Rotating-wave approximation](#rotating-wave-approximation)
- [Quantum rotor](#quantum-rotor)
  - [Real-time winding representation of a quantum rotor kernel](#real-time-winding-representation-of-a-quantum-rotor-kernel)
  - [Coupled quantum rotor chain](#coupled-quantum-rotor-chain)
    - [Harmonic phase mode of a quantum rotor chain](#harmonic-phase-mode-of-a-quantum-rotor-chain)
    - [Imaginary-time normalization for a coupled rotor chain](#imaginary-time-normalization-for-a-coupled-rotor-chain)
  - [Rotor winding-sector path integral](#rotor-winding-sector-path-integral)
    - [Momentum-winding duality of the quantum rotor](#momentum-winding-duality-of-the-quantum-rotor)
    - [Rotor return-kernel fluctuation prefactor](#rotor-return-kernel-fluctuation-prefactor)
- [Semiclassical quantization](#semiclassical-quantization)
  - [Bohr-Sommerfeld quantization](#bohr-sommerfeld-quantization)
- [Operator formalism](#operator-formalism)
- [Quasiparticle](#quasiparticle)
  - [Bogoliubov quasiparticle](#bogoliubov-quasiparticle)
  - [Polariton](#polariton)
  - [Exciton](#exciton)
  - [Electron hole](#electron-hole)
- [Sudden approximation](#sudden-approximation)
  - [Ground-state overlap after sudden expansion of a square well](#ground-state-overlap-after-sudden-expansion-of-a-square-well)
- [Canonical quantization](#canonical-quantization)
  - [Weyl ordering](#weyl-ordering)
  - [Canonical quantization of the electromagnetic field](#canonical-quantization-of-the-electromagnetic-field)
    - [Gauge reduction of the Maxwell Hamiltonian](#gauge-reduction-of-the-maxwell-hamiltonian)
    - [Canonical transverse photon field](#canonical-transverse-photon-field)
      - [Transverse equal-time commutator](#transverse-equal-time-commutator)
    - [Primary momentum constraint of the electromagnetic potential](#primary-momentum-constraint-of-the-electromagnetic-potential)
- [Nonrelativistic quantum mechanics](#nonrelativistic-quantum-mechanics)
- [Berry phase](#berry-phase)
- [Classical limit](#classical-limit)
- [Parity](#parity)
  - [Parity conservation](#parity-conservation)
  - [Parity operator](#parity-operator)
  - [Orbital parity](#orbital-parity)
  - [Multiparticle parity](#multiparticle-parity)
    - [Parity selection rule for a two-body decay](#parity-selection-rule-for-a-two-body-decay)
  - [Spatial reflection](#spatial-reflection)
    - [Pseudoscalar](#pseudoscalar)
- [Photon](#photon)
  - [Photon polarization](#photon-polarization)
  - [Photon polarization vector](#photon-polarization-vector)
  - [Two physical polarizations of a photon](#two-physical-polarizations-of-a-photon)
  - [Photon absorption](#photon-absorption)
  - [Photon emission](#photon-emission)
- [Free particle](#free-particle)
- [Ground state](#ground-state)
  - [Ground-state subspace](#ground-state-subspace)
  - [Ground-state degeneracy](#ground-state-degeneracy)
  - [Ground-state energy](#ground-state-energy)
    - [Quantum variational principle](#quantum-variational-principle)
      - [Exponential variational bound for the Yukawa potential](#exponential-variational-bound-for-the-yukawa-potential)
      - [Power-law quantum virial theorem](#power-law-quantum-virial-theorem)
- [Energy eigenvalue](#energy-eigenvalue)
  - [Energy eigenstate](#energy-eigenstate)
  - [Energy eigenspace](#energy-eigenspace)
  - [Excited state](#excited-state)
    - [First excited state](#first-excited-state)
  - [Eigenstate](#eigenstate)
    - [Momentum eigenstate](#momentum-eigenstate)
- [Quantum system](#quantum-system)
  - [Quantum state](#quantum-state)
    - [Dicke state](#dicke-state)
      - [W state](#w-state)
      - [One-qubit reduction of Dicke-state superpositions](#one-qubit-reduction-of-dicke-state-superpositions)
    - [Flavor eigenstate](#flavor-eigenstate)
    - [Quantum superposition](#quantum-superposition)
    - [Qudit](#qudit)
      - [Qudit shift and phase operators](#qudit-shift-and-phase-operators)
    - [Qubit](#qubit)
      - [Qubit state](#qubit-state)
    - [Qutrit](#qutrit)
    - [Quantum number](#quantum-number)
    - [Quantum phase](#quantum-phase)
      - [Global phase](#global-phase)
        - [Global phase of an uncontrolled quantum gate is unobservable](#global-phase-of-an-uncontrolled-quantum-gate-is-unobservable)
    - [Observable](#observable)
      - [Quantum uncertainty](#quantum-uncertainty)
      - [Expectation value](#expectation-value)
      - [Hamiltonian (quantum mechanics)](#hamiltonian-quantum-mechanics)
        - [Quadratic form of a positive quantum Hamiltonian](#quadratic-form-of-a-positive-quantum-hamiltonian)
        - [Morse potential](#morse-potential)
          - [Morse oscillator](#morse-oscillator)
        - [Factorized quantum Hamiltonian](#factorized-quantum-hamiltonian)
          - [Normalizable zero mode of a polynomial factorized Hamiltonian](#normalizable-zero-mode-of-a-polynomial-factorized-hamiltonian)
        - [Quantum symmetry of a Hamiltonian](#quantum-symmetry-of-a-hamiltonian)
          - [Conserved generator of a continuous quantum symmetry](#conserved-generator-of-a-continuous-quantum-symmetry)
        - [Unitary time evolution](#unitary-time-evolution)
          - [Perfect quantum state transfer](#perfect-quantum-state-transfer)
          - [Schrödinger picture](#schrodinger-picture)
          - [Time-evolution operator](#time-evolution-operator)
          - [Quantum-mechanical propagator](#quantum-mechanical-propagator)
            - [Quantum-mechanical propagator in a constant force](#quantum-mechanical-propagator-in-a-constant-force)
            - [Normalized short-time Schrödinger kernel](#normalized-short-time-schrodinger-kernel)
              - [Schrödinger equation from a short-time path integral](#schrodinger-equation-from-a-short-time-path-integral)
            - [Free-particle propagator](#free-particle-propagator)
            - [Semiclassical propagator](#semiclassical-propagator)
              - [Dirichlet fluctuation determinant of a semiclassical propagator](#dirichlet-fluctuation-determinant-of-a-semiclassical-propagator)
              - [Van Vleck determinant](#van-vleck-determinant)
          - [Heisenberg picture](#heisenberg-picture)
            - [Heisenberg equation of motion](#heisenberg-equation-of-motion)
          - [Interaction picture](#interaction-picture)
          - [Time-reversal symmetry in quantum mechanics](#time-reversal-symmetry-in-quantum-mechanics)
            - [Quantum time-reversal operator](#quantum-time-reversal-operator)
            - [Unitary time reversal reverses the energy spectrum](#unitary-time-reversal-reverses-the-energy-spectrum)
            - [Antiunitary time reversal preserves the energy spectrum](#antiunitary-time-reversal-preserves-the-energy-spectrum)
    - [Bound state](#bound-state)
      - [Coulomb bound state](#coulomb-bound-state)
        - [Polynomial construction of hydrogen S states](#polynomial-construction-of-hydrogen-s-states)
    - [Stationary state](#stationary-state)
- [Particle in a ring](#particle-in-a-ring)
- [Planck constant](#planck-constant)
- [Wave function](#wave-function)
  - [Wavefunction normalization](#wavefunction-normalization)
  - [Matter wave](#matter-wave)
    - [Matter-wave interference](#matter-wave-interference)
    - [de Broglie wavelength](#de-broglie-wavelength)
    - [Neutron interferometer](#neutron-interferometer)
      - [Colella–Overhauser–Werner experiment](#colella-overhauser-werner-experiment)
  - [Plane wave](#plane-wave)
  - [Probability amplitude](#probability-amplitude)
    - [Born rule](#born-rule)
      - [Two-level quantum return probability](#two-level-quantum-return-probability)
      - [Two-level observable transition probability](#two-level-observable-transition-probability)
      - [Wigner's theorem](#wigner-s-theorem)
        - [Projective unitary representation](#projective-unitary-representation)
      - [Energy measurement](#energy-measurement)
  - [Normalizable wavefunction](#normalizable-wavefunction)
  - [Probability density](#probability-density)
  - [Probability current](#probability-current)
    - [Probability continuity equation](#probability-continuity-equation)
      - [Conservation of quantum probability](#conservation-of-quantum-probability)
  - [Gaussian wave packet](#gaussian-wave-packet)
    - [Gaussian evolution in an inverted harmonic oscillator](#gaussian-evolution-in-an-inverted-harmonic-oscillator)
- [Potential barrier](#potential-barrier)
  - [Quantum tunnelling](#quantum-tunnelling)
    - [Double-well tunneling splitting](#double-well-tunneling-splitting)
    - [Finite square barrier transmission at half barrier height](#finite-square-barrier-transmission-at-half-barrier-height)
- [Hermitian operator on a nonorthogonal two-state basis](#hermitian-operator-on-a-nonorthogonal-two-state-basis)
  - [Commuting time-dependent two-state Hamiltonian](#commuting-time-dependent-two-state-hamiltonian)
- [Second moments of a complex Gaussian wave packet](#second-moments-of-a-complex-gaussian-wave-packet)
- [Finite square well](#finite-square-well)
  - [Attractive potential ordering does not order quantum reflection](#attractive-potential-ordering-does-not-order-quantum-reflection)
  - [Resonant transmission through a square well](#resonant-transmission-through-a-square-well)
  - [Spherical square well](#spherical-square-well)
    - [Spherically symmetric bound state of a finite well](#spherically-symmetric-bound-state-of-a-finite-well)
  - [Bound-state thresholds for a square well with one hard wall](#bound-state-thresholds-for-a-square-well-with-one-hard-wall)
  - [Hard-core spherical square-well potential](#hard-core-spherical-square-well-potential)
    - [Scattering length of a hard-core spherical square-well potential](#scattering-length-of-a-hard-core-spherical-square-well-potential)
- [Delta potential](#delta-potential)
  - [Central delta barrier in a symmetric infinite well](#central-delta-barrier-in-a-symmetric-infinite-well)
    - [High-energy shift from a central delta barrier](#high-energy-shift-from-a-central-delta-barrier)
  - [Odd bound state and resonance of two delta barriers](#odd-bound-state-and-resonance-of-two-delta-barriers)
  - [Bound state in a delta potential](#bound-state-in-a-delta-potential)
  - [Multiple delta potential](#multiple-delta-potential)
    - [Symmetric double-delta potential](#symmetric-double-delta-potential)
      - [Odd-parity S-matrix of a symmetric double-delta potential](#odd-parity-s-matrix-of-a-symmetric-double-delta-potential)
        - [Odd bound state of a symmetric double-delta potential](#odd-bound-state-of-a-symmetric-double-delta-potential)
        - [Odd resonance of a strongly repulsive symmetric double-delta potential](#odd-resonance-of-a-strongly-repulsive-symmetric-double-delta-potential)
  - [Scattering by a delta potential](#scattering-by-a-delta-potential)
- [Quantum scattering](#quantum-scattering)
  - [Quantum reflection probability](#quantum-reflection-probability)
  - [Transmission amplitude](#transmission-amplitude)
  - [S-matrix](#s-matrix)
    - [Redundant pole of a scattering matrix](#redundant-pole-of-a-scattering-matrix)
    - [Jost function](#jost-function)
    - [Unit-modulus hyperbolic scattering block](#unit-modulus-hyperbolic-scattering-block)
    - [Physical rapidity strip](#physical-rapidity-strip)
      - [Crossed-channel pole in diagonal factorized scattering](#crossed-channel-pole-in-diagonal-factorized-scattering)
      - [Relativistic bound-state mass from a rapidity pole](#relativistic-bound-state-mass-from-a-rapidity-pole)
    - [Hermitian analyticity of a two-particle S-matrix](#hermitian-analyticity-of-a-two-particle-s-matrix)
  - [Scattering wavefunction](#scattering-wavefunction)
  - [Scattering state](#scattering-state)
  - [Partial wave](#partial-wave)
  - [Partial-wave scattering](#partial-wave-scattering)
  - [Differential scattering cross-section](#differential-scattering-cross-section)
    - [Central-potential classical differential cross-section](#central-potential-classical-differential-cross-section)
    - [Quantum differential cross-section from a scattering amplitude](#quantum-differential-cross-section-from-a-scattering-amplitude)
  - [Reflected wave](#reflected-wave)
  - [Transmission probability](#transmission-probability)
  - [One-dimensional S-matrix](#one-dimensional-s-matrix)
    - [Parity basis of a one-dimensional S-matrix](#parity-basis-of-a-one-dimensional-s-matrix)
    - [One-dimensional transfer matrix from scattering amplitudes](#one-dimensional-transfer-matrix-from-scattering-amplitudes)
  - [Partial-wave S-matrix](#partial-wave-s-matrix)
    - [Scattering phase shift](#scattering-phase-shift)
      - [Periodic-box phase-shift quantization](#periodic-box-phase-shift-quantization)
    - [S wave (quantum scattering)](#s-wave-quantum-scattering)
    - [Partial-wave expansion of a scattering amplitude](#partial-wave-expansion-of-a-scattering-amplitude)
      - [Partial-wave total scattering cross-section](#partial-wave-total-scattering-cross-section)
    - [Partial-wave unitarity](#partial-wave-unitarity)
    - [Unitarity and reflection identities for a partial-wave S-matrix](#unitarity-and-reflection-identities-for-a-partial-wave-s-matrix)
    - [Scattering length from a partial-wave S-matrix](#scattering-length-from-a-partial-wave-s-matrix)
      - [Repulsive spherical barrier scattering length](#repulsive-spherical-barrier-scattering-length)
      - [Zero-energy scattering resonance](#zero-energy-scattering-resonance)
    - [Bound-state poles of a partial-wave S-matrix](#bound-state-poles-of-a-partial-wave-s-matrix)
      - [Hyperbolic-tangent S-wave exterior solution](#hyperbolic-tangent-s-wave-exterior-solution)
    - [Scattering resonance](#scattering-resonance)
      - [Resonance pole](#resonance-pole)
  - [Logarithmic-derivative matching](#logarithmic-derivative-matching)
  - [Hard-sphere limit](#hard-sphere-limit)
  - [Lippmann-Schwinger equation](#lippmann-schwinger-equation)
  - [Scattering amplitude](#scattering-amplitude)
    - [Optical theorem](#optical-theorem)
    - [Scattering-amplitude factorization](#scattering-amplitude-factorization)
    - [Crossing symmetry](#crossing-symmetry)
    - [Relativistic scattering cross-section](#relativistic-scattering-cross-section)
      - [Inclusive electron-positron annihilation into hadrons](#inclusive-electron-positron-annihilation-into-hadrons)
        - [Hadronic R ratio](#hadronic-r-ratio)
      - [Elastic scattering from a quartic scalar contact interaction](#elastic-scattering-from-a-quartic-scalar-contact-interaction)
      - [Invariant flux factor](#invariant-flux-factor)
      - [Lorentz-invariant phase-space measure](#lorentz-invariant-phase-space-measure)
        - [Relativistic two-body phase space](#relativistic-two-body-phase-space)
        - [Positive-energy on-shell delta function identity](#positive-energy-on-shell-delta-function-identity)
        - [Two-body decay phase space](#two-body-decay-phase-space)
        - [Identical-particle factor in a final-state phase-space integral](#identical-particle-factor-in-a-final-state-phase-space-integral)
    - [Momentum transfer](#momentum-transfer)
    - [Elastic scattering](#elastic-scattering)
    - [Diffraction](#diffraction)
    - [Crystal scattering](#crystal-scattering)
      - [Bravais lattice](#bravais-lattice)
        - [Unit cell](#unit-cell)
          - [Primitive unit cell](#primitive-unit-cell)
        - [Face-centered tetragonal lattice](#face-centered-tetragonal-lattice)
        - [Face-centered cubic lattice](#face-centered-cubic-lattice)
        - [Lattice point](#lattice-point)
        - [Reciprocal lattice](#reciprocal-lattice)
          - [Wigner-Seitz cell](#wigner-seitz-cell)
            - [Reciprocal lattice and Wigner-Seitz cell of the unit triangular lattice](#reciprocal-lattice-and-wigner-seitz-cell-of-the-unit-triangular-lattice)
        - [Cubic crystal system](#cubic-crystal-system)
          - [Body-centered cubic lattice](#body-centered-cubic-lattice)
            - [Reciprocal lattice of the 2023 Cambridge body-centered cubic basis](#reciprocal-lattice-of-the-2023-cambridge-body-centered-cubic-basis)
      - [Crystal lattice structure factor](#crystal-lattice-structure-factor)
        - [Reciprocal-lattice peaks of a finite crystal](#reciprocal-lattice-peaks-of-a-finite-crystal)
      - [Elastic Bragg scattering condition](#elastic-bragg-scattering-condition)
        - [Bragg's law](#bragg-s-law)
        - [Bragg scattering](#bragg-scattering)
    - [Bound-state pole of the scattering amplitude](#bound-state-pole-of-the-scattering-amplitude)
- [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)
  - [Supersymmetric factorization and zero-mode normalizability](#supersymmetric-factorization-and-zero-mode-normalizability)
  - [Witten index](#witten-index)
  - [Gradient superpotential Hamiltonian in supersymmetric quantum mechanics](#gradient-superpotential-hamiltonian-in-supersymmetric-quantum-mechanics)
    - [Zero mode in the fermion-vacuum sector](#zero-mode-in-the-fermion-vacuum-sector)
  - [Fermion-number sectors in supersymmetric quantum mechanics](#fermion-number-sectors-in-supersymmetric-quantum-mechanics)
    - [Radial superpartner in three-dimensional supersymmetric quantum mechanics](#radial-superpartner-in-three-dimensional-supersymmetric-quantum-mechanics)
  - [Fermionic Fock space](#fermionic-fock-space)
    - [Polarized fermionic Fock space](#polarized-fermionic-fock-space)
      - [Fermion-boson correspondence on the circle](#fermion-boson-correspondence-on-the-circle)
      - [Heisenberg current algebra of a fermion on the circle](#heisenberg-current-algebra-of-a-fermion-on-the-circle)
        - [Fermionic current on the circle](#fermionic-current-on-the-circle)
      - [Segal quantization criterion for fermions](#segal-quantization-criterion-for-fermions)
    - [Fermionic operator](#fermionic-operator)
    - [Clifford vacuum](#clifford-vacuum)
    - [Canonical anticommutation relations](#canonical-anticommutation-relations)
      - [Fermionic bilinear charge algebra](#fermionic-bilinear-charge-algebra)
        - [Triplet charged-current closure on electromagnetic charge](#triplet-charged-current-closure-on-electromagnetic-charge)
      - [Equal-time canonical anticommutator of a Dirac field](#equal-time-canonical-anticommutator-of-a-dirac-field)
    - [Fermion number operator](#fermion-number-operator)
      - [Supertrace](#supertrace)
        - [Equivariant supertrace](#equivariant-supertrace)
  - [Fermionic path integral](#fermionic-path-integral)
    - [Berezin integral](#berezin-integral)
      - [Grassmann change-of-variables formula](#grassmann-change-of-variables-formula)
    - [Short-time limit of a supersymmetric path integral](#short-time-limit-of-a-supersymmetric-path-integral)
  - [Twisted de Rham differential](#twisted-de-rham-differential)
  - [Partner Hamiltonians](#partner-hamiltonians)
  - [Pöschl-Teller potential](#poschl-teller-potential)
    - [Supersymmetric factorization of the one-soliton potential](#supersymmetric-factorization-of-the-one-soliton-potential)
- [Reflectionless potential](#reflectionless-potential)
- [Position operator](#position-operator)
  - [Position eigenstate](#position-eigenstate)
- [Momentum operator](#momentum-operator)
  - [Spatial translation operator](#spatial-translation-operator)
  - [Position representation of the momentum operator](#position-representation-of-the-momentum-operator)
  - [Canonical commutation relation](#canonical-commutation-relation)
    - [Weyl relations](#weyl-relations)
      - [Stone-von Neumann theorem](#stone-von-neumann-theorem)
      - [Gaussian projection in a Weyl representation](#gaussian-projection-in-a-weyl-representation)
- [Ehrenfest theorem](#ehrenfest-theorem)
  - [Proof of Ehrenfest theorem from the Schrodinger equation](#proof-of-ehrenfest-theorem-from-the-schrodinger-equation)
  - [Classical equations from Ehrenfest theorem](#classical-equations-from-ehrenfest-theorem)
  - [Correspondence principle](#correspondence-principle)
- [Angular momentum operator](#angular-momentum-operator)
  - [Axially symmetric quadratic orbital eigenfunction](#axially-symmetric-quadratic-orbital-eigenfunction)
  - [Angular momentum lowering operator](#angular-momentum-lowering-operator)
    - [Normalized highest-weight lowering formula](#normalized-highest-weight-lowering-formula)
  - [Angular momentum eigenstate](#angular-momentum-eigenstate)
  - [Angular momentum commutation relations](#angular-momentum-commutation-relations)
  - [Addition of angular momentum](#addition-of-angular-momentum)
    - [Total angular momentum operator](#total-angular-momentum-operator)
    - [Total-spin sector](#total-spin-sector)
      - [Three spin-one angular-momentum decomposition](#three-spin-one-angular-momentum-decomposition)
        - [Symmetric three-spin-one subspace](#symmetric-three-spin-one-subspace)
      - [Spin-one Cartesian basis](#spin-one-cartesian-basis)
      - [Spin-dot-product eigenvalue](#spin-dot-product-eigenvalue)
    - [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition)
      - [Lowest-weight coupling of two angular momenta](#lowest-weight-coupling-of-two-angular-momenta)
    - [Highest-weight states in angular momentum addition](#highest-weight-states-in-angular-momentum-addition)
    - [Singlet state](#singlet-state)
      - [Spin-one-half singlet state](#spin-one-half-singlet-state)
    - [Spin-one-half triplet state](#spin-one-half-triplet-state)
  - [Spin](#spin)
    - [Jordan–Wigner transformation](#jordan-wigner-transformation)
    - [Spin one-half](#spin-one-half)
      - [Spin one-half along an axis](#spin-one-half-along-an-axis)
    - [Holstein–Primakoff transformation](#holstein-primakoff-transformation)
      - [Holstein–Primakoff occupation constraint](#holstein-primakoff-occupation-constraint)
    - [Spin commutation relations](#spin-commutation-relations)
    - [Irreducible spin representation](#irreducible-spin-representation)
      - [Wigner D-matrix](#wigner-d-matrix)
      - [Unitary highest-weight termination](#unitary-highest-weight-termination)
      - [Spin-one half-turn matrix](#spin-one-half-turn-matrix)
    - [Spin ladder operator](#spin-ladder-operator)
      - [Spin raising operator](#spin-raising-operator)
      - [Spin lowering operator](#spin-lowering-operator)
    - [Spin-three-halves matrices](#spin-three-halves-matrices)
    - [Spin coherent state](#spin-coherent-state)
      - [Spin coherent-state path integral](#spin-coherent-state-path-integral)
      - [Equatorial spin-three-halves coherent state](#equatorial-spin-three-halves-coherent-state)
    - [Larmor precession](#larmor-precession)
      - [Larmor precession of a spin coherent state](#larmor-precession-of-a-spin-coherent-state)
        - [Time evolution under a spin-Z Hamiltonian](#time-evolution-under-a-spin-z-hamiltonian)
    - [Heisenberg model](#heisenberg-model)
      - [Magnetization sectors of a spin chain](#magnetization-sectors-of-a-spin-chain)
      - [Excitation-number conservation in XXZ spin chains](#excitation-number-conservation-in-xxz-spin-chains)
      - [Single-excitation subspace](#single-excitation-subspace)
        - [XY exchange interaction](#xy-exchange-interaction)
          - [Symmetric-arm reduction of an exchange Hamiltonian](#symmetric-arm-reduction-of-an-exchange-hamiltonian)
        - [Endpoint control of an XX spin chain](#endpoint-control-of-an-xx-spin-chain)
      - [Heisenberg antiferromagnet](#heisenberg-antiferromagnet)
        - [Bipartite spin rotation](#bipartite-spin-rotation)
      - [Heisenberg ferromagnet](#heisenberg-ferromagnet)
        - [Ferromagnetic ground-state multiplet](#ferromagnetic-ground-state-multiplet)
      - [Two-spin Heisenberg Hamiltonian in an opposing longitudinal field](#two-spin-heisenberg-hamiltonian-in-an-opposing-longitudinal-field)
      - [All-to-all Heisenberg model](#all-to-all-heisenberg-model)
      - [Infinite-coordination Heisenberg antiferromagnet](#infinite-coordination-heisenberg-antiferromagnet)
- [Infinite square well](#infinite-square-well)
  - [Energy form of a half-well sine state](#energy-form-of-a-half-well-sine-state)
  - [Ramp-state expansion in a symmetric infinite well](#ramp-state-expansion-in-a-symmetric-infinite-well)
  - [Particle in a rectangular box](#particle-in-a-rectangular-box)
- [Degenerate energy levels](#degenerate-energy-levels)
- [Orbital angular momentum](#orbital-angular-momentum)
  - [Highest-weight complex-coordinate orbital wavefunction](#highest-weight-complex-coordinate-orbital-wavefunction)
  - [Angular momentum of a homogeneous harmonic polynomial](#angular-momentum-of-a-homogeneous-harmonic-polynomial)
  - [Angular momentum of a radial function times a linear polynomial](#angular-momentum-of-a-radial-function-times-a-linear-polynomial)
  - [Magnetic quantum number](#magnetic-quantum-number)
  - [Rotation commutators for orbital angular momentum](#rotation-commutators-for-orbital-angular-momentum)
  - [Orbital angular momentum commutation relations](#orbital-angular-momentum-commutation-relations)
  - [Angular momentum ladder operator](#angular-momentum-ladder-operator)
  - [Squared orbital angular momentum in position and momentum operators](#squared-orbital-angular-momentum-in-position-and-momentum-operators)
    - [Spherical Laplacian from orbital angular momentum](#spherical-laplacian-from-orbital-angular-momentum)
  - [Angular momentum ladder variable](#angular-momentum-ladder-variable)
    - [Angular momentum of a complex-coordinate Gaussian state](#angular-momentum-of-a-complex-coordinate-gaussian-state)
  - [Rotational invariance of a central-potential Hamiltonian](#rotational-invariance-of-a-central-potential-hamiltonian)
    - [Separation of a two-dimensional central-potential eigenstate](#separation-of-a-two-dimensional-central-potential-eigenstate)
- [Quantum harmonic oscillator](#quantum-harmonic-oscillator)
  - [Stability of monomial ladder-operator perturbations](#stability-of-monomial-ladder-operator-perturbations)
  - [Harmonic oscillator transition kernel](#harmonic-oscillator-transition-kernel)
  - [Minimum-energy normalized oscillator mode](#minimum-energy-normalized-oscillator-mode)
  - [One-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain)
    - [Graph estimate for the harmonic oscillator](#graph-estimate-for-the-harmonic-oscillator)
      - [Resolvent of the shifted harmonic oscillator](#resolvent-of-the-shifted-harmonic-oscillator)
  - [Thermal partition function of a quantum harmonic oscillator](#thermal-partition-function-of-a-quantum-harmonic-oscillator)
  - [Displaced quantum harmonic oscillator](#displaced-quantum-harmonic-oscillator)
    - [Ground-state overlap after sudden oscillator displacement](#ground-state-overlap-after-sudden-oscillator-displacement)
  - [Zero-point energy](#zero-point-energy)
  - [Squeezed coherent state](#squeezed-coherent-state)
  - [Creation and annihilation operators](#creation-and-annihilation-operators)
    - [Annihilation operator](#annihilation-operator)
    - [Creation operator](#creation-operator)
    - [Bosonic creation operator](#bosonic-creation-operator)
    - [Bosonic annihilation operator](#bosonic-annihilation-operator)
    - [Single-mode squeeze operator](#single-mode-squeeze-operator)
      - [Squeezed vacuum state](#squeezed-vacuum-state)
        - [Multimode squeezed vacuum](#multimode-squeezed-vacuum)
    - [Number operator](#number-operator)
      - [Number state](#number-state)
      - [Integer spectrum of the number operator](#integer-spectrum-of-the-number-operator)
  - [Two commensurate quantum harmonic oscillators](#two-commensurate-quantum-harmonic-oscillators)
- [Three-dimensional isotropic harmonic oscillator](#three-dimensional-isotropic-harmonic-oscillator)
  - [Cartesian number state of the three-dimensional isotropic harmonic oscillator](#cartesian-number-state-of-the-three-dimensional-isotropic-harmonic-oscillator)
  - [Orbital angular momentum in oscillator ladder operators](#orbital-angular-momentum-in-oscillator-ladder-operators)
- [Two-dimensional isotropic harmonic oscillator](#two-dimensional-isotropic-harmonic-oscillator)
  - [Shifted two-dimensional oscillator in a uniform electric field](#shifted-two-dimensional-oscillator-in-a-uniform-electric-field)
  - [Oscillator bilinear commutator](#oscillator-bilinear-commutator)
  - [Schwinger boson representation](#schwinger-boson-representation)
- [Fermi oscillator](#fermi-oscillator)
  - [Projection Hamiltonian](#projection-hamiltonian)
  - [Fermionic raising and lowering operator](#fermionic-raising-and-lowering-operator)
- [Tensor product of quantum systems](#tensor-product-of-quantum-systems)
  - [Jaynes-Cummings model](#jaynes-cummings-model)
  - [Multiparticle quantum state](#multiparticle-quantum-state)
    - [Particle exchange operator](#particle-exchange-operator)
      - [Indistinguishable particles](#indistinguishable-particles)
        - [Boson](#boson)
          - [Bosonic exchange symmetry](#bosonic-exchange-symmetry)
            - [Bosonic statistics from commuting creation operators](#bosonic-statistics-from-commuting-creation-operators)
        - [Fermion](#fermion)
          - [Fermi-Dirac statistics](#fermi-dirac-statistics)
          - [Exchange symmetry of two identical spin-one-half fermions](#exchange-symmetry-of-two-identical-spin-one-half-fermions)
          - [Pauli exclusion principle](#pauli-exclusion-principle)
        - [Spin-statistics theorem](#spin-statistics-theorem)
        - [Two identical spin-one bosons](#two-identical-spin-one-bosons)
          - [Degeneracy of two identical spin-one bosons with equally spaced orbital levels](#degeneracy-of-two-identical-spin-one-bosons-with-equally-spaced-orbital-levels)
  - [Decoupled Fermi oscillators](#decoupled-fermi-oscillators)
  - [Kronecker product representation of local operators](#kronecker-product-representation-of-local-operators)
  - [Decoupled commuting Hamiltonian terms](#decoupled-commuting-hamiltonian-terms)
- [Time-dependent perturbation theory](#time-dependent-perturbation-theory)
  - [Electric-dipole interaction](#electric-dipole-interaction)
    - [Electric-dipole selection rule](#electric-dipole-selection-rule)
  - [Continuum transition probability at long times](#continuum-transition-probability-at-long-times)
- [Time-independent perturbation theory](#time-independent-perturbation-theory)
  - [Hellmann–Feynman theorem](#hellmann-feynman-theorem)
  - [First-order energy correction](#first-order-energy-correction)
  - [Nondegenerate energy eigenvalue](#nondegenerate-energy-eigenvalue)
  - [First-order nondegenerate perturbation theory](#first-order-nondegenerate-perturbation-theory)
    - [First-order ground state of the quartic oscillator](#first-order-ground-state-of-the-quartic-oscillator)
  - [Second-order nondegenerate perturbation theory](#second-order-nondegenerate-perturbation-theory)
  - [Imaginary-coupled two-level Hamiltonian](#imaginary-coupled-two-level-hamiltonian)
  - [Bright and dark state reduction of a star-coupled Hamiltonian](#bright-and-dark-state-reduction-of-a-star-coupled-hamiltonian)
- [Degenerate perturbation theory](#degenerate-perturbation-theory)
  - [Perturbation diagonal within a degenerate eigenspace](#perturbation-diagonal-within-a-degenerate-eigenspace)
  - [Exact diagonalization within a degenerate subspace](#exact-diagonalization-within-a-degenerate-subspace)
    - [Resonant two-to-one oscillator coupling](#resonant-two-to-one-oscillator-coupling)
- [Pauli X eigenstate](#pauli-x-eigenstate)
- [Rectangular potential barrier](#rectangular-potential-barrier)
- [Perturbation theory (quantum mechanics)](#perturbation-theory-quantum-mechanics)
- [Hartree equations](#hartree-equations)

## Circular infinite quantum well

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

A particle confined by a [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) to a disc of radius $a$ has angular functions $e^{im\phi}$, $m\in\mathbb Z$, and regular radial [Bessel functions of the first kind](analysis.md#bessel-function-of-the-first-kind) $J_{|m|}(kr)$. Their boundary zeros give the displayed energies. The ground state belongs to $m=0$: nonzero angular modes add a nonnegative centrifugal term to the kinetic-energy form. At the origin exclude the singular radial solution, rather than accepting every square-integrable logarithmic function as a physical eigenstate.

## Hegerfeldt theorem

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Let $H$ be a self-adjoint Hamiltonian bounded below, $A$ a bounded positive operator and $p_A(t)=\langle e^{-iHt}\psi,Ae^{-iHt}\psi\rangle$. The [Hegerfeldt theorem](#hegerfeldt-theorem) states that either $p_A(t)$ vanishes identically or it is nonzero for almost every real time. In particular, vanishing throughout an open interval forces identically vanishing. The proof uses analytic continuation of $A^{1/2}e^{-iHt}\psi$ into the lower half-plane. Applied to an assumed sharp localization effect, this obstructs strict finite-speed localization for positive-energy one-particle dynamics. It does not identify a controllable superluminal signal: the localization observables and admissible local preparation procedures need separate analysis.

## Rotating-wave approximation

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotating-wave_approximation)

After expressing a driven [Quantum Hamiltonian](#hamiltonian-quantum-mechanics) in a suitable interaction or rotating frame, discard terms oscillating rapidly compared with the retained dynamics. Near a selected transition, this leaves resonant terms that accumulate coherently while counter-rotating terms average out to leading order. The drive strength and detuning must be small relative to the discarded oscillation frequencies over the intended regime; strong driving can require the neglected frequency shifts and corrections. The approximation supports [resonant quantum control](control-theory.md#resonant-quantum-control), but it is not exact merely because the carrier is tuned to resonance.

## Quantum rotor

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

A quantum coordinate on a circle with kinetic Hamiltonian $\ell^2/(2I)$. Periodic wavefunctions have angular momentum $\hbar n$ and energy $\hbar^2n^2/(2I)$ for integer $n$. Its thermal trace has both a momentum-eigenstate sum and a topological winding-path representation. Twisted boundary conditions or flux would modify this spectrum and are separate models.

### Real-time winding representation of a quantum rotor kernel

↑ **Parent:** [Quantum rotor](#quantum-rotor)

The [quantum rotor](#quantum-rotor) with angle period $2\pi$ has both the spectral kernel $(2\pi)^{-1}\sum_n e^{in\Delta-i\hbar n^2T/(2I)}$ and the displayed winding representation. The [Poisson summation formula](fourier-analysis.md#poisson-summation-formula) converts one into the other by a [Gaussian integral](calculus.md#gaussian-integral). Each winding sector has a constant-velocity classical path and action $I(\Delta+2\pi m)^2/(2T)$. Quadratic fluctuations give the same prefactor in every sector, so this is exact. Real time is understood by $T\to T-i0$, which fixes the square-root branch and convergence prescription.

### Coupled quantum rotor chain

↑ **Parent:** [Quantum rotor](#quantum-rotor)

A chain with local rotor inertia and a phase-locking interaction $-J\cos(\phi_{n+1}-\phi_n)$. Its smooth-phase limit is an elastic phase field with inertia $I$ and stiffness $J$. Compact winding and phase-slip processes remain part of the full model even when absent from the Gaussian smooth-sector approximation.

#### Harmonic phase mode of a quantum rotor chain

↑ **Parent:** [Coupled quantum rotor chain](#coupled-quantum-rotor-chain)

Expanding the cosine gives a wave equation $I\phi_{tt}=J\phi_{xx}$ and a gapless phase mode with physical frequency $\sqrt{J/I}|q|$. The exact harmonic lattice frequency is $2\sqrt{J/I}|\sin(q/2)|$. It resembles [superfluid](statistical-physics.md#superfluid) sound. In one dimension, Gaussian phase fluctuations and possible compact [phase slips](dynamical-systems.md#phase-slip) require care before inferring true long-range order from this branch.

#### Imaginary-time normalization for a coupled rotor chain

↑ **Parent:** [Coupled quantum rotor chain](#coupled-quantum-rotor-chain)

When imaginary time is divided by $\hbar$ and ranges from zero to $\beta$, integrating rotor momenta gives $I\dot\phi^2/(2\hbar^2)$ but leaves the potential stiffness term $J(\partial_x\phi)^2/2$. Factoring $1/\hbar^2$ out of both terms requires spatial coefficient $\hbar^2J$ inside the bracket. Setting $\hbar=1$ hides this distinction, but restoring units must preserve it.

### Rotor winding-sector path integral

↑ **Parent:** [Quantum rotor](#quantum-rotor)

The thermal rotor [path integral](quantum-field-theory.md#path-integral) traces paths closed modulo $2\pi$. Lift them to the line and sum endpoints differing by $2\pi m$. In inverse-energy time $0<\tau<\beta$, the kinetic exponent is $I\int\dot\phi^2d\tau/(2\hbar^2)$. Integer $m$ counts trajectory windings, not angular-momentum eigenstates.

#### Momentum-winding duality of the quantum rotor

↑ **Parent:** [Rotor winding-sector path integral](#rotor-winding-sector-path-integral)

[Poisson resummation](fourier-analysis.md#poisson-summation-formula) relates the momentum sum $\sum_ne^{-\beta\hbar^2n^2/(2I)}$ to the winding sum $\sqrt{2\pi I/(\beta\hbar^2)}\sum_me^{-2\pi^2Im^2/(\beta\hbar^2)}$. Gaussian Fourier transformation proves equality, including the prefactor. The momentum form converges rapidly at low temperature and the winding form at high temperature.

#### Rotor return-kernel fluctuation prefactor

↑ **Parent:** [Rotor winding-sector path integral](#rotor-winding-sector-path-integral)

Writing $\phi=\phi_0+2\pi m\tau/\beta+\eta$ with endpoint-fixed $\eta$ separates winding action and Gaussian fluctuations. The latter give the free return kernel on the lifted line, $Z_0=\sqrt{I/(2\pi\hbar^2\beta)}$. The starting-angle integral supplies $2\pi$. Zero winding is not the same as the zero-momentum ground-state sector.

## Semiclassical quantization

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

[Semiclassical quantization](#semiclassical-quantization) uses classical trajectories and actions to approximate quantum states in a regime where relevant actions are large compared with $\hbar$. Phase consistency on a periodic orbit leads to [Bohr-Sommerfeld quantization](#bohr-sommerfeld-quantization). Soliton [collective coordinates](classical-field-theory-soliton.md#collective-coordinate-of-a-soliton) can be quantized this way, while fluctuations supply additional corrections to the leading classical [mass](classical-mechanics.md#mass).

### Bohr-Sommerfeld quantization

↑ **Parent:** [Semiclassical quantization](#semiclassical-quantization)

Single-valued semiclassical phase on a closed classical orbit quantizes its action, with [Maslov index](symplectic-geometry.md#maslov-index) $\mu$ accounting for turning-point phase corrections. A cyclic angle has no oscillator turning points: its wavefunctions are $e^{i\ell q}$, with signed $\ell\in\mathbb Z$ for a $2\pi$ period and [canonical momentum](classical-mechanics.md#canonical-momentum) $\hbar\ell$. There is no half-integer shift for that free angular coordinate.

## Operator formalism

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

The [operator formalism](#operator-formalism) describes a quantum system using states in a [Hilbert space](hilbert-space.md) and observables represented by [self-adjoint operators](linear-operator-theory.md#self-adjoint-operator) with suitable domains on that [Hilbert space](hilbert-space.md). Evolution and correlation functions are computed from [Hamiltonian operators](#hamiltonian-quantum-mechanics) and their [time-ordered products](perturbative-quantum-field-theory.md#time-ordered-product). For free [quantized fields](quantum-field-theory.md#quantized-field), the oscillator construction gives a [Fock space](quantum-field-theory.md#fock-space). The [operator-path-integral equivalence](quantum-field-theory.md#operator-path-integral-equivalence) relates these matrix elements to integrals over field histories.

## Quasiparticle

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasiparticle)

A quasiparticle is a collective excitation that can be described approximately by particle-like quantum numbers and dynamics, even though it is not an isolated elementary particle. [Excitons](#exciton) and [polaritons](#polariton) are examples.

### Bogoliubov quasiparticle

↑ **Parent:** [Quasiparticle](#quasiparticle)

A Bogoliubov [quasiparticle](#quasiparticle) is an excitation created by the diagonal mode operator obtained through a [Bogoliubov transformation](quantum-field-theory.md#bogoliubov-transformation). Its vacuum can contain particles in the original modes because creation and [annihilation operators](#annihilation-operator) mix. Examples include [antiferromagnetic spin waves](statistical-physics.md#antiferromagnetic-spin-wave), Bose-gas [phonons](statistical-physics.md#phonon) and paired-fermion excitations.

### Polariton

↑ **Parent:** [Quasiparticle](#quasiparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polariton)

A [polariton](#polariton) is a hybrid light–matter excitation formed by strong coupling between a [photon](#photon) and a material excitation. For an exciton-polariton, the material component is an [exciton](#exciton).

### Exciton

↑ **Parent:** [Quasiparticle](#quasiparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exciton)

An [exciton](#exciton) is a [bound state](#bound-state) of an electron and an [electron hole](#electron-hole). Coupling this material excitation strongly to a [photon](#photon) can form a [polariton](#polariton).

### Electron hole

↑ **Parent:** [Quasiparticle](#quasiparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electron_hole)

An electron hole is the absence of an electron in an otherwise filled band, described as a mobile positive-charge excitation. It can form a [bound state](#bound-state) with an electron, giving an [exciton](#exciton).

## Sudden approximation

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

When a [Hamiltonian operator](#hamiltonian-quantum-mechanics) changes instantaneously by a finite potential step, the [quantum state](#quantum-state) is continuous across the switching time. Its coefficients in the new energy eigenbasis are its overlaps with those eigenstates; the [Born rule](#born-rule) gives their squared moduli as probabilities. The state need not remain an energy eigenstate of the new Hamiltonian.

### Ground-state overlap after sudden expansion of a square well

↑ **Parent:** [Sudden approximation](#sudden-approximation)

For an [infinite square well](#infinite-square-well) initially on $[-a,a]$, a normalized [ground state](#ground-state) is $a^{-1/2}\cos(\pi x/(2a))$. If the endpoints change instantaneously to $\pm\eta a$, with $\eta>1$, the [sudden approximation](#sudden-approximation) leaves the [wave function](#wave-function) unchanged, extended by zero outside the old well. Its overlap with the new normalized [ground state](#ground-state) $(\eta a)^{-1/2}\cos(\pi x/(2\eta a))$ is $4\eta^{3/2}\cos(\pi/(2\eta))/[\pi(\eta^2-1)]$. The [Born rule](#born-rule) squares this [probability amplitude](#probability-amplitude); for $\eta=2$ the result is $64/(9\pi^2)$, and the limit as $\eta\downarrow1$ is $1$.

## Canonical quantization

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_quantization)

Canonical quantization promotes [canonical variables](classical-mechanics.md#canonical-variables) to operators and their [Poisson brackets](classical-mechanics.md#poisson-bracket) to [canonical commutation relations](#canonical-commutation-relation). Composite observables require an ordering prescription, and [quantum anomalies](relativistic-quantum-field.md#anomaly-physics) can modify their algebra.

### Weyl ordering

↑ **Parent:** [Canonical quantization](#canonical-quantization)

Weyl ordering symmetrizes position and momentum factors in a classical polynomial before promoting them to an operator. Its phase-space symbol corresponds to midpoint [time slicing of a phase-space path integral](quantum-field-theory.md#time-slicing-of-a-phase-space-path-integral). In particular, the Weyl symbol of $a^\dagger a$ is $\bar\psi\psi-1/2$, whereas its [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) symbol is $\bar\psi\psi$.

### Canonical quantization of the electromagnetic field

↑ **Parent:** [Canonical quantization](#canonical-quantization)

The [electromagnetic four-potential](electromagnetism.md#electromagnetic-four-potential) has a vanishing temporal momentum and a [Gauss law constraint in gauge theory](relativistic-quantum-field.md#gauss-law-constraint-in-gauge-theory). Gauge reduction leaves two transverse [canonical pairs](classical-mechanics.md#canonical-pair). Their [canonical commutation relations](#canonical-commutation-relation) give the [photon](#photon) creation and [annihilation operators](#annihilation-operator). Covariant [Gupta-Bleuler quantization](relativistic-quantum-field.md#gupta-bleuler-formalism) instead retains auxiliary polarization modes and selects the same physical state space by a subsidiary condition and null-state quotient.

#### Gauge reduction of the Maxwell Hamiltonian

↑ **Parent:** [Canonical quantization of the electromagnetic field](#canonical-quantization-of-the-electromagnetic-field)

For a spatial potential $\mathbf A$ with $\mathbf E=-\dot{\mathbf A}-\boldsymbol\nabla A_0$, the [Maxwell Lagrangian](electromagnetism.md#maxwell-lagrangian) gives $\boldsymbol\Pi=-\mathbf E$ and $\Pi^0=0$. Its [Hamiltonian](classical-mechanics.md#hamiltonian) is $\int[(\boldsymbol\Pi^2+\mathbf B^2)/2+A_0\boldsymbol\nabla\cdot\boldsymbol\Pi],d^3x$. Preserving the temporal momentum [first-class constraint](classical-mechanics.md#first-class-constraint) gives the [Gauss law constraint in gauge theory](relativistic-quantum-field.md#gauss-law-constraint-in-gauge-theory). In free space, [Coulomb gauge](electromagnetism.md#coulomb-gauge) and decay at spatial infinity set $A_0=0$ and leave only transverse modes. The reduced [Dirac bracket](classical-mechanics.md#dirac-bracket) uses the projector $\delta_{ij}-k_i k_j/|\mathbf k|^2$, so quantization gives the [transverse equal-time commutator](#transverse-equal-time-commutator) and the positive Hamiltonian displayed above.

#### Canonical transverse photon field

↑ **Parent:** [Canonical quantization of the electromagnetic field](#canonical-quantization-of-the-electromagnetic-field)

The free transverse [photon](#photon) field is a Hermitian sum of two transverse-polarization plane-wave modes with creation and [annihilation operators](#annihilation-operator). Their standard bosonic [commutator](lie-algebra.md#commutator) gives the [transverse equal-time commutator](#transverse-equal-time-commutator). The normal-ordered [Hamiltonian](classical-mechanics.md#hamiltonian) is a sum of positive oscillator energies.

##### Transverse equal-time commutator

↑ **Parent:** [Canonical transverse photon field](#canonical-transverse-photon-field)

The reduced [canonical commutation relation](#canonical-commutation-relation) for a transverse field uses a transverse delta function instead of an unconstrained componentwise delta. Its Fourier transform is the spatial transverse projector. It can be derived from the two-polarization oscillator expansion or from the [Dirac bracket](classical-mechanics.md#dirac-bracket) after [gauge fixing](relativistic-quantum-field.md#gauge-fixing).

#### Primary momentum constraint of the electromagnetic potential

↑ **Parent:** [Canonical quantization of the electromagnetic field](#canonical-quantization-of-the-electromagnetic-field)

The Maxwell [Lagrangian density](quantum-field-theory.md#lagrangian-density) contains no time derivative of $A_0$, so its [canonical momentum](classical-mechanics.md#canonical-momentum) vanishes. The condition is a [first-class constraint](classical-mechanics.md#first-class-constraint). Its time preservation yields the [Gauss law constraint in gauge theory](relativistic-quantum-field.md#gauss-law-constraint-in-gauge-theory); $A_0$ acts as the corresponding multiplier in the [Hamiltonian](classical-mechanics.md#hamiltonian).

## Nonrelativistic quantum mechanics

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Nonrelativistic quantum mechanics describes systems at speeds small compared with the speed of light, usually with time as an external parameter and evolution governed by the [Schrödinger equation](physics.md#schrodinger-equation).

## Berry phase

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Berry_phase)

A Berry phase is the geometric phase acquired by a quantum state transported around a closed path in parameter space.

## Classical limit

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classical_limit)

The classical limit is a regime in which quantum corrections or occupation-number discreteness become negligible and classical equations describe the relevant observables.

## Parity

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parity_(physics))

Parity is the eigenvalue $+1$ or $-1$ of a state under [spatial reflection](#spatial-reflection).

### Parity conservation

↑ **Parent:** [Parity](#parity)

An interaction commuting with the [parity operator](#parity-operator) preserves total parity. A two-body final state has the product of its particles' intrinsic parities times the orbital factor $(-1)^\ell$, giving the [parity selection rule for a two-body decay](#parity-selection-rule-for-a-two-body-decay).

### Parity operator

↑ **Parent:** [Parity](#parity)

The parity operator acts on a spatial [wavefunction](#wave-function) by $(P\psi)(x)=\psi(-x)$ and satisfies $P^2=I$. For a [Hamiltonian operator](#hamiltonian-quantum-mechanics) with an even potential and parity-invariant domain, $HP=PH$. A [nondegenerate energy eigenvalue](#nondegenerate-energy-eigenvalue) has a one-dimensional [eigenspace](linear-operator-theory.md#eigenspace), so its eigenfunction is an eigenvector of $P$ with eigenvalue $+1$ or $-1$.

### Orbital parity

↑ **Parent:** [Parity](#parity)

An [orbital angular momentum](#orbital-angular-momentum) eigenstate with quantum number $\ell$ changes by the factor $(-1)^\ell$ under [spatial reflection](#spatial-reflection). Equivalently,

$$
Y_\ell^m(-\widehat{\mathbf r})=(-1)^\ell Y_\ell^m(\widehat{\mathbf r}).
$$

### Multiparticle parity

↑ **Parent:** [Parity](#parity)

The parity of a two-particle centre-of-mass state with intrinsic parities $\eta_1,\eta_2$ and relative [orbital angular momentum](#orbital-angular-momentum) $\ell$ is

$$
\eta_1\eta_2(-1)^\ell.
$$

#### Parity selection rule for a two-body decay

↑ **Parent:** [Multiparticle parity](#multiparticle-parity)

If parity is conserved when a particle of intrinsic parity $\eta_i$ decays into two particles of intrinsic parities $\eta_1,\eta_2$, then their relative partial wave obeys

$$
\eta_i=\eta_1\eta_2(-1)^\ell.
$$

### Spatial reflection

↑ **Parent:** [Parity](#parity)

Spatial reflection reverses every spatial coordinate.

#### Pseudoscalar

↑ **Parent:** [Spatial reflection](#spatial-reflection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudoscalar)

A pseudoscalar is invariant under proper rotations but changes sign under a [spatial reflection](#spatial-reflection). In three dimensions the [scalar triple product](linear-algebra.md#scalar-triple-product) is a pseudoscalar.

## Photon

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Photon)

A photon is a quantum of the electromagnetic field with energy $E=h\nu=\hbar\omega$.

### Photon polarization

↑ **Parent:** [Photon](#photon)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Photon_polarization)

For a [photon](#photon) in a fixed spatial mode, the two transverse [photon polarizations](#photon-polarization) span a [qubit](#qubit) space. A pure [photon polarization](#photon-polarization) state is $\alpha|H\rangle+\beta|V\rangle$ with $|\alpha|^2+|\beta|^2=1$, and a general state is a two-dimensional [density matrix](quantum-theory.md#density-matrix). Its [Bloch vector](quantum-theory.md#bloch-vector) gives the normalized Stokes parameters. Polarization-dependent path separation can correlate this internal degree of freedom with a path [qubit](#qubit).

// Target: quantum-error-correction.bigb

### Photon polarization vector

↑ **Parent:** [Photon](#photon)

For a real [on shell](quantum-field-theory.md#on-shell) [photon](#photon) of null momentum $k$, a physical polarization satisfies $k\cdot\epsilon=0$ and is defined modulo $\epsilon\mapsto\epsilon+\alpha k$. The two-dimensional quotient carries the two physical [photon](#photon) helicities. In a transverse gauge choose $\epsilon^0=0$ and $\epsilon^*\cdot\epsilon=-1$. A [Ward identity](perturbative-quantum-field-theory.md#ward-identity) ensures that replacing an external polarization by its momentum gives zero in the summed physical amplitude.

### Two physical polarizations of a photon

↑ **Parent:** [Photon](#photon)

Two [first-class constraints](classical-mechanics.md#first-class-constraint) in Maxwell theory remove four phase-space variables from the eight variables of a four-component potential and its momenta. The remaining four phase-space variables form two [canonical pairs](classical-mechanics.md#canonical-pair). In [radiation gauge](electromagnetism.md#radiation-gauge) these are transverse polarization modes; circular combinations have [helicity](special-relativity.md#helicity) $+1$ and $-1$. Auxiliary covariant-gauge components do not add physical [photon](#photon) states.

### Photon absorption

↑ **Parent:** [Photon](#photon)

[Photon](#photon) absorption removes a [photon](#photon) and transfers its [energy](classical-mechanics.md#energy) and [momentum](classical-mechanics.md#momentum) to matter. It contributes a negative photon-number collision source. It differs from [Compton scattering](physics.md#compton-scattering), which redistributes a [photon](#photon)'s [energy](classical-mechanics.md#energy) and direction while preserving the count. The integrated source can vanish if [photon emission](#photon-emission) and absorption balance.

### Photon emission

↑ **Parent:** [Photon](#photon)

[Photon](#photon) emission creates a [photon](#photon), for example in [bremsstrahlung](electromagnetism.md#bremsstrahlung) or the decay of an excited material state. It produces a positive photon-number collision source when not balanced by inverse processes. The [photon number current](statistical-physics.md#photon-number-current) is conserved only if its integrated creation and destruction rates cancel.

## Free particle

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_particle)

A free particle has no potential energy, so its Hamiltonian is $H=\mathbf p^2/(2m)$. On unbounded Euclidean space its energy spectrum has no normalizable lowest-energy eigenstate.

## Ground state

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ground_state)

A ground state is an energy eigenstate with the smallest possible energy. For noninteracting particles, the many-body ground state is obtained by filling one-particle levels subject to the particles' exchange statistics.

### Ground-state subspace

↑ **Parent:** [Ground state](#ground-state)

The [ground-state subspace](#ground-state-subspace) is the eigenspace of a [Hamiltonian operator](#hamiltonian-quantum-mechanics) at its lowest [eigenvalue](linear-operator-theory.md#eigenvalue) $E_0$. A [computational history state](quantum-circuit.md#computational-history-state) construction can have many valid [quantum witnesses](computer-science.md#quantum-witness), hence a degenerate [ground space](#ground-state-subspace). Perturbation bounds must optimize on this entire subspace, rather than on a chosen basis of ground states.

### Ground-state degeneracy

↑ **Parent:** [Ground state](#ground-state)

The [ground-state degeneracy](#ground-state-degeneracy) counts independent states minimizing the energy. For a classical continuous-symmetry system it can instead be described by a manifold of minimizing configurations, such as the sphere of orientations of a [Néel state](statistical-physics.md#neel-state) in an isotropic [Heisenberg antiferromagnet](#heisenberg-antiferromagnet).

### Ground-state energy

↑ **Parent:** [Ground state](#ground-state)

The ground-state energy is the smallest [energy eigenvalue](#energy-eigenvalue) of a [Hamiltonian operator](#hamiltonian-quantum-mechanics).

#### Quantum variational principle

↑ **Parent:** [Ground-state energy](#ground-state-energy)

For every normalized trial state $\psi$ in the domain of a [Hamiltonian operator](#hamiltonian-quantum-mechanics) $H$ that is bounded below,

$$
E_0\leq\langle\psi,H\psi\rangle,
$$

where $E_0$ is the [ground-state energy](#ground-state-energy). Equality holds precisely when the trial state lies in the ground-state eigenspace.

##### Exponential variational bound for the Yukawa potential

↑ **Parent:** [Quantum variational principle](#quantum-variational-principle)

For $V=-Ae^{-\mu r}/r$, the normalized exponential with scale $\alpha$ gives $E(\alpha)=\hbar^2\alpha^2/(2m)-4A\alpha^3/(\mu+2\alpha)^2$. Choosing $\alpha=\mu/2$ proves binding if $\mu<Am/\hbar^2$. Failure to obtain a negative trial expectation outside this range does not prove absence of a [bound state](#bound-state). At equality a small positive admixture of the scale-$\mu$ exponential has a negative cross matrix element and proves binding too.

##### Power-law quantum virial theorem

↑ **Parent:** [Quantum variational principle](#quantum-variational-principle)

For a bound stationary state in a homogeneous potential $V(\lambda x)=\lambda^nV(x)$, scaling a normalized wavefunction gives stationarity of $\lambda^2\langle T\rangle+\lambda^{-n}\langle V\rangle$ at $\lambda=1$. Hence $2\langle T\rangle=n\langle V\rangle$.

## Energy eigenvalue

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

An energy eigenvalue $E$ is an [eigenvalue](linear-operator-theory.md#eigenvalue) of the Hamiltonian: $H|\psi\rangle=E|\psi\rangle$ for some nonzero state $|\psi\rangle$.

### Energy eigenstate

↑ **Parent:** [Energy eigenvalue](#energy-eigenvalue)

An energy eigenstate is a nonzero [quantum state](#quantum-state) represented by an eigenvector of the [Hamiltonian operator](#hamiltonian-quantum-mechanics). Its time evolution changes only its overall phase.

### Energy eigenspace

↑ **Parent:** [Energy eigenvalue](#energy-eigenvalue)

The energy eigenspace for $E$ is $\ker(H-EI)$.

### Excited state

↑ **Parent:** [Energy eigenvalue](#energy-eigenvalue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Excited_state)

An excited state is an [energy eigenstate](#energy-eigenvalue) whose energy exceeds the [ground state](#ground-state) energy.

#### First excited state

↑ **Parent:** [Excited state](#excited-state)

The first excited state has the smallest energy strictly above the ground-state energy.

### Eigenstate

↑ **Parent:** [Energy eigenvalue](#energy-eigenvalue)

An eigenstate of an observable is a [quantum state](#quantum-state) represented by an [eigenvector](linear-operator-theory.md#eigenvector) of that observable.

#### Momentum eigenstate

↑ **Parent:** [Eigenstate](#eigenstate)

A momentum eigenstate is an eigenstate of the [momentum operator](#momentum-operator). In one dimension it is a [plane wave](#plane-wave) $e^{ikx}$ with momentum eigenvalue $\hbar k$.

## Quantum system

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_system)

A quantum system is modeled by a complex [Hilbert space](hilbert-space.md); its [quantum states](#quantum-state) describe preparations, while [observables](#observable) describe measurable quantities.

### Quantum state

↑ **Parent:** [Quantum system](#quantum-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_state)

A pure quantum state is a ray in a complex Hilbert space and may be represented by a normalized state vector.

#### Dicke state

↑ **Parent:** [Quantum state](#quantum-state)

The $n$-[qubit](#qubit) Dicke state with $m$ excitations is the normalized equal superposition

$$
|D_m^n\rangle=\binom nm^{-1/2}\sum_{|x|=m}|x\rangle,\qquad 0\leq m\leq n,
$$

where $|x|$ is the [Hamming weight](coding-theory.md#hamming-weight) in the [computational basis](quantum-theory.md#computational-basis). The [binomial coefficient](combinatorics.md#binomial-coefficient) counts the mutually orthogonal summands, proving normalization. Every permutation of the qubits leaves the vector unchanged. Splitting the sum according to the first bit and using $\binom{n-1}{m}/\binom nm=(n-m)/n$ gives

$$
|D_m^n\rangle=\sqrt{\frac{n-m}{n}}|0\rangle|D_m^{n-1}\rangle+\sqrt{\frac mn}|1\rangle|D_{m-1}^{n-1}\rangle.
$$

Terms with zero coefficient are omitted at the endpoints. This recursion is useful for [partial traces](quantum-theory.md#partial-trace) and for distributing a logical [qubit](#qubit) among many symmetric physical qubits.

##### W state

↑ **Parent:** [Dicke state](#dicke-state)

The $n$-[qubit](#qubit) [W state](#w-state) is the [Dicke state](#dicke-state) with one excitation:

$$
|W_n\rangle=\frac1{\sqrt n}\sum_{j=1}^n|0\cdots010\cdots0\rangle=|D_1^n\rangle.
$$

For three [qubits](#qubit) it is $(|001\rangle+|010\rangle+|100\rangle)/\sqrt3$. Its [reduced density matrix](bell-state.md#reduced-density-matrix) on any one [qubit](#qubit) is $\operatorname{diag}((n-1)/n,1/n)$, from the [Dicke state](#dicke-state) recursion. For $n>1$ both diagonal entries are nonzero, so that [qubit](#qubit) is entangled with the rest: a pure [product state](bell-state.md#product-state) would have a pure marginal. A [symmetric-arm reduction of an exchange Hamiltonian](#symmetric-arm-reduction-of-an-exchange-hamiltonian) supplies a dynamical preparation from one initial excitation.

##### One-qubit reduction of Dicke-state superpositions

↑ **Parent:** [Dicke state](#dicke-state)

For $|\Omega\rangle=\alpha|D_m^n\rangle+\beta|D_{m+1}^n\rangle$, $|\alpha|^2+|\beta|^2=1$ and $0\leq m<n$, the [reduced density matrix](bell-state.md#reduced-density-matrix) of any one qubit is

$$
\rho=\frac1n\begin{pmatrix}(n-m)|\alpha|^2+(n-m-1)|\beta|^2&\sqrt{(n-m)(m+1)}\,\alpha\beta^*\\\sqrt{(n-m)(m+1)}\,\alpha^*\beta&m|\alpha|^2+(m+1)|\beta|^2\end{pmatrix}.
$$

Use the [Dicke state](#dicke-state) recursion. The rest-of-system vectors of different [Hamming weights](coding-theory.md#hamming-weight) are orthogonal. For the diagonal terms this leaves the probabilities of the distinguished bit being zero and one. In the cross term, only the rest vector $|D_m^{n-1}\rangle$ occurs in both states, with coefficients $\sqrt{(n-m)/n}$ multiplying $|0\rangle$ and $\sqrt{(m+1)/n}$ multiplying $|1\rangle$. Thus $\operatorname{Tr}_{\mathrm{rest}}(|D_m^n\rangle\langle D_{m+1}^n|)=\sqrt{(n-m)(m+1)}|0\rangle\langle1|/n$, proving the matrix. A single [Dicke state](#dicke-state) alone gives the diagonal matrix $\operatorname{diag}((n-m)/n,m/n)$.

#### Flavor eigenstate

↑ **Parent:** [Quantum state](#quantum-state)

A [flavor eigenstate](#flavor-eigenstate) is a state with a definite flavor label in the specified interaction or flavor-charge basis. For neutral [kaons](physics.md#kaon), $K^0=d\bar s$ and $\bar K^0=s\bar d$ have definite opposite [strangeness](standard-model.md#strangeness). [Weak interactions](standard-model.md#weak-interaction) mix them, so these flavor states are not the [mass eigenstates](numerical-analysis.md#mass-eigenstate). The precise flavor basis must be specified when discussing mixing.

#### Quantum superposition

↑ **Parent:** [Quantum state](#quantum-state)

A normalized [quantum state](#quantum-state) is a [linear combination](vector-space.md#linear-combination) of [orthonormal basis](linear-algebra.md#orthonormal-basis) vectors in a [Hilbert space](hilbert-space.md). Its [density operator](quantum-theory.md#density-matrix) is $|\psi\rangle\langle\psi|$. When at least two basis amplitudes are nonzero, it has off-diagonal terms and differs from the [mixed state](quantum-theory.md#mixed-state) $\sum_j|a_j|^2|j\rangle\langle j|$. [Quantum gates](quantum-circuit.md#quantum-logic-gate) act linearly on this superposition and preserve its phase information.

#### Qudit

↑ **Parent:** [Quantum state](#quantum-state)

A [qudit](#qudit) is a quantum subsystem with $d$ distinguishable basis states and [Hilbert space](hilbert-space.md) $\mathbb C^d$. A [qubit](#qubit) is the special case $d=2$. Tensor products of [qudits](#qudit) give a natural setting for [local Hamiltonians](quantum-theory.md#local-hamiltonian) and finite-dimensional [quantum circuits](quantum-circuit.md).

##### Qudit shift and phase operators

↑ **Parent:** [Qudit](#qudit)

For an $n$-level [qudit](#qudit) and [primitive root of unity](algebra.md#primitive-root-of-unity) $\omega$, these [unitary operators](vector-space.md#unitary-operator) obey $X^n=Z^n=I$ and $ZX=\omega XZ$. The inverse of $X^sZ^{-r}$ is $Z^rX^{-s}$, with the order reversed. These operators implement the receiver corrections in [qudit teleportation](bell-state.md#qudit-teleportation).

#### Qubit

↑ **Parent:** [Quantum state](#quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Qubit)

A qubit is a two-dimensional [quantum system](#quantum-system). Its pure state is a ray in a two-dimensional complex [Hilbert space](hilbert-space.md) and may be written $\alpha|0\rangle+\beta|1\rangle$ with $|\alpha|^2+|\beta|^2=1$.

##### Qubit state

↑ **Parent:** [Qubit](#qubit)

#### Qutrit

↑ **Parent:** [Quantum state](#quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Qutrit)

A qutrit is a three-dimensional [quantum system](#quantum-system), with pure states $\alpha|0\rangle+\beta|1\rangle+\gamma|2\rangle$ satisfying $|\alpha|^2+|\beta|^2+|\gamma|^2=1$. A [qubit](#qubit)-qutrit state is a bipartite state on $\mathbb C^2\otimes\mathbb C^3$.

#### Quantum number

↑ **Parent:** [Quantum state](#quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_number)

A quantum number is a discrete label, usually an observable's eigenvalue, used to distinguish quantum states.

#### Quantum phase

↑ **Parent:** [Quantum state](#quantum-state)

Multiplying a quantum state by one global complex phase does not change any measurement probability; relative phases between components can affect interference.

The [global phase](#global-phase) is common to the whole state; relative phases control interference between state components.

##### Global phase

↑ **Parent:** [Quantum phase](#quantum-phase)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Global_phase)

A global phase multiplies an entire [quantum state](#quantum-state) by one complex number of [modulus](complex-analysis.md#modulus) one. It does not change any measurement probability, unlike a relative phase between components.

###### Global phase of an uncontrolled quantum gate is unobservable

↑ **Parent:** [Global phase](#global-phase)

A physical [unitary gate](quantum-circuit.md#quantum-logic-gate) used without coherent control gives the same [quantum channel](quantum-information-theory.md#quantum-channel) for $V$ and $e^{i\gamma}V$:

$$
(e^{i\gamma}V)\rho(e^{i\gamma}V)^\dagger=V\rho V^\dagger.
$$

Interleaving any preparations, known operations and measurements preserves this equality. Equivalently, each fixed measurement branch with $k$ uses gains only the overall factor $e^{ik\gamma}$, which cancels in its [probability](probability-theory.md#probability). Thus unrestricted repeated uncontrolled uses do not determine the common phase of the [eigenvalues](linear-operator-theory.md#eigenvalue). A supplied [controlled unitary gate](quantum-theory.md#controlled-unitary-gate) is a different resource: $|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes V$ changes by a relative control phase when $V$ is replaced by $e^{i\gamma}V$. Such controlled access permits [quantum phase estimation](quantum-theory.md#quantum-phase-estimation) to measure that phase relative to the identity branch.

#### Observable

↑ **Parent:** [Quantum state](#quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Observable)

A quantum observable is represented by a self-adjoint operator; its possible measured values are spectral values of that operator.

##### Quantum uncertainty

↑ **Parent:** [Observable](#observable)

For a normalized state with finite second moment of a [quantum observable](#observable) $Q$, its uncertainty is the standard deviation of the measurement outcome: $(\Delta Q)^2=\langle Q^2\rangle-\langle Q\rangle^2$. This equals $\|(Q-\langle Q\rangle)\psi\|^2$. The [Robertson uncertainty principle](quantum-theory.md#robertson-uncertainty-principle) bounds products of uncertainties using the expectation of the [commutator](lie-algebra.md#commutator).

##### Expectation value

↑ **Parent:** [Observable](#observable)

In a normalized state $|\psi\rangle$, the expectation of an observable $A$ is $\langle\psi|A|\psi\rangle$.

##### Hamiltonian (quantum mechanics)

↑ **Parent:** [Observable](#observable)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamiltonian_(quantum_mechanics))

The [Hamiltonian operator](#hamiltonian-quantum-mechanics) represents the total [energy](classical-mechanics.md#energy) and generates [unitary time evolution](#unitary-time-evolution) through the [Schrödinger equation](physics.md#schrodinger-equation).

###### Quadratic form of a positive quantum Hamiltonian

↑ **Parent:** [Hamiltonian (quantum mechanics)](#hamiltonian-quantum-mechanics)

For a positive self-adjoint [Hamiltonian operator](#hamiltonian-quantum-mechanics), finite energy means that a normalized state lies in $D(H^{1/2})$, its form domain, and has [expectation value](#expectation-value) $q_H(\psi)$. This domain can be larger than $D(H)$. With a complete orthonormal basis of [energy eigenstates](#energy-eigenstate), $\psi=\sum_nc_ne_n$ and $He_n=E_ne_n$ give $q_H(\psi)=\sum_nE_n|c_n|^2$ by applying $H^{1/2}$ and taking its squared norm. Membership in $D(H)$ instead requires $\sum_nE_n^2|c_n|^2<\infty$. For a Dirichlet free-particle [Hamiltonian operator](#hamiltonian-quantum-mechanics) on an interval, the energy form is $\hbar^2\int|\psi'|^2/(2m)$ on functions with square-integrable weak derivative and zero endpoint values.

###### Morse potential

↑ **Parent:** [Hamiltonian (quantum mechanics)](#hamiltonian-quantum-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morse_potential)

The Morse potential models an anharmonic molecular bond with dissociation energy $D_e>0$, equilibrium separation $x_e$, and inverse length $a>0$. Unlike a [quantum harmonic oscillator](#quantum-harmonic-oscillator), it has finitely many bound levels and a dissociation continuum.

###### Morse oscillator

↑ **Parent:** [Morse potential](#morse-potential)

The quantum Hamiltonian with kinetic energy $p^2/(2\mu)$ and [Morse potential](#morse-potential) has bound energies of the displayed form, where $A=\hbar\omega_e$, $B=A^2/(4D_e)>0$ and $\omega_e=a\sqrt{2D_e/\mu}$. Adjacent energy differences are $A-2B(n+1)$, distinct and positive over the physical bound-level range. A finite truncation with nonzero adjacent dipole couplings therefore satisfies [connected nondegenerate transition chain generates special unitary control](control-theory.md#connected-nondegenerate-transition-chain-generates-special-unitary-control). Controllability of such a truncation does not by itself prove controllability on the full space including dissociation states.

###### Factorized quantum Hamiltonian

↑ **Parent:** [Hamiltonian (quantum mechanics)](#hamiltonian-quantum-mechanics)

For $Q=\hat p-isA(x)$ with real $A$ and positive $s$, the factorization gives potential $(s^2A^2-s\hbar A')/(2m)$ and a nonnegative energy form. Its zero mode is proportional to $\exp[-s\int A\,dx/\hbar]$. Taking $A=x$ and optimizing positivity over $s$ gives the [Heisenberg uncertainty principle](quantum-theory.md#heisenberg-uncertainty-relation) for states with finite second moments.

###### Normalizable zero mode of a polynomial factorized Hamiltonian

↑ **Parent:** [Factorized quantum Hamiltonian](#factorized-quantum-hamiltonian)

For real [polynomial](polynomial.md) $f(x)=cx^n+\cdots$, $c\ne0$, the zero mode of $H=(p+if)(p-if)/(2m)$ is normalizable on $\mathbb R$ exactly when $n$ is odd and $c>0$. Its squared modulus has leading exponential $\exp[-2cx^{n+1}/((n+1)\hbar)]$. Odd $n$ gives the same tail sign at both ends; positivity of $c$ makes both tails decay. This kernel is one-dimensional because $(p-if)\psi=0$ is a first-order [differential equation](differential-equation.md). On the [operator domain](vector-space.md#operator-domain) where integration by parts is valid, the energy form is $\|(p-if)\psi\|^2/(2m)\geq0$.

###### Quantum symmetry of a Hamiltonian

↑ **Parent:** [Hamiltonian (quantum mechanics)](#hamiltonian-quantum-mechanics)

A unitary operator $U$ is a symmetry of a time-independent Hamiltonian $H$ when

$$
U^\dagger H U=H,
$$

equivalently $[U,H]=0$. A differentiable one-parameter symmetry $U(s)=e^{-isQ/\hbar}$ has a self-adjoint generator $Q$ satisfying $[Q,H]=0$, so $Q$ is conserved.

###### Conserved generator of a continuous quantum symmetry

↑ **Parent:** [Quantum symmetry of a Hamiltonian](#quantum-symmetry-of-a-hamiltonian)

If $U(s)=e^{-isQ/\hbar}$ and $U(s)^\dagger H U(s)=H$, differentiation at $s=0$ gives

$$
[Q,H]=0.
$$

In the [Heisenberg picture](#heisenberg-picture),

$$
\frac{dQ}{dt}=\frac i\hbar[H,Q]=0.
$$

###### Unitary time evolution

↑ **Parent:** [Hamiltonian (quantum mechanics)](#hamiltonian-quantum-mechanics)

A time-independent Hamiltonian evolves a state by the unitary operator $U(t)=e^{-iHt/\hbar}$.

###### Perfect quantum state transfer

↑ **Parent:** [Unitary time evolution](#unitary-time-evolution)

A [Hamiltonian operator](#hamiltonian-quantum-mechanics) has perfect transfer between [basis](vector-space.md#basis) states $|a\rangle,|b\rangle$ at time $t_*$ if $e^{-iHt_*}|a\rangle=e^{i\chi}|b\rangle$ for a known [global phase](#global-phase) $\chi$. In an excitation-conserving [qubit](#qubit) network whose vacuum is fixed, the initial [product state](bell-state.md#product-state) with $\alpha|0\rangle+\beta|1\rangle$ at site $a$ and zeros elsewhere evolves to $\alpha|\mathrm{vac}\rangle+\beta e^{i\chi}|b\rangle$. A local [phase gate](quantum-theory.md#phase-gate) at $b$ removing $\chi$ restores the unknown [qubit](#qubit) there. This explains why transfer of the single-excitation [basis](vector-space.md#basis) state suffices for [qubit](#qubit) transfer when the vacuum phase is also accounted for.

<h6 id="schrodinger-picture">Schrödinger picture</h6>

↑ **Parent:** [Unitary time evolution](#unitary-time-evolution)

In the Schrödinger picture, states evolve with the [Hamiltonian operator](#hamiltonian-quantum-mechanics) while observables without explicit time dependence are fixed. For time-independent $H$, the corresponding [Heisenberg picture](#heisenberg-picture) operator is $O_H(t)=e^{iHt/\hbar}O_Se^{-iHt/\hbar}$.

###### Time-evolution operator

↑ **Parent:** [Unitary time evolution](#unitary-time-evolution)

The time-evolution operator maps an initial [quantum state](#quantum-state) to its state at a later time. For a time-independent [Hamiltonian operator](#hamiltonian-quantum-mechanics) $H$, it is the [unitary operator](vector-space.md#unitary-operator) $U(t)=e^{-iHt/\hbar}$.

###### Quantum-mechanical propagator

↑ **Parent:** [Unitary time evolution](#unitary-time-evolution)

A quantum-mechanical propagator is the position-space kernel $K(q_f,t_f;q_i,t_i)=\langle q_f|U(t_f,t_i)|q_i\rangle$ of the time-evolution operator. It is the amplitude to evolve between the specified endpoint configurations.

###### Quantum-mechanical propagator in a constant force

↑ **Parent:** [Quantum-mechanical propagator](#quantum-mechanical-propagator)

In units $\hbar=1$, a particle of mass $m$ with potential $V(q)=-Fq$ has classical path $q_c(t)=q_0+[(q_1-q_0)/T-FT/(2m)]t+Ft^2/(2m)$. Its action and exact [quantum-mechanical propagator](#quantum-mechanical-propagator) are

$$
S_c=\frac{m(q_1-q_0)^2}{2T}+\frac{FT(q_1+q_0)}2-\frac{F^2T^3}{24m},\qquad K_F=\sqrt{\frac{m}{2\pi iT}}e^{iS_c}.
$$

The fluctuation operator is the free one because the potential is linear. This is a special case of [classical-path factorization of a quadratic path integral](quantum-field-theory.md#classical-path-factorization-of-a-quadratic-path-integral).

<h6 id="normalized-short-time-schrodinger-kernel">Normalized short-time Schrödinger kernel</h6>

↑ **Parent:** [Quantum-mechanical propagator](#quantum-mechanical-propagator)

For unit mass and $\hbar=1$, this prepoint kernel tends to the identity and generates the [Time-dependent Schrödinger equation](physics.md#time-dependent-schrodinger-equation). The square-root branch follows the damped [Fresnel integral](analysis.md#fresnel-integral). Its normalized moments are $1$, $0$, and $i\Delta t$ at orders zero, one and two; these fix both the normalization and the kinetic sign.

<h6 id="schrodinger-equation-from-a-short-time-path-integral">Schrödinger equation from a short-time path integral</h6>

↑ **Parent:** [Normalized short-time Schrödinger kernel](#normalized-short-time-schrodinger-kernel)

Expand a smooth [wavefunction](#wave-function) and potential in the [normalized short-time Schrödinger kernel](#normalized-short-time-schrodinger-kernel). Its odd moment vanishes and its second moment is $i\Delta t$, so one step changes the wavefunction by $i\Delta t\,\psi^{\prime\prime}/2-i\Delta tV\psi+O(\Delta t^2)$. Division by the time step gives the [Time-dependent Schrödinger equation](physics.md#time-dependent-schrodinger-equation).

###### Free-particle propagator

↑ **Parent:** [Quantum-mechanical propagator](#quantum-mechanical-propagator)

For a free particle of mass $m$ on the line,

$$
K(x_f,T;x_i,0)=\sqrt{\frac{m}{2\pi i\hbar T}}
\exp\!\left(\frac{im(x_f-x_i)^2}{2\hbar T}\right).
$$

###### Semiclassical propagator

↑ **Parent:** [Quantum-mechanical propagator](#quantum-mechanical-propagator)

A semiclassical propagator sums $e^{iS_{\rm cl}/\hbar}$ over classical paths joining its endpoints, weighted by their quadratic fluctuation determinants and phase indices. It is exact for quadratic actions.

###### Dirichlet fluctuation determinant of a semiclassical propagator

↑ **Parent:** [Semiclassical propagator](#semiclassical-propagator)

Expanding a [configuration-space path integral](quantum-field-theory.md#configuration-space-path-integral) about a classical trajectory $q_c$ with fixed endpoints gives $S[q_c+f]=S[q_c]+\tfrac12\int f\mathcal O_cf\,dt+O(f^3)$, where $f$ obeys homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). The [Gaussian functional integral](quantum-field-theory.md#gaussian-functional-integral) contributes $(\det\mathcal O_c)^{-1/2}$ with the phase prescribed by continuation of the [quantum-mechanical propagator](#quantum-mechanical-propagator). Relative to the free operator $\mathcal O_0=-m\,d^2/dt^2$, the prefactor is $D_0(T)[\det\mathcal O_c/\det\mathcal O_0]^{-1/2}$. In a general potential the operator, and thus the prefactor, depends on the endpoints through $q_c$. For a quadratic potential $V^{\prime\prime}$ is constant and all higher fluctuation terms vanish, so the approximation is exact away from singular focusing times. At a zero mode the simple determinant formula requires a limiting prescription or a different treatment of the zero mode.

###### Van Vleck determinant

↑ **Parent:** [Semiclassical propagator](#semiclassical-propagator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Van_Vleck_determinant)

The Van Vleck determinant is the determinant of mixed endpoint derivatives of a classical action. It measures how nearby classical trajectories focus and supplies the fluctuation prefactor of the [semiclassical propagator](#semiclassical-propagator).

###### Heisenberg picture

↑ **Parent:** [Unitary time evolution](#unitary-time-evolution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heisenberg_picture)

In the Heisenberg picture, states are fixed and an observable evolves as

$$
A_H(t)=U(t)^\dagger A_S U(t).
$$

For a time-independent Schrödinger-picture observable,

$$
\frac{dA_H}{dt}=\frac i\hbar[H,A_H].
$$

###### Heisenberg equation of motion

↑ **Parent:** [Heisenberg picture](#heisenberg-picture)

For an operator $O_H=U^\dagger O_SU$ in the [Heisenberg picture](#heisenberg-picture), differentiating the evolution operators gives $dO_H/dt=i[H_H,O_H]+U^\dagger(\partial O_S/\partial t)U$ in units $\hbar=1$. With no explicit operator time dependence, the second term vanishes. Applying this [commutator](lie-algebra.md#commutator) identity to the [canonical momentum](classical-mechanics.md#canonical-momentum) and [real scalar field](scalar-field-theory.md#real-scalar-field) gives their operator field equations.

###### Interaction picture

↑ **Parent:** [Unitary time evolution](#unitary-time-evolution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interaction_picture)

For $H=H_0+H_{\rm int}$, the interaction picture moves the free evolution into operators and leaves states to evolve with $H_I(t)=e^{iH_0t}H_{\rm int}e^{-iH_0t}$. Its evolution operator is the time-ordered [Dyson series](perturbative-quantum-field-theory.md#dyson-series).

###### Time-reversal symmetry in quantum mechanics

↑ **Parent:** [Unitary time evolution](#unitary-time-evolution)

A time-reversal operator $T$ intertwines forward and backward evolution:

$$
U(t)T=TU(-t).
$$

It must be antiunitary in ordinary quantum mechanics. Its conjugate linearity sends $i$ to $-i$, allowing it to commute with a time-reversal-invariant Hamiltonian rather than reversing the sign of its energy.

###### Quantum time-reversal operator

↑ **Parent:** [Time-reversal symmetry in quantum mechanics](#time-reversal-symmetry-in-quantum-mechanics)

A quantum time-reversal operator is an [antiunitary operator](vector-space.md#antiunitary-operator) reversing spatial [momentum](classical-mechanics.md#momentum) and [angular momentum](classical-mechanics.md#angular-momentum). For a time-reversal-invariant [Hamiltonian operator](#hamiltonian-quantum-mechanics), its conjugation of $i$ makes it intertwine forward and backward [unitary time evolution](#unitary-time-evolution) without reversing the [energy](classical-mechanics.md#energy) spectrum. A scalar [momentum eigenstate](#momentum-eigenstate) may transform as $\hat T|\boldsymbol p\rangle=e^{i\chi(\boldsymbol p)}|-\boldsymbol p\rangle$. With unit-modulus phases and a complete normalized basis, expansion of arbitrary states proves [antiunitarity](vector-space.md#antiunitary-operator).

###### Unitary time reversal reverses the energy spectrum

↑ **Parent:** [Time-reversal symmetry in quantum mechanics](#time-reversal-symmetry-in-quantum-mechanics)

If a unitary $T$ satisfied $U(t)T=TU(-t)$, differentiation at zero would give

$$
HT=-TH.
$$

It would map every energy $E$ to $-E$. A Hamiltonian unbounded above would consequently be unbounded below and have no stable ground state.

###### Antiunitary time reversal preserves the energy spectrum

↑ **Parent:** [Time-reversal symmetry in quantum mechanics](#time-reversal-symmetry-in-quantum-mechanics)

For antiunitary $T$, conjugate linearity gives $T(i\psi)=-iT\psi$. Differentiating

$$
U(t)T=TU(-t)
$$

therefore yields $HT=TH$. Time reversal maps an energy eigenspace to itself and creates no negative-energy instability.

#### Bound state

↑ **Parent:** [Quantum state](#quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bound_state)

A bound state is a normalizable energy eigenstate spatially confined by a potential.

##### Coulomb bound state

↑ **Parent:** [Bound state](#bound-state)

A Coulomb bound state is a physical normalizable eigenfunction for an attractive potential $V(r)=-\gamma/r$, $\gamma>0$. For the usual regular boundary condition at the origin its energies are the displayed values, $N=1,2,\ldots$. The spherically symmetric states have [orbital angular momentum](#orbital-angular-momentum) zero; [series-termination quantization of the Coulomb radial equation](physics.md#series-termination-quantization-of-the-coulomb-radial-equation) constructs them as a polynomial times a decaying exponential. Square integrability on the punctured radial interval alone does not replace the physical condition at the origin.

###### Polynomial construction of hydrogen S states

↑ **Parent:** [Coulomb bound state](#coulomb-bound-state)

For a spherically symmetric bound state, write $\psi=e^{-br}\sum c_jr^j$. The radial Coulomb equation gives the displayed recurrence. Choosing $b=a/(2N)$ terminates it after degree $N-1$, producing a nonzero continuous polynomial times an exponentially decaying function. Its three-dimensional norm $4\pi\int_0^\infty r^2|\psi|^2dr$ is finite and can be normalized. The energy is $-\hbar^2a^2/(8mN^2)$. Continuity at the origin is compatible with the Coulomb cusp; no differentiability as a Cartesian radial function at the origin is asserted.

#### Stationary state

↑ **Parent:** [Quantum state](#quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stationary_state)

A stationary state is an energy eigenstate whose time dependence is only an overall phase.

## Particle in a ring

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Particle_in_a_ring)

A quantum particle constrained to a circle has integer angular-momentum eigenvalues and periodic position eigenfunctions. Its propagator can be written either as a sum over angular momenta or as a sum over [winding number](complex-analysis.md#winding-number) sectors.

## Planck constant

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Planck_constant)

The reduced Planck constant is $\hbar=h/(2\pi)$ and sets the scale of quantum commutators and phases.

## Wave function

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_function)

A wavefunction is a complex amplitude whose squared [modulus](complex-analysis.md#modulus) gives a [probability density](#probability-density).

### Wavefunction normalization

↑ **Parent:** [Wave function](#wave-function)

Wavefunction normalization makes the total [Born rule](#born-rule) probability equal to one. In an [orthonormal basis](linear-algebra.md#orthonormal-basis) of [energy eigenstates](#energy-eigenstate), $\psi=\sum_n c_n\phi_n$ is normalized precisely when $\sum_n|c_n|^2=1$.

### Matter wave

↑ **Parent:** [Wave function](#wave-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matter_wave)

A matter wave is the quantum wave associated with a material particle. Its phase can interfere after coherent paths recombine.

#### Matter-wave interference

↑ **Parent:** [Matter wave](#matter-wave)

Matter-wave interference occurs when coherent spatial branches of a particle's [wavefunction](#wave-function) recombine and their relative [quantum phase](#quantum-phase) changes the detection probabilities.

#### de Broglie wavelength

↑ **Parent:** [Matter wave](#matter-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/de_Broglie_wavelength)

The de Broglie wavelength of a particle with momentum magnitude $p$ is $\lambda=h/p$.

#### Neutron interferometer

↑ **Parent:** [Matter wave](#matter-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neutron_interferometer)

A neutron interferometer coherently splits and recombines neutron matter waves, allowing path-dependent phases to be measured through the output intensity.

<h5 id="colella-overhauser-werner-experiment">Colella–Overhauser–Werner experiment</h5>

↑ **Parent:** [Neutron interferometer](#neutron-interferometer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Colella–Overhauser–Werner_experiment)

The Colella–Overhauser–Werner experiment observed the relative phase acquired by neutron paths at different heights in the Earth's gravitational field.

[https://doi.org/10.1103/PhysRevLett.34.1472](https://doi.org/10.1103/PhysRevLett.34.1472)

### Plane wave

↑ **Parent:** [Wave function](#wave-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plane_wave)

A plane wave has constant amplitude and a phase linear in space and time. It is a [momentum eigenstate](#momentum-eigenstate) and is not spatially normalizable.

### Probability amplitude

↑ **Parent:** [Wave function](#wave-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probability_amplitude)

A probability amplitude is a complex coefficient whose squared modulus gives the probability of the associated measurement outcome.

#### Born rule

↑ **Parent:** [Probability amplitude](#probability-amplitude)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Born_rule)

The Born rule assigns probability $|\langle a|\psi\rangle|^2$ to outcome $a$ when a normalized state $|\psi\rangle$ is measured in an orthonormal eigenbasis.

##### Two-level quantum return probability

↑ **Parent:** [Born rule](#born-rule)

A normalized [quantum state](#quantum-state) $\chi=\sqrt q\,\psi_1+e^{i\eta}\sqrt{1-q}\,\psi_2$ in two orthonormal [energy eigenstates](#energy-eigenstate) returns to its original one-dimensional measurement subspace with probability

$$
|\langle\chi,e^{-iHt/\hbar}\chi\rangle|^2=q^2+(1-q)^2+2q(1-q)\cos((E_1-E_2)t/\hbar).
$$

This follows by applying [unitary time evolution](#unitary-time-evolution) to each [energy eigenstate](#energy-eigenstate), then the [Born rule](#born-rule). The relative phase $\eta$ cancels from the return amplitude. Degenerate energies make the probability identically one.

##### Two-level observable transition probability

↑ **Parent:** [Born rule](#born-rule)

For two orthonormal [energy eigenstates](#energy-eigenstate) $\psi_1,\psi_2$, let an [observable](#observable) have distinct nondegenerate [eigenstates](#eigenstate) $\phi_\pm=(\psi_1\pm\psi_2)/\sqrt2$. Starting in $\phi_-$, [unitary time evolution](#unitary-time-evolution) gives $(e^{-iE_1t/\hbar}\psi_1-e^{-iE_2t/\hbar}\psi_2)/\sqrt2$. Its [probability amplitude](#probability-amplitude) along $\phi_+$ is $(e^{-iE_1t/\hbar}-e^{-iE_2t/\hbar})/2$. The [Born rule](#born-rule) therefore gives the stated transition probability. The energy difference determines the oscillation frequency, while a common energy shift has no effect.

<h5 id="wigner-s-theorem">Wigner's theorem</h5>

↑ **Parent:** [Born rule](#born-rule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wigner's_theorem)

Every bijection of pure-state rays that preserves transition probabilities is induced by either a unitary or an antiunitary operator on the Hilbert space.

###### Projective unitary representation

↑ **Parent:** [Wigner's theorem](#wigner-s-theorem)

Because state vectors differing by a [quantum phase](#quantum-phase) represent the same ray, a unitary realization of a group action need only satisfy

$$
U(g_1)U(g_2)=e^{i\phi(g_1,g_2)}U(g_1g_2).
$$

A [projective unitary representation](#projective-unitary-representation) is a [projective representation](representation-theory.md#projective-representation) whose chosen representatives are unitary operators. The phase factors disappear on rays.

##### Energy measurement

↑ **Parent:** [Born rule](#born-rule)

An ideal energy measurement returns an eigenvalue of the Hamiltonian with probability equal to the squared norm of the state's projection onto its eigenspace. After obtaining a nondegenerate energy, the state is the corresponding energy eigenstate.

### Normalizable wavefunction

↑ **Parent:** [Wave function](#wave-function)

A wavefunction is normalizable when the integral of its squared modulus is finite, so multiplication by a constant can make its total probability one.

### Probability density

↑ **Parent:** [Wave function](#wave-function)

A probability density is a nonnegative [function](function.md) whose [integral](calculus.md#integral) over an event gives its probability.

### Probability current

↑ **Parent:** [Wave function](#wave-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probability_current)

For a nonrelativistic particle of mass $m$, the probability current is

$$
J=-\frac{i\hbar}{2m}
\left(\psi^*\nabla\psi-\psi\nabla\psi^*\right).
$$

#### Probability continuity equation

↑ **Parent:** [Probability current](#probability-current)

For a [wavefunction](#wave-function) satisfying the [Schrödinger equation](physics.md#schrodinger-equation) with a real potential,

$$
\frac{\partial|\psi|^2}{\partial t}+\nabla\cdot J=0.
$$

This [continuity equation](physics.md#continuity-equation) expresses local conservation of probability.

##### Conservation of quantum probability

↑ **Parent:** [Probability continuity equation](#probability-continuity-equation)

If the [probability current](#probability-current) of a [normalizable wavefunction](#normalizable-wavefunction) vanishes at spatial infinity, integrating the [probability continuity equation](#probability-continuity-equation) over all space shows that the total probability $\int |\psi|^2$ is constant in time.

### Gaussian wave packet

↑ **Parent:** [Wave function](#wave-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_wave_packet)

A Gaussian wave packet is a [wavefunction](#wave-function) whose spatial amplitude is a [Gaussian function](calculus.md#gaussian-function). Free quantum evolution preserves its Gaussian form while changing its complex width and spreading its [probability density](#probability-density).

#### Gaussian evolution in an inverted harmonic oscillator

↑ **Parent:** [Gaussian wave packet](#gaussian-wave-packet)

For the [Hamiltonian](#hamiltonian-quantum-mechanics) $H=(p^2-x^2)/2$, a [Gaussian wave packet](#gaussian-wave-packet) $Ae^{-Bx^2}$ satisfies $\dot A=-i\hbar AB$ and $\dot B=-i/(2\hbar)-2i\hbar B^2$. The displayed solution is normalizable for real $\phi$ exactly when $\sin(2\phi)>0$; its [second moments of a complex Gaussian wave packet](#second-moments-of-a-complex-gaussian-wave-packet) are

$$
\langle x^2\rangle=\frac{\hbar[\cosh(2t)+\cos(2\phi)]}{2\sin(2\phi)},\qquad
\langle p^2\rangle=\frac{\hbar[\cosh(2t)-\cos(2\phi)]}{2\sin(2\phi)}.
$$

Both grow as $\hbar e^{2t}/[4\sin(2\phi)]$, while their difference and hence the mean [energy](classical-mechanics.md#energy) remain constant.

## Potential barrier

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

A potential barrier is a region where the potential energy exceeds that in the surrounding regions.

A [rectangular potential barrier](#rectangular-potential-barrier) is the piecewise-constant special case used for exact transmission and reflection calculations.

### Quantum tunnelling

↑ **Parent:** [Potential barrier](#potential-barrier)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_tunnelling)

Quantum tunnelling is transmission through a [potential barrier](#potential-barrier) even when the particle energy is below the barrier height.

#### Double-well tunneling splitting

↑ **Parent:** [Quantum tunnelling](#quantum-tunnelling)

A symmetric two-well system has nearly localized left/right states coupled by a positive [quantum tunnelling](#quantum-tunnelling) magnitude $\Delta=\hbar Ke^{-S_I/\hbar}$. Its effective [Hamiltonian](classical-mechanics.md#hamiltonian) is $E_{\rm well}I-\Delta\sigma_x$, so the superposition with an [even](calculus.md#even-function) spatial [wavefunction](#wave-function) is lower, and the level splitting is $2\Delta$. The [dilute instanton gas](quantum-field-theory.md#dilute-instanton-gas) reproduces these two exponents through even/odd crossing sums.

#### Finite square barrier transmission at half barrier height

↑ **Parent:** [Quantum tunnelling](#quantum-tunnelling)

For a square [potential barrier](#potential-barrier) of width $2a$ and height $U_0=2E$, put

$$
k=\frac{\sqrt{2mE}}{\hbar}.
$$

The oscillatory wavenumber outside and decay constant inside are both $k$. Matching the [wavefunction](#wave-function) and its [derivative](calculus.md#derivative) at both faces gives transmission amplitude

$$
t=\frac{e^{-2ika}}{\cosh(2ka)}
$$

and transmission probability $\operatorname{sech}^2(2ka)$.

## Hermitian operator on a nonorthogonal two-state basis

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

For normalized independent states with $H|\psi\rangle=g|\phi\rangle$ and $H|\phi\rangle=g^*|\psi\rangle$, Hermiticity is equivalent to $g\langle\psi|\phi\rangle\in\mathbb R$. Writing $r=g\langle\psi|\phi\rangle/|g|$, the orthonormal eigenstates are proportional to

$$
(g^*/|g|)|\psi\rangle\pm|\phi\rangle
$$

with eigenvalues $\pm|g|$ and squared norms $2(1\pm r)$.

### Commuting time-dependent two-state Hamiltonian

↑ **Parent:** [Hermitian operator on a nonorthogonal two-state basis](#hermitian-operator-on-a-nonorthogonal-two-state-basis)

If a time-dependent perturbation remains diagonal in a fixed eigenbasis, Hamiltonians at different times commute. Each component therefore acquires the exact phase $\exp[-i\int E_\pm(t)dt/\hbar]$, with no time ordering required.

## Second moments of a complex Gaussian wave packet

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

For a normalized wavefunction $\psi(x)=Ae^{-Bx^2}$ with $\operatorname{Re}B>0$,

$$
\langle x^2\rangle=\frac1{4\operatorname{Re}B},
\qquad
\langle p^2\rangle=\frac{\hbar^2|B|^2}{\operatorname{Re}B}.
$$

## Finite square well

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_square_well)

A finite square well is a bounded interval on which the potential is lower than outside, supporting matched oscillatory and exponential states.

### Attractive potential ordering does not order quantum reflection

↑ **Parent:** [Finite square well](#finite-square-well)

For a square well of width $L$, exterior [wavenumber](wave-equation.md#wavenumber) $k$ and interior [wavenumber](wave-equation.md#wavenumber) $q>k$, matching the [wavefunction](#wave-function) and its [derivative](calculus.md#derivative) gives the [reflection probability](#quantum-reflection-probability) $R=C\sin^2(qL)/(1+C\sin^2(qL))$, where $C=(q^2-k^2)^2/(4k^2q^2)$. For example $q=3k$ and $kL=\pi/2$ give $R=16/25$, whereas zero potential gives $R=0$. Moreover deeper wells at $qL\in\pi\mathbb Z$ have zero reflection by [resonant transmission through a square well](#resonant-transmission-through-a-square-well). Reflection therefore cannot be ordered solely by pointwise ordering of attractive potentials.

### Resonant transmission through a square well

↑ **Parent:** [Finite square well](#finite-square-well)

For an attractive [finite square well](#finite-square-well) of width $a$, outside wave number $k$ and inside wave number $q$, matching the [wavefunction](#wave-function) and its first [derivative](calculus.md#derivative) at both endpoints gives the displayed [transmission probability](#transmission-probability). It equals one when $qa$ is an integer multiple of $\pi$: the internal reflections cancel. For $q=2k$ the coefficient of $\sin^2(qa)$ is $9/16$.

### Spherical square well

↑ **Parent:** [Finite square well](#finite-square-well)

A [spherical square well](#spherical-square-well) is a central potential equal to a negative constant inside a sphere and zero outside it. For an [S-wave scattering](#s-wave-quantum-scattering) state with exterior wave number $k$, the interior wave number obeys $\kappa^2=k^2+2mV_0/\hbar^2$. Continuity of the reduced radial wave and its derivative gives $\kappa\cot(\kappa a)=k\cot(ka+\delta_0)$, relating the depth to the [scattering phase shift](#scattering-phase-shift).

#### Spherically symmetric bound state of a finite well

↑ **Parent:** [Spherical square well](#spherical-square-well)

For well depth $U$ and radius $a$, let $u=r\psi$ for a regular spherically symmetric [wavefunction](#wave-function). At energy $-U<E<0$, the interior is $u=C\sin(kr)$ and the exterior is proportional to $e^{-\kappa r}$, with $k^2=2m(U+E)/\hbar^2$ and $\kappa^2=-2mE/\hbar^2$. Matching gives $k\cot(ka)=-\kappa$. The first negative-energy solution exists strictly above the displayed threshold. At equality the exterior zero-energy wave behaves as $1/r$ and is not square-integrable, so the threshold is not itself a bound state.

### Bound-state thresholds for a square well with one hard wall

↑ **Parent:** [Finite square well](#finite-square-well)

For a zero-potential interval of width $a$, an infinite wall at its left end, and constant exterior potential $U_0$ to its right, the $j$th [bound state](#bound-state) branch exists precisely when $U_0>\mathcal U_j$, for $j=0,1,\ldots$. Matching the [wavefunction](#wave-function) and its derivative gives $z\cot z=-\sqrt{z_0^2-z^2}$ with $z_0=a\sqrt{2mU_0}/\hbar$. At equality the new threshold solution is not [normalizable](#normalizable-wavefunction), so exactly one bound state corresponds to $U_0\in(\mathcal U_0,\mathcal U_1]$.

### Hard-core spherical square-well potential

↑ **Parent:** [Finite square well](#finite-square-well)

For radii $0<a<b$, a hard-core spherical square-well potential has $V(r)=\infty$ for $r\leq a$, $V(r)=-V_0$ for $a<r\leq b$, and $V(r)=0$ for $r>b$. Its radial wavefunction vanishes at the hard-core radius and is matched continuously with its radial derivative at $r=b$.

#### Scattering length of a hard-core spherical square-well potential

↑ **Parent:** [Hard-core spherical square-well potential](#hard-core-spherical-square-well-potential)

For outer radius $b=2a$ and zero-energy well wavenumber $\kappa_0=\sqrt{2mV_0}/\hbar$, matching the [S-wave scattering](#s-wave-quantum-scattering) logarithmic derivative gives

$$
a_s=2a-\frac{\tan(\kappa_0a)}{\kappa_0}.
$$

It diverges when $\kappa_0a=(n+\tfrac12)\pi$, where the well has a [zero-energy scattering resonance](#zero-energy-scattering-resonance).

## Delta potential

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Delta_potential)

A delta potential is a point interaction imposing continuity of the wavefunction and a jump in its derivative.

### Central delta barrier in a symmetric infinite well

↑ **Parent:** [Delta potential](#delta-potential)

Inside walls at $\pm a$, a central [delta potential](#delta-potential) of strength $\kappa$ leaves odd [parity operator](#parity-operator) eigenstates unchanged because their wavefunctions vanish at zero. For even states, continuity and the derivative jump $\psi'(0+)-\psi'(0-)=2m\kappa\psi(0)/\hbar^2$ give the displayed quantization equation. For $\kappa>0$, one root lies between $(n+1/2)\pi/a$ and $(n+1)\pi/a$ for every $n\ge0$.

#### High-energy shift from a central delta barrier

↑ **Parent:** [Central delta barrier in a symmetric infinite well](#central-delta-barrier-in-a-symmetric-infinite-well)

Put $c=m\kappa/\hbar^2$, $k_n=(n+1/2)\pi/a$, and $\delta_n=a(\lambda_n-k_n)$. The quantization equation gives $\delta_n=\arctan(c/\lambda_n)$, so $\lambda_n\delta_n\to c$ and $\delta_n\to0$. Therefore $\lambda_n^2-k_n^2\to2c/a$, proving the displayed absolute [energy](classical-mechanics.md#energy) shift. Its ratio to the unperturbed energy tends to zero. The normalized unperturbed even state has probability density $1/a$ at the origin, so its first-order delta-barrier expectation is also $\kappa/a$.

### Odd bound state and resonance of two delta barriers

↑ **Parent:** [Delta potential](#delta-potential)

For equal delta potentials at $\pm a$, odd parity makes the interior wave proportional to $\sin(kx)$. The derivative jump gives the odd-channel denominator $k\cot(ka)+U_0-ik$. At $k=i\kappa$, its zero is the displayed equation. The function $2\kappa/(1-e^{-2\kappa a})$ increases strictly from $1/a$, proving exactly one odd bound state when $U_0a<-1$. For $U_0a=u\gg1$, the outgoing pole near $ka=\pi$ is $\pi-\pi/u+(\pi-i\pi^2)/u^2+O(u^{-3})$, with positive resonance width.

### Bound state in a delta potential

↑ **Parent:** [Delta potential](#delta-potential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bound_state_in_a_delta_potential)

An attractive one-dimensional delta potential has one even exponentially decaying bound state.

### Multiple delta potential

↑ **Parent:** [Delta potential](#delta-potential)

For delta interactions at points $x_j$, a Green-function solution reduces the Schrodinger equation to a finite linear system for the values $\psi(x_j)$.

#### Symmetric double-delta potential

↑ **Parent:** [Multiple delta potential](#multiple-delta-potential)

The symmetric double-delta potential

$$
V(x)=\frac{\hbar^2U_0}{2m}\bigl(\delta(x-a)+\delta(x+a)\bigr)
$$

separates into even and odd [parity](#parity) channels. At either interaction, the [wavefunction](#wave-function) is continuous and its derivative has the jump

$$
\psi'(a^+)-\psi'(a^-)=U_0\psi(a).
$$

##### Odd-parity S-matrix of a symmetric double-delta potential

↑ **Parent:** [Symmetric double-delta potential](#symmetric-double-delta-potential)

For positive [wavenumber](wave-equation.md#wavenumber) $k$, the odd channel of the [symmetric double-delta potential](#symmetric-double-delta-potential) has

$$
S_{--}(k)=e^{-2ika}
\frac{k e^{ika}+U_0\sin(ka)}{k e^{-ika}+U_0\sin(ka)}.
$$

For real $k$ its numerator and denominator are complex conjugates, making the channel [unitary](vector-space.md#unitary-operator). Its poles are the zeros of $k e^{-ika}+U_0\sin(ka)$.

###### Odd bound state of a symmetric double-delta potential

↑ **Parent:** [Odd-parity S-matrix of a symmetric double-delta potential](#odd-parity-s-matrix-of-a-symmetric-double-delta-potential)

For $U_0<0$, an odd bound state has $k=i\kappa$ with $\kappa>0$ and obeys

$$
2\kappa=-U_0\left(1-e^{-2\kappa a}\right).
$$

A nonzero positive solution exists exactly when $-U_0a>1$; equality is the zero-energy threshold.

###### Odd resonance of a strongly repulsive symmetric double-delta potential

↑ **Parent:** [Odd-parity S-matrix of a symmetric double-delta potential](#odd-parity-s-matrix-of-a-symmetric-double-delta-potential)

For $U_0a\gg1$, the lowest odd [scattering resonance](#scattering-resonance) pole lies near the first odd mode trapped between the barriers:

$$
k=\frac\pi a\left(1-\frac1{U_0a}+O((U_0a)^{-2})\right)
-i\frac{\pi^2}{U_0^2a^3}\left(1+O((U_0a)^{-1})\right)
$$

in its real part and to leading nonzero order in its imaginary part. Writing $E=\hbar^2k^2/(2m)=E_R-i\Gamma/2$, the survival probability decays as $e^{-\Gamma t/\hbar}$.

### Scattering by a delta potential

↑ **Parent:** [Delta potential](#delta-potential)

For $V(x)=V_0\delta(x)$, $E=\hbar^2k^2/(2m)$, and $\gamma=mV_0/(\hbar^2k)$, continuity and the derivative jump give

$$
t=\frac1{1+i\gamma},
\qquad
r=\frac{-i\gamma}{1+i\gamma}.
$$

They obey $|r|^2+|t|^2=1$ and $r^*t+t^*r=0$.

## Quantum scattering

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_scattering)

Quantum scattering compares a wavefunction's incoming and outgoing asymptotic components.

### Quantum reflection probability

↑ **Parent:** [Quantum scattering](#quantum-scattering)

For one-dimensional scattering from a real potential, write the left exterior [wavefunction](#wave-function) as $e^{ikx}+re^{-ikx}$ with $k>0$. The reflected-to-incident probability-current ratio is $R=|r|^2$, since both components have the same speed and their currents have opposite signs. This probability differs from the complex reflection amplitude $r$. With transmission into a right exterior [wavenumber](wave-equation.md#wavenumber) $q$, the [transmission probability](#transmission-probability) is $T=(q/k)|t|^2$ and conservation of current gives $R+T=1$ when there is no absorption.

### Transmission amplitude

↑ **Parent:** [Quantum scattering](#quantum-scattering)

For one-dimensional [quantum scattering](#quantum-scattering), $t$ is the complex amplitude of the outgoing transmitted wave relative to the incoming wave. The [transmission probability](#transmission-probability) is $|t|^2$ times the ratio of transmitted and incident flux velocities; with equal asymptotic dispersion it is $|t|^2$. A [reflectionless potential](#reflectionless-potential) has $r=0$ and a unit-modulus transmission amplitude whose phase shifts continuum quantization. The [supersymmetric factorization of the one-soliton potential](#supersymmetric-factorization-of-the-one-soliton-potential) gives $t(k)=(k+im)/(k-im)$ for its single-bound-state potential.

### S-matrix

↑ **Parent:** [Quantum scattering](#quantum-scattering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/S-matrix)

The [S-matrix](#s-matrix) maps incoming asymptotic states to outgoing asymptotic states. Its connected transition matrix elements contain an overall energy-momentum [Dirac delta function](distribution-theory.md#dirac-delta-function) and an invariant [scattering amplitude](#scattering-amplitude). In [quantum field theory](quantum-field-theory.md), the [LSZ reduction formula](perturbative-quantum-field-theory.md#lsz-reduction-formula) obtains these elements from amputated field correlators.

#### Redundant pole of a scattering matrix

↑ **Parent:** [S-matrix](#s-matrix)

A pole of a [scattering matrix](#s-matrix) arising from the numerator $F(-k)$ rather than a zero of the incoming [Jost function](#jost-function) $F(k)$ can fail to correspond to a [bound state](#bound-state). For $F(k)=(k-i\kappa)/(k+i\alpha)$, the pole at $i\kappa$ is associated with the incoming zero; the pole at $i\alpha$ comes from the numerator. The regular Eckart realization has $\alpha>\kappa$. The distinction and this explicit example are discussed in [https://dipot.ulb.ac.be/dspace/bitstream/2013/373712/4/2306.12216.pdf.](https://dipot.ulb.ac.be/dspace/bitstream/2013/373712/4/2306.12216.pdf.)

#### Jost function

↑ **Parent:** [S-matrix](#s-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jost_function)

For radial [quantum scattering](#quantum-scattering), the incoming coefficient of the regular solution defines the Jost function, with convention $S(k)=F(-k)/F(k)$. A zero at $k=i\kappa$, $\kappa>0$, removes the exponentially growing component and produces a [bound state](#bound-state), subject to regularity and normalizability. Poles of the outgoing numerator alone need not produce [bound states](#bound-state).

#### Unit-modulus hyperbolic scattering block

↑ **Parent:** [S-matrix](#s-matrix)

For real $u$, this scalar [S-matrix](#s-matrix) block satisfies $S_u(\theta)S_u(-\theta)=1$ and [Hermitian analyticity of a two-particle S-matrix](#hermitian-analyticity-of-a-two-particle-s-matrix). It therefore has modulus one for real [rapidity](special-relativity.md#rapidity) differences. For $0<u<\pi$ its [pole](isolated-singularity.md#pole) at $\theta=iu$ has [residue](analysis.md#residue) $2i\sin u$ and admits a direct-channel [bound-state pole](#bound-state-pole-of-the-scattering-amplitude) interpretation. Its crossed block is $\cosh[(\theta-iu)/2]/\cosh[(\theta+iu)/2]$. The endpoints $u=0$ and $u=\pi$ are removable degeneracies giving constant amplitudes, so a particle cannot be inferred there from the uncancelled denominator alone. This block specifies an amplitude; a complete theory must also obey the remaining [crossing symmetry](#crossing-symmetry) and [bootstrap fusion](quantum-field-theory.md#bound-state-fusion-of-factorized-s-matrices) constraints.

#### Physical rapidity strip

↑ **Parent:** [S-matrix](#s-matrix)

For relativistic two-body scattering in one spatial dimension, this strip is the standard domain containing bound-state and crossed-channel [poles](isolated-singularity.md#pole). A stable-particle interpretation requires appropriate [pole](isolated-singularity.md#pole) kinematics and residues; not every singularity automatically represents a new particle. Crossing relates [rapidity](special-relativity.md#rapidity) $\vartheta$ to $i\pi-\vartheta$.

##### Crossed-channel pole in diagonal factorized scattering

↑ **Parent:** [Physical rapidity strip](#physical-rapidity-strip)

A physical-strip [pole](isolated-singularity.md#pole) of a diagonal [S-matrix](#s-matrix) can come from exchange of an existing particle in the crossed channel. For external [masses](classical-mechanics.md#mass) $m_a,m_b$, use the momentum difference, rather than the sum, to identify the exchanged [mass](classical-mechanics.md#mass) through the displayed invariant. [Crossing symmetry](#crossing-symmetry) turns the pole at $i\alpha$ into a direct pole at $i(\pi-\alpha)$ of the particle-antiparticle channel. For $m_B=2m\cos(u/2)$, the [pole](isolated-singularity.md#pole) of $S_{BA}$ at $iu/2$ has $t=m^2$ and exchanges the existing charge-one particle; it is not a new charge-three [bound state](#bound-state).

##### Relativistic bound-state mass from a rapidity pole

↑ **Parent:** [Physical rapidity strip](#physical-rapidity-strip)

At relative [rapidity](special-relativity.md#rapidity) $iu$, the analytically continued sum of the constituent [four-momentum](special-relativity.md#four-momentum) vectors is on the bound-state [mass shell](special-relativity.md#mass-shell) with the displayed [mass](classical-mechanics.md#mass). For equal constituents, [rapidities](special-relativity.md#rapidity) $\chi\pm iu/2$ sum to $2m_a\cos(u/2)(\cosh\chi,\sinh\chi)$. A [pole](isolated-singularity.md#pole) at $u=0$ is at threshold rather than a strictly [bound state](#bound-state).

#### Hermitian analyticity of a two-particle S-matrix

↑ **Parent:** [S-matrix](#s-matrix)

In a real species basis, the two-particle [S-matrix](#s-matrix) satisfies $S(-\theta^*)=S(\theta)^\dagger$ under the usual scattering analyticity assumptions. On the real [rapidity](special-relativity.md#rapidity) axis this relates inverse-rapidity amplitudes to [complex conjugates](complex-analysis.md#complex-conjugate). Combined with the algebraic inverse relation $S(\theta)S(-\theta)=I$, it gives physical [unitarity](vector-space.md#unitary-operator).

### Scattering wavefunction

↑ **Parent:** [Quantum scattering](#quantum-scattering)

For a localized target and a plane wave incident along the $z$-axis, the large-radius scattering wavefunction has the form

$$
\psi(\mathbf r)\sim e^{ikz}+f(\theta,\phi)\frac{e^{ikr}}r,
$$

where $f$ is the [scattering amplitude](#scattering-amplitude).

### Scattering state

↑ **Parent:** [Quantum scattering](#quantum-scattering)

A [scattering state](#scattering-state) is a state used to describe [quantum scattering](#quantum-scattering). Its asymptotic incoming and outgoing components determine a [scattering amplitude](#scattering-amplitude).

### Partial wave

↑ **Parent:** [Quantum scattering](#quantum-scattering)

A partial wave is a component of a scattering state with definite [orbital angular momentum](#orbital-angular-momentum). A [central potential](classical-mechanics.md#central-potential) preserves each angular-momentum channel, so the scattering problem decomposes into independent partial waves.

### Partial-wave scattering

↑ **Parent:** [Quantum scattering](#quantum-scattering)

[Partial-wave scattering](#partial-wave-scattering) decomposes a [scattering state](#scattering-state) into [partial waves](#partial-wave) with definite [orbital angular momentum](#orbital-angular-momentum). For a [central potential](classical-mechanics.md#central-potential), each channel has its own [scattering phase shift](#scattering-phase-shift) and [Partial-wave S-matrix](#partial-wave-s-matrix).

### Differential scattering cross-section

↑ **Parent:** [Quantum scattering](#quantum-scattering)

The differential scattering cross-section is the effective incident area scattered per unit [solid angle](geometry-and-topology.md#solid-angle). It is defined by the ratio of the outgoing particle rate through $d\Omega$ to the incident flux.

#### Central-potential classical differential cross-section

↑ **Parent:** [Differential scattering cross-section](#differential-scattering-cross-section)

For an azimuthally symmetric classical scattering map from [impact parameter](classical-mechanics.md#impact-parameter) $b$ to scattering angle $\theta$,

$$
\frac{d\sigma}{d\Omega}
=\frac{b}{\sin\theta}\left|\frac{db}{d\theta}\right|.
$$

When several impact parameters produce the same angle, their nonnegative contributions are summed.

#### Quantum differential cross-section from a scattering amplitude

↑ **Parent:** [Differential scattering cross-section](#differential-scattering-cross-section)

If

$$
\psi\sim e^{ikz}+f(\theta)\frac{e^{ikr}}r,
$$

then the ratio of scattered radial [probability current](#probability-current) through $r^2d\Omega$ to the incident probability flux is

$$
\frac{d\sigma}{d\Omega}=|f(\theta)|^2.
$$

### Reflected wave

↑ **Parent:** [Quantum scattering](#quantum-scattering)

A reflected wave is an outgoing component travelling back toward the side from which the incident wave arrived.

### Transmission probability

↑ **Parent:** [Quantum scattering](#quantum-scattering)

The transmission probability is the ratio of transmitted to incident [probability current](#probability-current). When the asymptotic wavenumbers agree, it is the squared modulus of the transmission amplitude.

### One-dimensional S-matrix

↑ **Parent:** [Quantum scattering](#quantum-scattering)

For a reflection-invariant localized potential, order incoming amplitudes from the left and right and outgoing amplitudes toward the left and right. Then

$$
S=\begin{pmatrix}r&t\\t&r\end{pmatrix},
$$

where $r$ and $t$ are the reflection and transmission amplitudes. Probability-current conservation makes $S$ unitary for a real potential.

#### Parity basis of a one-dimensional S-matrix

↑ **Parent:** [One-dimensional S-matrix](#one-dimensional-s-matrix)

For a [parity-symmetric](#parity) one-dimensional potential, the even and odd parity states diagonalize the [One-dimensional S-matrix](#one-dimensional-s-matrix):

$$
S_{+-}=S_{-+}=0,
\qquad
S=\operatorname{diag}(S_{++},S_{--}).
$$

For a real potential, [unitarity](vector-space.md#unitary-operator) further gives $|S_{++}|=|S_{--}|=1$ at real positive energy.

#### One-dimensional transfer matrix from scattering amplitudes

↑ **Parent:** [One-dimensional S-matrix](#one-dimensional-s-matrix)

If the left and right travelling-wave coefficients are related by

$$
B_L=rA_L+tB_R,
\qquad
A_R=tA_L+rB_R,
$$

then

$$
\begin{pmatrix}A_R\\B_R\end{pmatrix}
=\frac1t
\begin{pmatrix}t^2-r^2&r\\-r&1\end{pmatrix}
\begin{pmatrix}A_L\\B_L\end{pmatrix}.
$$

### Partial-wave S-matrix

↑ **Parent:** [Quantum scattering](#quantum-scattering)

For a central potential, each angular-momentum channel has a scalar scattering coefficient $S_l(k)=e^{2i\delta_l(k)}$.

Each channel coefficient is a component of the [scattering matrix](#s-matrix) in a basis adapted to rotational symmetry.

#### Scattering phase shift

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

For elastic scattering by a real central potential, the phase shift $\delta_l(k)$ measures the phase difference between the asymptotic radial wave in angular-momentum channel $l$ and the corresponding free wave. Its channel [Partial-wave S-matrix](#partial-wave-s-matrix) is $S_l=e^{2i\delta_l}$.

The phase shift parametrizes elastic [partial-wave scattering](#partial-wave-scattering), rather than general scattering phenomena.

##### Periodic-box phase-shift quantization

↑ **Parent:** [Scattering phase shift](#scattering-phase-shift)

For a reflectionless [scattering wavefunction](#scattering-wavefunction) whose two asymptotic phases differ by $\delta(k)$, a large periodic box gives $k_nL+\delta(k_n)=2\pi n$. Compared with the free value $k_n^{(0)}=2\pi n/L$, $k_n-k_n^{(0)}=-\delta(k_n^{(0)})/L+O(L^{-2})$ away from thresholds. Discrete [bound states](#bound-state) and phase-branch changes alter mode indexing and must be counted when comparing complete spectra.

#### S wave (quantum scattering)

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

An S wave is the rotationally invariant angular-momentum channel $l=0$. At sufficiently low energy it normally dominates short-range scattering because higher partial waves are suppressed by their centrifugal barriers.

#### Partial-wave expansion of a scattering amplitude

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

For a central potential and the convention $S_l=1+2if_l=e^{2i\delta_l}$, the [scattering amplitude](#scattering-amplitude) is

$$
f(\theta)=\frac1k\sum_{l=0}^{\infty}(2l+1)f_lP_l(\cos\theta),
\qquad
f_l=e^{i\delta_l}\sin\delta_l.
$$

The identity $|S_l|=1$ is equivalent to $\operatorname{Im}f_l=|f_l|^2$.

##### Partial-wave total scattering cross-section

↑ **Parent:** [Partial-wave expansion of a scattering amplitude](#partial-wave-expansion-of-a-scattering-amplitude)

For elastic scattering by a central potential,

$$
\sigma_T=\frac{4\pi}{k^2}\sum_{l=0}^{\infty}(2l+1)\sin^2\delta_l.
$$

At low momentum, the [S wave](wave-equation.md#s-wave) normally supplies the leading term.

#### Partial-wave unitarity

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

Partial-wave unitarity bounds each angular-momentum component of a scattering amplitude because its elastic S-matrix eigenvalue has modulus one. Perturbative violation of this bound signals that interactions become strong or that additional degrees of freedom must enter.

#### Unitarity and reflection identities for a partial-wave S-matrix

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

For a real central potential and real $k$, radial-current conservation gives $S_l(k)^*S_l(k)=1$. Invariance of the radial equation under $k\mapsto-k$ gives $S_l(k)S_l(-k)=1$, so a continuous phase convention has $\delta_l(-k)=-\delta_l(k)$.

#### Scattering length from a partial-wave S-matrix

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

The $s$-wave scattering length is

$$
a_s=-\lim_{k\to0}\frac{\tan\delta_0(k)}k,
$$

and the low-energy total cross-section is $4\pi a_s^2$.

##### Repulsive spherical barrier scattering length

↑ **Parent:** [Scattering length from a partial-wave S-matrix](#scattering-length-from-a-partial-wave-s-matrix)

For a barrier of radius $a$ and potential $\hbar^2\gamma^2/(2m)$, matching the regular inner hyperbolic-sine wave to the outer sine wave gives $a_s=a-\tanh(\gamma a)/\gamma$. The low-energy $s$-wave [scattering amplitude](#scattering-amplitude) is $-a_s$.

##### Zero-energy scattering resonance

↑ **Parent:** [Scattering length from a partial-wave S-matrix](#scattering-length-from-a-partial-wave-s-matrix)

A zero-energy scattering resonance occurs when an S-wave bound state reaches the continuum threshold. The zero-energy radial solution then approaches a nonzero constant rather than a generic linear function, and the [scattering length](#scattering-length-from-a-partial-wave-s-matrix) diverges and changes sign.

#### Bound-state poles of a partial-wave S-matrix

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

A pole at $k=i\kappa$ with $\kappa>0$ represents a normalizable bound state of energy $-\hbar^2\kappa^2/(2m)$. Resonance poles instead lie away from the imaginary axis on the analytically continued unphysical sheet.

##### Hyperbolic-tangent S-wave exterior solution

↑ **Parent:** [Bound-state poles of a partial-wave S-matrix](#bound-state-poles-of-a-partial-wave-s-matrix)

For the exterior wave

$$
\psi(r)=\frac{e^{-ikr}}r
+\frac{k+i\lambda\tanh(\lambda r)}{k-i\lambda}
\frac{e^{ikr}}r,
$$

the partial-wave scattering matrix is

$$
S_0(k)=-\frac{k+i\lambda}{k-i\lambda}
=\frac{\lambda-ik}{\lambda+ik}.
$$

Thus $\tan\delta_0=-k/\lambda$, the scattering length is $1/\lambda$, and the pole at $k=i\lambda$ represents a bound state of energy $-\hbar^2\lambda^2/(2m)$ whose exterior wavefunction is proportional to $\operatorname{sech}(\lambda r)/r$.

#### Scattering resonance

↑ **Parent:** [Partial-wave S-matrix](#partial-wave-s-matrix)

A scattering resonance is a metastable state represented by a pole of the analytically continued scattering matrix. Near an isolated narrow resonance, a cross-section has a Breit-Wigner peak whose energy width is the inverse lifetime up to $\hbar$.

##### Resonance pole

↑ **Parent:** [Scattering resonance](#scattering-resonance)

A pole of the continued [scattering matrix](#s-matrix) associated with outgoing boundary conditions and an unstable trapped state. A pole below the real energy axis gives time dependence $e^{-iE_Rt/\hbar}e^{-\Gamma t/(2\hbar)}$, so the probability lifetime is $\hbar/\Gamma$. Bound-state poles instead lie on the positive imaginary wavenumber axis and produce square-integrable decaying spatial waves.

### Logarithmic-derivative matching

↑ **Parent:** [Quantum scattering](#quantum-scattering)

At an interface where a finite potential changes discontinuously, continuity of a radial wavefunction and its derivative is equivalent to matching $u'/u$ on the two sides. This removes the arbitrary normalization constants and gives an equation for the [scattering phase shift](#scattering-phase-shift).

### Hard-sphere limit

↑ **Parent:** [Quantum scattering](#quantum-scattering)

The hard-sphere limit of a repulsive spherical potential makes penetration into a sphere of radius $a$ vanish. Its low-energy [S wave](wave-equation.md#s-wave) scattering length tends to $a$, and its quantum total cross-section tends to $4\pi a^2$.

### Lippmann-Schwinger equation

↑ **Parent:** [Quantum scattering](#quantum-scattering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lippmann-Schwinger_equation)

The Lippmann-Schwinger equation rewrites the Schrodinger differential equation as an integral equation using a free Green function and a prescribed incoming state.

### Scattering amplitude

↑ **Parent:** [Quantum scattering](#quantum-scattering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scattering_amplitude)

A scattering amplitude is the coefficient of an outgoing asymptotic wave relative to the specified incoming wave.

#### Optical theorem

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)

Write the [S-matrix](#s-matrix) as $S=1+iT$. [Unitarity](vector-space.md#unitary-operator) gives $-i(T-T^\dagger)=T^\dagger T$, so the diagonal forward matrix element obeys $2\operatorname{Im}T_{ii}=\sum_f\int d\Phi_f\,|T_{fi}|^2$. Thus the imaginary part of a forward [scattering amplitude](#scattering-amplitude) measures the total inclusive transition rate. For an electromagnetic source, the [hadronic electromagnetic-current spectral density](perturbative-quantum-field-theory.md#hadronic-electromagnetic-current-spectral-density) supplies the inclusive spectral sum.

#### Scattering-amplitude factorization

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)

Near a one-particle pole, a [scattering amplitude](#scattering-amplitude) factors into amplitudes coupling each side to the intermediate state, summed over its physical polarizations. The pole position gives its squared [mass](classical-mechanics.md#mass), while its [residue](analysis.md#residue) encodes its spin and couplings.

#### Crossing symmetry

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crossing_symmetry)

Crossing symmetry relates [scattering amplitudes](#scattering-amplitude) by analytic continuation exchanging incoming and outgoing particles. A symmetric four-point scalar amplitude has equivalent descriptions under permutations of the [Mandelstam variables](special-relativity.md#mandelstam-variables).

#### Relativistic scattering cross-section

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)

With relativistically normalized external states, a two-particle initial state has differential cross-section $d\sigma=|\mathcal M|^2d\Phi_n/\mathcal F$, where $d\Phi_n$ is the [Lorentz-invariant phase-space measure](#lorentz-invariant-phase-space-measure) and $\mathcal F$ is the [invariant flux factor](#invariant-flux-factor). For identical unobserved final particles, divide the full labeled phase-space integral by their permutation multiplicity.

##### Inclusive electron-positron annihilation into hadrons

↑ **Parent:** [Relativistic scattering cross-section](#relativistic-scattering-cross-section)

At leading electromagnetic order and with negligible electron mass, the photon-channel [relativistic cross-section](#relativistic-scattering-cross-section) is $\sigma_h=4\pi^2\alpha\rho_h=16\pi^3\alpha^2\rho_J/s$, in the stated [hadronic photon spectral density](quantum-field-theory.md#hadronic-photon-spectral-density) and [hadronic electromagnetic-current spectral density](perturbative-quantum-field-theory.md#hadronic-electromagnetic-current-spectral-density) conventions. Initial electron and positron spins are averaged; final hadronic states are summed inclusively. Electroweak channels beyond photon exchange are separate contributions.

###### Hadronic R ratio

↑ **Parent:** [Inclusive electron-positron annihilation into hadrons](#inclusive-electron-positron-annihilation-into-hadrons)

The [hadronic R ratio](#hadronic-r-ratio) normalizes the photon-channel hadronic [relativistic cross-section](#relativistic-scattering-cross-section) to the leading massless muon-pair value. The free active-quark result is $R=N_c\sum_fQ_f^2$. It depends on flavor charges as well as the number of active flavors; it is not simply $N_cN_f$.

##### Elastic scattering from a quartic scalar contact interaction

↑ **Parent:** [Relativistic scattering cross-section](#relativistic-scattering-cross-section)

The factorial-normalized quartic vertex gives an angle-independent tree amplitude of magnitude $|\lambda|$. For equal incoming and outgoing masses, the momentum ratio in the two-body cross-section cancels. The event density for identical outgoing particles over a full sphere is $\lambda^2/(128\pi^2s)$. On a hemisphere representing each event once, the density is $\lambda^2/(64\pi^2s)$. Both conventions give total event cross-section $\lambda^2/(32\pi s)$.

##### Invariant flux factor

↑ **Parent:** [Relativistic scattering cross-section](#relativistic-scattering-cross-section)

For two incident particles in relativistic normalization, this is $2\sqrt{\kappa(s,m_1^2,m_2^2)}$, where $\kappa$ is the [Källén function](special-relativity.md#kallen-function). For equal masses it is $2\sqrt{s(s-4m^2)}$.

##### Lorentz-invariant phase-space measure

↑ **Parent:** [Relativistic scattering cross-section](#relativistic-scattering-cross-section)

The on-shell measure $d^3p/(2E)$ is Lorentz invariant. The product measure together with the four-dimensional [Dirac delta distribution](distribution-theory.md#dirac-delta-function) enforces [four-momentum conservation](special-relativity.md#four-momentum-conservation). For equal masses in two-body scattering, $d\Phi_2=\sqrt{1-4m^2/s}\,d\Omega/(32\pi^2)$.

###### Relativistic two-body phase space

↑ **Parent:** [Lorentz-invariant phase-space measure](#lorentz-invariant-phase-space-measure)

For two outgoing particles with centre-of-mass momentum magnitude $k$ and total energy $\sqrt s$, integrating the four-momentum delta function gives $d\Phi_2/d\Omega=k/(16\pi^2\sqrt s)$. A factor $1/2!$ for identical outgoing particles is inserted when counting events over the full phase space, not into this labelled kinematic measure itself.

###### Positive-energy on-shell delta function identity

↑ **Parent:** [Lorentz-invariant phase-space measure](#lorentz-invariant-phase-space-measure)

For $E>0$ and the positive-energy branch, the root Jacobian of the [Dirac delta function](distribution-theory.md#dirac-delta-function) gives this identity. In a [massless collinear parton approximation](standard-model.md#massless-collinear-parton-approximation), it produces $\delta(x-\xi)/(P\cdot q)$.

###### Two-body decay phase space

↑ **Parent:** [Lorentz-invariant phase-space measure](#lorentz-invariant-phase-space-measure)

This total decay-width formula applies in the parent's rest frame when the squared [scattering amplitude](#scattering-amplitude) is independent of direction and the daughters are distinct. For identical daughters an additional symmetry factor is needed.

###### Identical-particle factor in a final-state phase-space integral

↑ **Parent:** [Lorentz-invariant phase-space measure](#lorentz-invariant-phase-space-measure)

When the full [Lorentz-invariant phase-space measure](#lorentz-invariant-phase-space-measure) treats $n$ identical final particles as labeled, each physical final configuration is counted $n!$ times. The unlabelled [relativistic scattering cross-section](#relativistic-scattering-cross-section) therefore includes $1/n!$. For two identical scalars, this divides the full-angle result by two; equivalently, integrate over a region containing only one representative of each exchanged pair.

#### Momentum transfer

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Momentum_transfer)

The momentum transfer in a scattering process is the difference between the incoming and outgoing [wavevectors](continuum-mechanics.md#wavevector), commonly $Q=k-k'$ up to a sign convention and a factor of $\hbar$.

#### Elastic scattering

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elastic_scattering)

Elastic scattering preserves the total kinetic energy. For one particle scattered by a fixed target, the incoming and outgoing [wavevectors](continuum-mechanics.md#wavevector) therefore have equal magnitudes.

#### Diffraction

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diffraction)

Diffraction is interference produced when waves scatter from spatial structure. A periodic structure concentrates the scattered intensity at reciprocal-lattice conditions.

#### Crystal scattering

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)

In the [Born approximation](quantum-theory.md#born-approximation), scattering from identical atomic potentials translated to lattice sites factors into one atomic form factor times a finite sum of phases over the crystal sites.

##### Bravais lattice

↑ **Parent:** [Crystal scattering](#crystal-scattering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bravais_lattice)

A three-dimensional Bravais lattice is

$$
\Lambda=\{n_1a_1+n_2a_2+n_3a_3:n_i\in\mathbb Z\},
$$

where the primitive vectors $a_1,a_2,a_3$ are linearly independent.

###### Unit cell

↑ **Parent:** [Bravais lattice](#bravais-lattice)

A region whose translates tile a lattice's ambient space, together with the lattice points represented in it. A [primitive unit cell](#primitive-unit-cell) represents one lattice point; a conventional unit cell may represent several to display symmetry.

###### Primitive unit cell

↑ **Parent:** [Unit cell](#unit-cell)

A fundamental cell of a [Bravais lattice](#bravais-lattice), of volume equal to the absolute [determinant](linear-algebra.md#determinant) of any primitive lattice basis. Direct and [reciprocal lattice](#reciprocal-lattice) primitive cell volumes multiply to $(2\pi)^d$ in dimension $d$ with the angular-wavenumber convention.

###### Face-centered tetragonal lattice

↑ **Parent:** [Bravais lattice](#bravais-lattice)

A tetragonal conventional cell with lattice points at its vertices and face centers describes a [Bravais lattice](#bravais-lattice). It is equivalent, after a rotation and a change of conventional cell, to a body-centered tetragonal description. The [reciprocal lattice](#reciprocal-lattice) of a body-centered tetragonal lattice with conventional sides $a,a,b$ consists of $2\pi(h/a,k/a,l/b)$ with $h+k+l$ even; these points form a face-centered tetragonal conventional cell with sides $4\pi/a,4\pi/a,4\pi/b$.

###### Face-centered cubic lattice

↑ **Parent:** [Bravais lattice](#bravais-lattice)

A face-centered cubic lattice has lattice points at every corner and face center of a conventional cube. One primitive cell has one quarter of the conventional cube's volume.

###### Lattice point

↑ **Parent:** [Bravais lattice](#bravais-lattice)

A lattice point is a vector $l=n_1a_1+n_2a_2+n_3a_3$ whose coefficients in a chosen primitive [basis](vector-space.md#basis) are [integers](number-theory.md#integer).

###### Reciprocal lattice

↑ **Parent:** [Bravais lattice](#bravais-lattice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reciprocal_lattice)

The reciprocal lattice is

$$
\Lambda^*=\{q:q\cdot l\in2\pi\mathbb Z\text{ for every }l\in\Lambda\}.
$$

If $\Omega=a_1\cdot(a_2\times a_3)$, its primitive vectors are

$$
b_1=2\pi\frac{a_2\times a_3}{\Omega},
\quad
b_2=2\pi\frac{a_3\times a_1}{\Omega},
\quad
b_3=2\pi\frac{a_1\times a_2}{\Omega},
$$

and satisfy $a_i\cdot b_j=2\pi\delta_{ij}$.

###### Wigner-Seitz cell

↑ **Parent:** [Reciprocal lattice](#reciprocal-lattice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wigner–Seitz_cell)

The Wigner--Seitz cell of a lattice point consists of points at least as close to it as to every other lattice point. Its faces lie on perpendicular bisectors to neighbouring lattice points.

###### Reciprocal lattice and Wigner-Seitz cell of the unit triangular lattice

↑ **Parent:** [Wigner-Seitz cell](#wigner-seitz-cell)

For direct primitive vectors $(1,0)$ and $(-1/2,\sqrt3/2)$, reciprocal primitive vectors are

$$
\left(2\pi,\frac{2\pi}{\sqrt3}\right),
\qquad
\left(0,\frac{4\pi}{\sqrt3}\right).
$$

The reciprocal Wigner--Seitz cell is a regular hexagon of area $8\pi^2/\sqrt3$ and circumradius $4\pi/3$.

###### Cubic crystal system

↑ **Parent:** [Bravais lattice](#bravais-lattice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cubic_crystal_system)

The [cubic crystal system](#cubic-crystal-system) has cubic point symmetry. Its three cubic [Bravais lattices](#bravais-lattice) are primitive, body-centered, and face-centered. The [body-centered cubic lattice](#body-centered-cubic-lattice) is one member of that classification.

###### Body-centered cubic lattice

↑ **Parent:** [Cubic crystal system](#cubic-crystal-system)

A body-centered cubic lattice consists of the points of a cubic lattice together with their body centers. Its reciprocal lattice is face-centered cubic.

###### Reciprocal lattice of the 2023 Cambridge body-centered cubic basis

↑ **Parent:** [Body-centered cubic lattice](#body-centered-cubic-lattice)

For

$$
a_1=\frac a2(1,1,1),
\quad a_2=\frac a2(1,-1,1),
\quad a_3=a(0,0,1),
$$

a reciprocal basis is

$$
b_1=\frac{2\pi}{a}(1,1,0),
\quad b_2=\frac{2\pi}{a}(1,-1,0),
\quad b_3=\frac{2\pi}{a}(-1,0,1).
$$

Thus $\Lambda^*=(2\pi/a)\{(h,k,l)\in\mathbb Z^3:h+k+l\text{ even}\}$ and its shortest nonzero vectors have length $2\sqrt2\pi/a$.

##### Crystal lattice structure factor

↑ **Parent:** [Crystal scattering](#crystal-scattering)

For a finite set $S$ of crystal sites, the lattice structure factor at momentum transfer $Q$ is

$$
\Delta(Q)=\sum_{l\in S}e^{iQ\cdot l}.
$$

It multiplies the single-atom [scattering amplitude](#scattering-amplitude).

###### Reciprocal-lattice peaks of a finite crystal

↑ **Parent:** [Crystal lattice structure factor](#crystal-lattice-structure-factor)

For $S=\{\sum_il_ia_i:-L_i/2\leq l_i\leq L_i/2\}$ and $\alpha_i=Q\cdot a_i$,

$$
\Delta(Q)=\prod_{i=1}^3
\frac{\sin((L_i+1)\alpha_i/2)}{\sin(\alpha_i/2)}.
$$

For large $L_i$, each factor is sharply peaked when $\alpha_i\in2\pi\mathbb Z$, exactly the condition $Q\in\Lambda^*$.

##### Elastic Bragg scattering condition

↑ **Parent:** [Crystal scattering](#crystal-scattering)

For elastic scattering with $k-k'=q\in\Lambda^*$ and $|k|=|k'|=k$,

$$
2k\cdot q=|q|^2,
\qquad
|q|=2k\sin\frac\theta2.
$$

The smallest nonzero diffraction angle is determined by the shortest reciprocal-lattice vector.

This reciprocal-lattice condition is equivalent to [Bragg's law](#bragg-s-law), expressed in terms of the lattice-plane spacing and the wavelength.

<h6 id="bragg-s-law">Bragg's law</h6>

↑ **Parent:** [Elastic Bragg scattering condition](#elastic-bragg-scattering-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bragg's_law)

Constructive interference between waves reflected by successive equally spaced lattice planes requires their path difference $2d\sin\theta$ to be an integer multiple of the wavelength $\lambda$. Here $d$ is plane spacing, $\theta$ is the glancing angle and $m$ is the diffraction order.

###### Bragg scattering

↑ **Parent:** [Elastic Bragg scattering condition](#elastic-bragg-scattering-condition)

Bragg scattering is coherent elastic scattering from a periodic lattice, enhanced when the wavevector transfer is a [reciprocal lattice](#reciprocal-lattice) vector. Finite crystals have narrow rather than infinitely sharp reciprocal-space peaks.

#### Bound-state pole of the scattering amplitude

↑ **Parent:** [Scattering amplitude](#scattering-amplitude)

After analytic continuation in momentum, a pole at $k=i\kappa$ with $\kappa>0$ gives negative energy and spatial decay, and therefore represents a bound state.

## Supersymmetric quantum mechanics

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersymmetric_quantum_mechanics)

Supersymmetric quantum mechanics factors partner Hamiltonians through first-order operators. Its odd supercharges anticommute to the Hamiltonian; on a Riemannian manifold, the Hilbert space can be realized by square-integrable differential forms with supercharges given by a differential and its adjoint.

### Supersymmetric factorization and zero-mode normalizability

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)

The candidate zero modes are $e^{-\int^xw}$ in the minus sector and $e^{+\int^xw}$ in the plus sector; this follows from the positive squared-norm expressions for their energy. Their membership in the [Hilbert space](hilbert-space.md) determines whether [supersymmetry](supersymmetry.md) is unbroken. For $w=x$ only the first is normalizable. For $w=x^2+a$, $a>0$, neither is normalizable, while both partner potentials grow quartically and have discrete spectra. Thus their strictly positive lowest energy is paired and [supersymmetry](supersymmetry.md) is broken, with zero [Witten index](#witten-index).

### Witten index

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)

With a well-defined regulated supertrace, positive-energy states of [supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics) are paired by an odd invertible charge. Their opposite [fermion parities](topological-quantum-matter.md#fermion-parity) cancel, leaving $I=n_B^0-n_F^0$, independent of $\beta$. A nonzero index proves the existence of a [supersymmetric vacuum](supersymmetry.md#supersymmetric-vacuum); zero does not prove its absence. Discrete-spectrum or suitable infrared conditions matter, because continuum thresholds and states escaping to infinity can invalidate naive trace manipulations or deformation invariance.

### Gradient superpotential Hamiltonian in supersymmetric quantum mechanics

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)

For a real smooth function $\chi$ on [Euclidean space](functional-analysis.md#euclidean-norm), put $A_a=\partial_a-\partial_a\chi$ and $q=\sum_a\psi_a^\dagger A_a$. The [adjoint operator](hilbert-space.md#adjoint-operator) for the usual $L^2$ [inner product](linear-algebra.md#inner-product) is $A_a^\dagger=-\partial_a-\partial_a\chi$. Since $[A_a,A_b]=0$, the [canonical anticommutation relations](#canonical-anticommutation-relations) give $q^2=0$. Expanding $H=\{q,q^\dagger\}$ and using $[A_a,A_b^\dagger]=-2\partial_a\partial_b\chi$ gives

$$
H=(-\Delta+|\nabla\chi|^2+\Delta\chi)I-2\sum_{a,b}(\partial_a\partial_b\chi)\psi_a^\dagger\psi_b.
$$

In the empty [fermionic Fock space](#fermionic-fock-space) sector the last term vanishes; in the filled sector $\psi_a^\dagger\psi_b=\delta_{ab}$. Consequently the two scalar [Hamiltonian operators](#hamiltonian-quantum-mechanics) are $H_0=-\Delta+|\nabla\chi|^2+\Delta\chi$ and $H_d=-\Delta+|\nabla\chi|^2-\Delta\chi$. On the compatible [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) domain the [Hamiltonian operator](#hamiltonian-quantum-mechanics) is nonnegative because $\langle v,Hv\rangle=\|qv\|^2+\|q^\dagger v\|^2$.

#### Zero mode in the fermion-vacuum sector

↑ **Parent:** [Gradient superpotential Hamiltonian in supersymmetric quantum mechanics](#gradient-superpotential-hamiltonian-in-supersymmetric-quantum-mechanics)

For the [gradient superpotential Hamiltonian in supersymmetric quantum mechanics](#gradient-superpotential-hamiltonian-in-supersymmetric-quantum-mechanics), $H_0=\sum_aA_a^\dagger A_a$. A zero-energy [normalizable wavefunction](#normalizable-wavefunction) therefore satisfies $A_af=0$ for every $a$, because its energy is $\sum_a\|A_af\|^2$. Equivalently $\partial_a(e^{-\chi}f)=0$, so on a connected configuration space $f=Ce^\chi$. It exists in the [Hilbert space](hilbert-space.md) precisely when $e^\chi$ is [square-integrable](measure-theory.md#square-integrable-function). In three dimensions with radial $\chi$, this requires $4\pi\int_0^\infty r^2e^{2\chi(r)}\,dr<\infty$. The sign depends on the convention $A=\partial-\partial\chi$; the filled sector instead has the possible zero mode $e^{-\chi}$.

### Fermion-number sectors in supersymmetric quantum mechanics

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)

For $d$ [fermionic creation operators](relativistic-quantum-field.md#fermionic-creation-operator) with the [canonical anticommutation relations](#canonical-anticommutation-relations), the [Hilbert space](hilbert-space.md) $L^2(\mathbb R^d)\otimes\Lambda^\bullet\mathbb C^d$ splits into $\mathcal H_n=L^2(\mathbb R^d)\otimes\Lambda^n\mathbb C^d$, $0\leq n\leq d$. The [fermion number operator](#fermion-number-operator) $N=\sum_a\psi_a^\dagger\psi_a$ has value $n$ on $\mathcal H_n$; its internal multiplicity is $\binom dn$. An odd [supercharge](supersymmetry.md#supersymmetry-generator) $Q=q+q^\dagger$, with $q$ raising $n$ and $q^2=0$, gives $H=\{q,q^\dagger\}$ and preserves these sectors.

On an [eigenspace](linear-operator-theory.md#eigenspace) with $E>0$, $Q/\sqrt E$ is an [odd involution pairing bosonic and fermionic states](supersymmetry.md#odd-involution-pairing-bosonic-and-fermionic-states). More precisely,

$$
v=E^{-1}(qq^\dagger+q^\dagger q)v
$$

gives an [orthogonal decomposition](hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) of each state into the images of $q$ and $q^\dagger$: their [inner product](linear-algebra.md#inner-product) vanishes because $(q^\dagger)^2=0$. If $u\in\operatorname{im}q^\dagger$, then $q^\dagger u=0$, $q^\dagger qu=Eu$ and $\|qu\|^2=E\|u\|^2$. Thus $q/\sqrt E$ pairs such a state in degree $n$ with one in degree $n+1$, and $q^\dagger/\sqrt E$ is the inverse. States with zero energy are killed by both operators and may remain unpaired. The pairing applies to positive spectral subspaces as well; discreteness is not implied.

#### Radial superpartner in three-dimensional supersymmetric quantum mechanics

↑ **Parent:** [Fermion-number sectors in supersymmetric quantum mechanics](#fermion-number-sectors-in-supersymmetric-quantum-mechanics)

Let $\chi=\chi(r)$, $r=|x|$, and let $f(r)|0\rangle$ be a normalized [eigenstate](#eigenstate) of $H_0$ with $E>0$, where $|0\rangle$ is the [Clifford vacuum](#clifford-vacuum). Acting with the [supercharge](supersymmetry.md#supersymmetry-generator) differentiates only its [wavefunction](#wave-function):

$$
Qf(r)|0\rangle=(f'-\chi'f)\psi_r^\dagger|0\rangle,
\qquad \psi_r^\dagger=\sum_a\frac{x_a}{r}\psi_a^\dagger.
$$

The normalized partner is $E^{-1/2}(f'-\chi'f)\psi_r^\dagger|0\rangle$. Indeed $[H,Q]=0$, and $\|Qf|0\rangle\|^2=E\|f|0\rangle\|^2$; acting with $Q$ again returns $\sqrt E$ times the original state. The expression at $r=0$ is interpreted by the regular extension of the original state. Although its coefficient depends only on $r$, its degree-one components contain the radial unit vector.

### Fermionic Fock space

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)

The fermionic Fock space of $n$ modes is the exterior algebra $\Lambda^\bullet\mathbb C^n$. Creation acts by exterior multiplication and annihilation by contraction.

#### Polarized fermionic Fock space

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

An orthogonal projection $P$ splits a one-particle [Hilbert space](hilbert-space.md) into empty and filled modes. Take completed exterior Fock spaces of empty particles and of holes in the filled modes, with the graded tensor product enforcing the [canonical anticommutation relations](#canonical-anticommutation-relations) between both factors. The vacuum is killed by particle annihilation in $PH$ and by particle creation in $(I-P)H$. Only finite particle-hole excitations are needed for a dense basis. Normal ordering subtracts the filled-vacuum expectation from bilinear observables.

##### Fermion-boson correspondence on the circle

↑ **Parent:** [Polarized fermionic Fock space](#polarized-fermionic-fock-space)

In charge $q$, let $\Omega_q$ fill all integer modes below $q$. Its rotation energy is $q(q-1)/2$. The negative [Heisenberg current algebra of a fermion on the circle](#heisenberg-current-algebra-of-a-fermion-on-the-circle) modes create mutually commuting oscillators $b_n^*=J_{-n}/\sqrt n$ with $[b_n,b_m^*]=\delta_{nm}$. Their normalized occupation monomials applied to $\Omega_q$ are orthonormal. The [Jacobi triple product](modular-function.md#jacobi-triple-product) identifies the fermionic charge-energy generating function with $\sum_q u^q t^{q(q-1)/2}\prod_{n>0}(1-t^n)^{-1}$, proving completeness in each finite-dimensional energy space. Thus the rotation Hamiltonian is $Q(Q-1)/2+\sum_{n>0}n b_n^*b_n$.

##### Heisenberg current algebra of a fermion on the circle

↑ **Parent:** [Polarized fermionic Fock space](#polarized-fermionic-fock-space)

For integer modes filled at indices below zero, set $E_{rs}=c_r^\dagger c_s-\delta_{rs}\mathbf1_{r<0}$ and $J_n=\sum_r E_{r,r+n}$ on the finite-energy domain. The [canonical anticommutation relations](#canonical-anticommutation-relations) give a central term $\delta_{st}\delta_{ur}(\mathbf1_{r<0}-\mathbf1_{s<0})$ in $[E_{rs},E_{tu}]$. Summing across the filled-empty boundary gives $[J_n,J_m]=n\delta_{n+m,0}I$, with $J_n^*=J_{-n}$. The current's level is the coefficient of this central term.

###### Fermionic current on the circle

↑ **Parent:** [Heisenberg current algebra of a fermion on the circle](#heisenberg-current-algebra-of-a-fermion-on-the-circle)

A Fourier mode of the normal-ordered fermion density is a fermionic current. On the finite-energy domain its defining sum has finitely many nonzero actions on each occupation vector. The modes satisfy $J_n^*=J_{-n}$ and $[J_n,J_m]=n\delta_{n+m,0}I$. The zero mode is charge; positive modes annihilate charge ground states and negative modes create the oscillators in the [fermion-boson correspondence on the circle](#fermion-boson-correspondence-on-the-circle).

##### Segal quantization criterion for fermions

↑ **Parent:** [Polarized fermionic Fock space](#polarized-fermionic-fock-space)

For the irreducible representation of the [canonical anticommutation relations](#canonical-anticommutation-relations) determined by $P$, a unitary one-particle map $u$ is unitarily implementable precisely when $P-uPu^*$ is [Hilbert-Schmidt](compact-operator.md#hilbert-schmidt-operator), equivalently when $[P,u]$ is Hilbert-Schmidt. The implementer is unique up to a scalar phase. The equivalent representation criterion for two polarizations is that their projections differ by a Hilbert-Schmidt operator. This yields a continuous [projective unitary representation](#projective-unitary-representation) of the [restricted unitary group](topological-group.md#restricted-unitary-group).

#### Fermionic operator

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

A [fermionic operator](#fermionic-operator) is odd under [fermion parity](topological-quantum-matter.md#fermion-parity): if $P=(-1)^N$ is the parity operator, then $PAP=-A$. A [fermionic creation operator](relativistic-quantum-field.md#fermionic-creation-operator) or [fermionic annihilation operator](relativistic-quantum-field.md#fermionic-annihilation-operator) is an example. Interchanging odd insertions in a [time-ordered product](perturbative-quantum-field-theory.md#time-ordered-product) contributes the corresponding [fermionic sign](perturbative-quantum-field-theory.md#fermionic-sign). Odd parity alone does not imply that every pair of such operators has zero [anticommutator](vector-space.md#anticommutator).

#### Clifford vacuum

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

A Clifford vacuum is a state annihilated by all the chosen fermionic annihilation operators. In a [massless supermultiplet](supersymmetry.md#massless-supermultiplet) it labels the starting [helicity](special-relativity.md#helicity), and applying [fermionic raising and lowering operators](#fermionic-raising-and-lowering-operator) constructs the remaining states.

#### Canonical anticommutation relations

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

Fermionic creation and annihilation operators satisfy $\{a_i,a_j^\dagger\}=\delta_{ij}$ and vanishing equal-type anticommutators. These relations make each mode either empty or singly occupied.

##### Fermionic bilinear charge algebra

↑ **Parent:** [Canonical anticommutation relations](#canonical-anticommutation-relations)

For constant internal matrices acting on [Dirac fields](relativistic-quantum-field.md#dirac-field), the equal-time [canonical anticommutation relations](#canonical-anticommutation-relations) give

$$
[\psi_i^\dagger\psi_j,\psi_k^\dagger\psi_l]=\delta_{jk}\psi_i^\dagger\psi_l-\delta_{il}\psi_k^\dagger\psi_j
$$

with the corresponding spatial delta functions for fields. The quartic terms cancel after fermion reordering. Integrating proves the displayed algebra for well-defined global [Noether charges](quantum-field-theory.md#noether-charge), with [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) and a regulator that preserves the nonanomalous internal symmetry. Orthogonal [chiral projectors](relativistic-quantum-field.md#chiral-projector) make the left/right mixed commutators zero. This reduces current-charge closure to a finite matrix calculation.

###### Triplet charged-current closure on electromagnetic charge

↑ **Parent:** [Fermionic bilinear charge algebra](#fermionic-bilinear-charge-algebra)

For normalized triplets $(E^+,n,e)_L$ and $(E^+,N,e)_R$, let the raising matrix have ones in entries $(1,2)$ and $(2,3)$. Its commutator with its adjoint is $\operatorname{diag}(1,0,-1)$. Neutral mixing in $n=c_\alpha\nu+s_\alpha N$ leaves this result unchanged because $c_\alpha^2+s_\alpha^2=1$. With current normalization using $1\mp\gamma^5=2P_{L,R}$, [fermionic bilinear charge algebra](#fermionic-bilinear-charge-algebra) gives the displayed proportionality to the leptonic [electric charge](electromagnetism.md#electric-charge) $Q_\ell=e\int:(E^{+\dagger}E^+-e^\dagger e):$. Other current normalizations change the numerical prefactor, not closure. Equal-time algebra does not itself imply conservation of a fermionic weak charge in a symmetry-broken theory.

##### Equal-time canonical anticommutator of a Dirac field

↑ **Parent:** [Canonical anticommutation relations](#canonical-anticommutation-relations)

For mode normalization $1/\sqrt{2E_{\mathbf p}}$, particle and antiparticle operators satisfy $\{a_{\mathbf p}^s,a_{\mathbf q}^{r\dagger}\}=\{b_{\mathbf p}^s,b_{\mathbf q}^{r\dagger}\}=(2\pi)^3\delta^{sr}\delta^3(\mathbf p-\mathbf q)$. The [Dirac spinor](relativistic-quantum-field.md#dirac-spinor) completeness relations imply $\sum_s[u_s(\mathbf p)u_s^\dagger(\mathbf p)+v_s(-\mathbf p)v_s^\dagger(-\mathbf p)]=2E_{\mathbf p}I$. Inserting this into the [mode expansion of a Dirac field](relativistic-quantum-field.md#mode-expansion-of-a-dirac-field) gives the displayed local anticommutator. The reversed momentum in the antiparticle completeness term is essential.

#### Fermion number operator

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

The fermion number operator counts occupied fermionic modes. Its parity $(-1)^F$ is positive on even exterior degree and negative on odd exterior degree.

##### Supertrace

↑ **Parent:** [Fermion number operator](#fermion-number-operator)

A supertrace is the trace weighted by fermion parity. Supersymmetry makes paired positive-energy states cancel in a supertrace.

###### Equivariant supertrace

↑ **Parent:** [Supertrace](#supertrace)

An equivariant supertrace inserts a symmetry $f$ as well as fermion parity, $\operatorname{Tr}((-1)^FfA)$. In a path integral, $f$ produces boundary conditions twisted by its action.

### Fermionic path integral

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)

A fermionic path integral integrates Grassmann-valued histories. Its Gaussian integral is a determinant, in contrast with the inverse determinant produced by a bosonic Gaussian integral.

#### Berezin integral

↑ **Parent:** [Fermionic path integral](#fermionic-path-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Berezin_integral)

The Berezin integral is differentiation with respect to a Grassmann variable: $\int d\theta\,1=0$ and $\int d\theta\,\theta=1$. A finite-dimensional fermionic Gaussian integral gives a determinant or Pfaffian.

##### Grassmann change-of-variables formula

↑ **Parent:** [Berezin integral](#berezin-integral)

For independent [Grassmann variables](linear-algebra.md#grassmann-variable) and an invertible ordinary matrix $S$, the linear change $\eta=S\xi$ transforms the [Berezin integral](#berezin-integral) measure by the inverse [Jacobian determinant](calculus.md#jacobian-determinant). Indeed, the highest-degree monomial transforms by $\det S$, and coefficient extraction must undo that factor. For paired variables $\eta=S\xi$ and $\bar\eta=\bar\xi S^{-1}$ the two factors cancel. The order of odd variables and differentials fixes the overall sign and must be kept consistent.

#### Short-time limit of a supersymmetric path integral

↑ **Parent:** [Fermionic path integral](#fermionic-path-integral)

The short-time limit rescales a Euclidean time circle toward zero size. Supersymmetry cancels paired nonzero-mode determinants, leaving an integral over constant or symmetry-fixed zero modes.

### Twisted de Rham differential

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)

For a real function $h$, the twisted de Rham differential is $d_h=d+dh\wedge=e^{-h}de^h$. Its adjoint and $d_h$ define a supersymmetric Hamiltonian, and its square-integrable cohomology describes zero-energy states.

### Partner Hamiltonians

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partner_Hamiltonians)

Partner Hamiltonians reverse the order of two first-order factors and share corresponding positive-energy states.

<h3 id="poschl-teller-potential">Pöschl-Teller potential</h3>

↑ **Parent:** [Supersymmetric quantum mechanics](#supersymmetric-quantum-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pöschl–Teller_potential)

A Pöschl-Teller potential is a solvable one-dimensional potential built from $\operatorname{sech}^2 x$. The attractive member

$$
V(x)=-n(n+1)\alpha^2\operatorname{sech}^2(\alpha x)
$$

is reflectionless when $n$ is a positive integer.

#### Supersymmetric factorization of the one-soliton potential

↑ **Parent:** [Pöschl-Teller potential](#poschl-teller-potential)

Let

$$
A=\frac{d}{dx}+\chi\tanh(\chi x),
\qquad
A^\dagger=-\frac{d}{dx}+\chi\tanh(\chi x).
$$

Then

$$
A^\dagger A=-\frac{d^2}{dx^2}+\chi^2-2\chi^2\operatorname{sech}^2(\chi x),
\qquad
AA^\dagger=-\frac{d^2}{dx^2}+\chi^2.
$$

Thus the one-soliton Schrodinger operator is paired with the free Schrodinger operator. Its normalizable state annihilated by $A$ is proportional to $\operatorname{sech}(\chi x)$.

## Reflectionless potential

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflectionless_potential)

A reflectionless potential transmits every scattering state with zero reflected probability.

In one-dimensional inverse scattering, its continuous reflection coefficient vanishes and its remaining discrete scattering data reconstruct multisoliton potentials.

## Position operator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Position_operator)

In position representation, the position operator multiplies a wavefunction by its coordinate.

### Position eigenstate

↑ **Parent:** [Position operator](#position-operator)

A generalized eigenstate of the [position operator](#position-operator) is labeled by its position eigenvalue. In a continuous [position](classical-mechanics.md#position) coordinate the normalization is distributional: $\langle q|q'\rangle=\delta(q-q')$ and $\int dq\,|q\rangle\langle q|=1$. Individual position eigenstates are not normalizable Hilbert-space vectors. The [Dirac delta distribution](distribution-theory.md#dirac-delta-function) normalization makes $\langle q_f|U|q_i\rangle$ the integral kernel of a [time-evolution operator](#time-evolution-operator), such as the [free-particle propagator](#free-particle-propagator).

## Momentum operator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Momentum_operator)

In position representation, momentum is minus i hbar times spatial differentiation.

### Spatial translation operator

↑ **Parent:** [Momentum operator](#momentum-operator)

The spatial translation operator is the unitary generated by the [momentum operator](#momentum-operator). With the convention $U(\mathbf y)=e^{-i\mathbf P\cdot\mathbf y}$, a momentum eigenstate of eigenvalue $\mathbf p$ acquires the phase $e^{-i\mathbf p\cdot\mathbf y}$, while $U(\mathbf y)\phi(\mathbf x)U(\mathbf y)^{-1}=\phi(\mathbf x+\mathbf y)$.

### Position representation of the momentum operator

↑ **Parent:** [Momentum operator](#momentum-operator)

In one dimension the momentum operator acts on a position-space wavefunction as $p=-i\hbar\partial_x$, and $p^2=-\hbar^2\partial_x^2$.

### Canonical commutation relation

↑ **Parent:** [Momentum operator](#momentum-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_commutation_relation)

In position representation, $x$ acts by multiplication and $p_x=-i\hbar\partial_x$, so

$$
[x,p_x]=i\hbar I.
$$

#### Weyl relations

↑ **Parent:** [Canonical commutation relation](#canonical-commutation-relation)

These bounded-unitary relations encode a pair of [canonical commutation relations](#canonical-commutation-relation) without multiplying unbounded position and momentum operators. In a fixed convention on $L^2(\mathbb R)$, $W(x,y)f(t)=e^{ixy+2iyt}f(t+x)$ and $a\wedge b=x_1y_2-y_1x_2$. Strong continuity is part of a regular Weyl representation. Different nonzero choices of the central normalization rescale the canonical coordinates.

##### Stone-von Neumann theorem

↑ **Parent:** [Weyl relations](#weyl-relations)

Every irreducible strongly continuous representation of the [Weyl relations](#weyl-relations) with fixed nonzero central character is unitarily equivalent to the translation-modulation representation on $L^2(\mathbb R)$. The [Gaussian projection in a Weyl representation](#gaussian-projection-in-a-weyl-representation) supplies a cyclic vector whose Weyl-orbit inner products agree with those of a Gaussian in the standard representation. Matching those orbit vectors gives the unitary intertwiner, with no appeal to a classification assertion in place of the proof.

##### Gaussian projection in a Weyl representation

↑ **Parent:** [Weyl relations](#weyl-relations)

The integrated Gaussian in any nonzero regular representation of the [Weyl relations](#weyl-relations) is an orthogonal projection and obeys $PW(a)P=e^{-|a|^2/2}P$. Gaussian integration with the Weyl phase proves both identities. It cannot be zero: conjugating it by all Weyl operators would otherwise make the Fourier transform of every Gaussian-weighted matrix coefficient vanish, including its nonzero value at the identity. In an irreducible representation its range has dimension one, and the orbit of a unit vector there gives a dense cyclic space with universal Gaussian inner products.

## Ehrenfest theorem

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ehrenfest_theorem)

Ehrenfest’s theorem makes expectation values obey Hamiltonian commutator equations analogous to classical motion.

For a possibly time-dependent observable $O$,

$$
\frac d{dt}\langle O\rangle
=\frac1{i\hbar}\langle[O,H]\rangle
+\left\langle\frac{\partial O}{\partial t}\right\rangle.
$$

### Proof of Ehrenfest theorem from the Schrodinger equation

↑ **Parent:** [Ehrenfest theorem](#ehrenfest-theorem)

Differentiating $\langle\psi|O|\psi\rangle$ and using $i\hbar|\dot\psi\rangle=H|\psi\rangle$ and its adjoint gives

$$
\frac d{dt}\langle O\rangle
=\frac i\hbar\langle[H,O]\rangle
+\left\langle\frac{\partial O}{\partial t}\right\rangle.
$$

### Classical equations from Ehrenfest theorem

↑ **Parent:** [Ehrenfest theorem](#ehrenfest-theorem)

For $H=p^2/(2m)+U(x)$, the [canonical commutation relation](#canonical-commutation-relation) gives

$$
m\frac d{dt}\langle x\rangle=\langle p\rangle,
\qquad
\frac d{dt}\langle p\rangle=-\langle U'(x)\rangle,
\qquad
\frac d{dt}\langle H\rangle=0.
$$

These are the expectation-value analogues of [Newton's second law](classical-mechanics.md#newton-s-second-law) and conservation of energy.

### Correspondence principle

↑ **Parent:** [Ehrenfest theorem](#ehrenfest-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Correspondence_principle)

The correspondence principle states that quantum predictions approach classical mechanics in the appropriate large-scale or semiclassical regime.

## Angular momentum operator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Angular_momentum_operator)

### Axially symmetric quadratic orbital eigenfunction

↑ **Parent:** [Angular momentum operator](#angular-momentum-operator)

Each [orbital angular momentum](#orbital-angular-momentum) operator annihilates a radial factor and $r^2$. Direct differentiation gives $L^2x_3^2=\hbar^2(6x_3^2-2r^2)$ and $L_3x_3^2=0$. Hence the displayed trace-free quadratic polynomial, times any admissible radial factor, has orbital labels $l=2,m=0$. Its angular dependence is proportional to the [spherical harmonic](analysis.md#spherical-harmonic) $Y_{20}$; subtracting $r^2/3$ removes the rotational scalar part.

### Angular momentum lowering operator

↑ **Parent:** [Angular momentum operator](#angular-momentum-operator)

The operator $J_-=J_x-iJ_y$ acts by $J_-|j,m\rangle=\hbar\sqrt{(j+m)(j-m+1)}|j,m-1\rangle$. It generates lower magnetic states and determines [Clebsch-Gordan coefficients](representation-theory.md#clebsch-gordan-coefficients).

#### Normalized highest-weight lowering formula

↑ **Parent:** [Angular momentum lowering operator](#angular-momentum-lowering-operator)

In an [irreducible spin representation](#irreducible-spin-representation), the [angular momentum lowering operator](#angular-momentum-lowering-operator) has squared [norm](functional-analysis.md#norm) factor $(I+m)(I-m+1)$. Multiplying these factors from the [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) gives the factorial normalization displayed above. All factorial arguments are integers even when $I$ is half-integral. This produces a consistent positive-coefficient phase convention for all weight states and fixes signs in subsequent [isospin rotations](standard-model.md#isorotation).

### Angular momentum eigenstate

↑ **Parent:** [Angular momentum operator](#angular-momentum-operator)

A joint eigenstate $|j,m\rangle$ of $J^2$ and $J_z$, with eigenvalues $\hbar^2j(j+1)$ and $\hbar m$. Its allowed labels satisfy $j\in\{0,1/2,1,\ldots\}$ and $m=-j,-j+1,\ldots,j$.

### Angular momentum commutation relations

↑ **Parent:** [Angular momentum operator](#angular-momentum-operator)

Every angular momentum operator satisfies

$$
[J_i,J_j]=i\hbar\varepsilon_{ijk}J_k,
\qquad
[J^2,J_i]=0.
$$

### Addition of angular momentum

↑ **Parent:** [Angular momentum operator](#angular-momentum-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Addition_of_angular_momentum)

For two subsystems, the total operator is $\mathbf J=\mathbf J_1\otimes I+I\otimes\mathbf J_2$, and $J_\pm=J_{1\pm}+J_{2\pm}$. The coupled basis diagonalizes $\mathbf J^2$ and $J_z$.

#### Total angular momentum operator

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

For a composite quantum system, the total angular momentum operator is the sum of the constituent angular momenta, with each summand acting on its own tensor factor. Its simultaneous eigenstates with $J_z$ organize the state space into [total-spin sectors](#total-spin-sector).

#### Total-spin sector

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

A total-spin-$J$ sector is an irreducible subspace on which $\mathbf J^2$ has eigenvalue $J(J+1)\hbar^2$. For two spin-one particles, [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition) gives sectors $J=0,1,2$ of dimensions one, three, and five.

##### Three spin-one angular-momentum decomposition

↑ **Parent:** [Total-spin sector](#total-spin-sector)

Coupling three distinguishable spin-one systems gives

$$
1\otimes1\otimes1
=0\oplus3(1)\oplus2(2)\oplus3,
$$

where the labels denote total spin and coefficients denote multiplicities. The dimensions are respectively $1$, $3\cdot3$, $2\cdot5$, and $7$, summing to $27$.

###### Symmetric three-spin-one subspace

↑ **Parent:** [Three spin-one angular-momentum decomposition](#three-spin-one-angular-momentum-decomposition)

The completely symmetric subspace of three spin-one systems has dimension

$$
\binom{3+3-1}{3}=10
$$

and decomposes into one total-spin-$3$ multiplet and one total-spin-$1$ multiplet:

$$
\operatorname{Sym}^3(1)=3\oplus1.
$$

The highest-weight product state generates the seven-dimensional spin-$3$ multiplet; its three-dimensional invariant complement is spin $1$.

##### Spin-one Cartesian basis

↑ **Parent:** [Total-spin sector](#total-spin-sector)

The spin-one Cartesian basis $|x\rangle,|y\rangle,|z\rangle$ transforms as a three-dimensional vector under rotations. In its two-site tensor square, the scalar, antisymmetric, and symmetric traceless subspaces are respectively the total-spin $0$, $1$, and $2$ sectors.

##### Spin-dot-product eigenvalue

↑ **Parent:** [Total-spin sector](#total-spin-sector)

For two spins of magnitude $s$, $\mathbf S_1\mathbin\cdot\mathbf S_2=\tfrac12(\mathbf J^2-\mathbf S_1^2-\mathbf S_2^2)$. For two spin-one particles its eigenvalues in total-spin sectors $J=0,1,2$ are $-2,-1,1$ in units of $\hbar^2$.

#### Clebsch-Gordan decomposition

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

The tensor product of spin-$j_1$ and spin-$j_2$ irreducible representations decomposes into one copy of each spin

$$
j=|j_1-j_2|,|j_1-j_2|+1,\ldots,j_1+j_2.
$$

The change-of-basis entries between uncoupled and coupled states are Clebsch--Gordan coefficients.

##### Lowest-weight coupling of two angular momenta

↑ **Parent:** [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition)

Put $s=j_1+j_2$, with both $j_i>0$. At magnetic quantum number $-s+1$, let $|a\rangle$ raise only the first factor of the lowest product state and $|b\rangle$ raise only the second. Applying total $J_+$ to the lowest product gives the normalized $J=s$ combination $\sqrt{j_1/s}|a\rangle+\sqrt{j_2/s}|b\rangle$. Its orthogonal combination is annihilated by total $J_-$ and therefore has $J=s-1$. This obtains a useful [Clebsch-Gordan coefficients](representation-theory.md#clebsch-gordan-coefficients) without a table.

#### Highest-weight states in angular momentum addition

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

With $J=j_1+j_2$, the maximal state is the product $|J,J\rangle=|j_1,j_1\rangle|j_2,j_2\rangle$. Lowering it once gives

$$
|J,J-1\rangle=
\sqrt{\frac{j_1}{J}}|j_1,j_1-1\rangle|j_2,j_2\rangle
+\sqrt{\frac{j_2}{J}}|j_1,j_1\rangle|j_2,j_2-1\rangle.
$$

The orthogonal combination is the highest-weight state $|J-1,J-1\rangle$.

#### Singlet state

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singlet_state)

Two equal spins $j$ have the unique total-spin-zero state

$$
|0,0\rangle=\frac1{\sqrt{2j+1}}
\sum_{m=-j}^j(-1)^{j-m}|j,m\rangle|j,-m\rangle.
$$

It is invariant under joint rotations.

A [singlet state](#singlet-state) is the one-dimensional rotation representation; this construction supplies the angular-momentum-zero case for two equal spins.

##### Spin-one-half singlet state

↑ **Parent:** [Singlet state](#singlet-state)

For two spin-one-half particles, the singlet is

$$
|0,0\rangle=\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2}.
$$

Every component of the total spin annihilates it, and $\mathbf S^2$ has eigenvalue zero.

#### Spin-one-half triplet state

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

The symmetric two-particle states

$$
|\uparrow\uparrow\rangle,
\qquad
\frac{|\uparrow\downarrow\rangle+|\downarrow\uparrow\rangle}{\sqrt2},
\qquad
|\downarrow\downarrow\rangle
$$

form the spin-one triplet. On this subspace, $\mathbf S^2$ has eigenvalue $1(1+1)\hbar^2=2\hbar^2$.

### Spin

↑ **Parent:** [Angular momentum operator](#angular-momentum-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_(physics))

Spin operators satisfy $[S_i,S_j]=i\hbar\varepsilon_{ijk}S_k$ and are Hermitian traceless generators of rotations in finite-dimensional irreducible representations.

<h4 id="jordan-wigner-transformation">Jordan–Wigner transformation</h4>

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan–Wigner_transformation)

The Jordan–Wigner transformation represents a one-dimensional [spin one-half](#spin-one-half) chain by fermions with a parity string preceding each site. With $P_n=\prod_{m<n}(1-2n_m)$, one has $S_n^+=P_nc_n$ and $S_n^z=1/2-n_n$. The string converts the off-site [canonical anticommutation relations](#canonical-anticommutation-relations) into commuting spin operators. Adjacent exchange terms become quadratic fermion expressions, while a periodic end bond depends on global [fermion parity](topological-quantum-matter.md#fermion-parity).

#### Spin one-half

↑ **Parent:** [Spin](#spin)

In units $\hbar=1$, spin one-half is the two-dimensional irreducible [spin angular momentum](#spin) representation with components $S_i=\sigma_i/2$. The [Pauli matrices](algebra.md#pauli-matrices) give [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm1/2$ along every unit axis. The normalized $x$-axis states are $(|\uparrow_z\rangle\pm|\downarrow_z\rangle)/\sqrt2$.

##### Spin one-half along an axis

↑ **Parent:** [Spin one-half](#spin-one-half)

For $\mathbf n=(\sin\theta,0,\cos\theta)$, the normalized eigenstates of $\mathbf n\cdot\mathbf S$ are

$$
|\uparrow_\theta\rangle
=\cos\frac\theta2|\uparrow\rangle
+\sin\frac\theta2|\downarrow\rangle,
\qquad
|\downarrow_\theta\rangle
=-\sin\frac\theta2|\uparrow\rangle
+\cos\frac\theta2|\downarrow\rangle,
$$

with eigenvalues $+\hbar/2$ and $-\hbar/2$.

<h4 id="holstein-primakoff-transformation">Holstein–Primakoff transformation</h4>

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holstein–Primakoff_transformation)

The Holstein–Primakoff transformation represents a spin-$S$ [operator algebra](functional-analysis.md#operator-algebra) with a bosonic [creation operator](#creation-operator) and [annihilation operator](#annihilation-operator):

$$
S^+=\sqrt{2S}\sqrt{1-\frac{a^\dagger a}{2S}}\,a,\qquad S^-=\sqrt{2S}\,a^\dagger\sqrt{1-\frac{a^\dagger a}{2S}},\qquad S^z=S-a^\dagger a.
$$

The order of the square root and oscillator operator matters. On the physical [Fock states](quantum-field-theory.md#fock-state) $|n\rangle$, $0\le n\le2S$, the raising and lowering matrix elements are $\sqrt{n(2S-n+1)}$ and $\sqrt{(n+1)(2S-n)}$. Their squared difference gives $[S^+,S^-]|n\rangle=2(S-n)|n\rangle$, proving the [spin commutation relations](#spin-commutation-relations). Expanding the square root yields the [linear spin-wave approximation](critical-phenomenon.md#linear-spin-wave-approximation) and its interaction corrections.

<h5 id="holstein-primakoff-occupation-constraint">Holstein–Primakoff occupation constraint</h5>

↑ **Parent:** [Holstein–Primakoff transformation](#holstein-primakoff-transformation)

A spin-$S$ [Hilbert space](hilbert-space.md) has dimension $2S+1$. Its [Holstein–Primakoff transformation](#holstein-primakoff-transformation) therefore uses only bosonic [occupation numbers](quantum-field-theory.md#occupation-number) $0,1,\ldots,2S$. The square root annihilates the upper endpoint. A truncated [linear spin-wave approximation](critical-phenomenon.md#linear-spin-wave-approximation) formally enlarges this space; it is self-consistent only when boson depletion is small compared with $S$.

#### Spin commutation relations

↑ **Parent:** [Spin](#spin)

The components of [spin angular momentum](#spin) satisfy $[S_i,S_j]=i\hbar\epsilon_{ijk}S_k$. In units $\hbar=1$, the [spin ladder operators](#spin-ladder-operator) obey $[S^+,S^-]=2S^z$ and $[S^z,S^\pm]=\pm S^\pm$.

#### Irreducible spin representation

↑ **Parent:** [Spin](#spin)

The spin-$s$ irreducible representation has dimension $2s+1$, with basis $|s,m\rangle$ for $m=-s,-s+1,\ldots,s$ and Casimir eigenvalue $\hbar^2s(s+1)$.

##### Wigner D-matrix

↑ **Parent:** [Irreducible spin representation](#irreducible-spin-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wigner_D-matrix)

For active rotations with $U=e^{-i\phi J_3}e^{-i\theta J_2}e^{-i\psi J_3}$, the [irreducible spin representation](#irreducible-spin-representation) [matrix](vector-space.md#matrix) is $D^{(j)}_{mm'}=e^{-im\phi}d^{(j)}_{mm'}(\theta)e^{-im'\psi}$, where $d^{(j)}_{mm'}=\langle j,m|e^{-i\theta J_2}|j,m'\rangle$. Its spin-one-half middle [matrix](vector-space.md#matrix) is $\begin{pmatrix}\cos(\theta/2)&-\sin(\theta/2)\\\sin(\theta/2)&\cos(\theta/2)\end{pmatrix}$. A $2\pi$ rotation acts by $(-1)^{2j}$; only integer-spin representations descend to the [special orthogonal group](linear-algebra.md#special-orthogonal-group) in three [dimensions](vector-space.md#dimension-vector-space).

##### Unitary highest-weight termination

↑ **Parent:** [Irreducible spin representation](#irreducible-spin-representation)

For Hermitian $J_3$ and adjoint [angular momentum ladder operators](#angular-momentum-ladder-operator) $J_+^\dagger=J_-$ on a positive-definite inner-product space, a [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) of weight $j$ obeys $J_+|j,j\rangle=0$. The commutation relations give $J_+(J_-)^\ell|j,j\rangle=\ell(2j-\ell+1)(J_-)^{\ell-1}|j,j\rangle$. Taking [inner products](linear-algebra.md#inner-product) forces $2j$ to be a nonnegative integer: otherwise the first negative factor would give a negative squared norm. The norm first vanishes at $\ell=2j+1$, so the generated [unitary representation](representation-theory.md#unitary-representation) has [dimension](vector-space.md#dimension-vector-space) $2j+1$. Without positivity an abstract highest-weight module can remain infinite-dimensional even at an integral [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation).

##### Spin-one half-turn matrix

↑ **Parent:** [Irreducible spin representation](#irreducible-spin-representation)

In the ordered spin-one basis $(m=1,0,-1)$, the second [angular momentum operator](#angular-momentum-operator) satisfies $J_2^3=J_2$. Therefore its [matrix exponential](linear-operator-theory.md#matrix-exponential) reduces to $I-i\sin\theta J_2+(\cos\theta-1)J_2^2$. A half-turn exchanges the two outer weights and negates the middle weight. Applied to the [pion](standard-model.md#pion) [isospin](standard-model.md#isospin) triplet, this fixes the rotation factor in [G parity](standard-model.md#g-parity).

#### Spin ladder operator

↑ **Parent:** [Spin](#spin)

The operators $S_\pm=S_x\pm iS_y$ satisfy

$$
S_\pm|s,m\rangle
=\hbar\sqrt{s(s+1)-m(m\pm1)}|s,m\pm1\rangle.
$$

##### Spin raising operator

↑ **Parent:** [Spin ladder operator](#spin-ladder-operator)

The spin raising operator $S_+=S_x+iS_y$ increases the [magnetic quantum number](#magnetic-quantum-number) by one and annihilates the maximal-weight state.

##### Spin lowering operator

↑ **Parent:** [Spin ladder operator](#spin-ladder-operator)

The spin lowering operator $S_-=S_x-iS_y$ decreases the [magnetic quantum number](#magnetic-quantum-number) by one and annihilates the minimal-weight state.

#### Spin-three-halves matrices

↑ **Parent:** [Spin](#spin)

In descending $S_z$ order, the spin-$3/2$ raising operator has superdiagonal entries $\hbar\sqrt3,2\hbar,\hbar\sqrt3$; $S_x$ and $S_y$ are its Hermitian real and imaginary combinations.

#### Spin coherent state

↑ **Parent:** [Spin](#spin)

A spin coherent state is obtained by rotating the maximal-weight state $|s,s\rangle$ so that it is an eigenstate of spin along a chosen direction with eigenvalue $s\hbar$.

##### Spin coherent-state path integral

↑ **Parent:** [Spin coherent state](#spin-coherent-state)

A spin coherent-state path integral inserts group-averaged resolutions of the identity between short time steps. Its kinetic term is the [Spin coherent-state Berry phase](statistical-physics.md#spin-coherent-state-berry-phase), equal to $S$ times the oriented solid angle swept on the sphere.

##### Equatorial spin-three-halves coherent state

↑ **Parent:** [Spin coherent state](#spin-coherent-state)

At azimuth $\varphi$, the normalized spin-$3/2$ coherent-state components are proportional to $1,\sqrt3e^{i\varphi},\sqrt3e^{2i\varphi},e^{3i\varphi}$.

#### Larmor precession

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Larmor_precession)

[Larmor precession](#larmor-precession) is the precession of a magnetic moment about an applied magnetic field. For a spin with gyromagnetic ratio $\gamma$ and Hamiltonian $H=-\gamma\mathbf B\cdot\mathbf S$, its expectation obeys $d\langle\mathbf S
angle/dt=\gamma\langle\mathbf S
angle	imes\mathbf B$. A spin coherent state retains its coherent form during this rotation.

##### Larmor precession of a spin coherent state

↑ **Parent:** [Larmor precession](#larmor-precession)

Under $H=-\gamma BS_z$, a coherent spin direction precesses around the $z$-axis with angular velocity $-\gamma B$.

###### Time evolution under a spin-Z Hamiltonian

↑ **Parent:** [Larmor precession of a spin coherent state](#larmor-precession-of-a-spin-coherent-state)

The propagator $e^{i\gamma BtS_z/\hbar}$ multiplies each magnetic component $|s,m\rangle$ by $e^{im\gamma Bt}$.

#### Heisenberg model

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heisenberg_model)

The Heisenberg model couples neighboring or more general pairs of spins through $\boldsymbol\sigma_i\mathbin{\cdot}\boldsymbol\sigma_j$. For all-to-all equal coupling, the Hamiltonian can be written in terms of the square of the total spin.

##### Magnetization sectors of a spin chain

↑ **Parent:** [Heisenberg model](#heisenberg-model)

With $S=\sum_{n=1}^NZ_n$, a computational basis vector containing $k$ excitations has eigenvalue $N-2k$. There are $N+1$ distinct eigenspaces, of dimensions $\binom Nk$. Any Hamiltonian commuting with $S$ preserves each sector and their population weights. In particular, a state supported in one sector cannot be transferred to a different sector by such controls.

##### Excitation-number conservation in XXZ spin chains

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For $H=\sum_{m<n}c_{mn}(X_mX_n+Y_mY_n)+\gamma_{mn}Z_mZ_n$, Pauli [commutators](lie-algebra.md#commutator) give cancellation between the $XX$ and $YY$ terms in $[H,Z_m+Z_n]$, while each $ZZ$ term commutes individually. Hence total spin magnetization is conserved. Local $Z_k$ controls preserve the same law, so dynamics split into fixed-excitation sectors even when a particular sector is controllable.

##### Single-excitation subspace

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For a network of $N$ spin-one-half sites with $Z|0\rangle=|0\rangle$ and $Z|1\rangle=-|1\rangle$, the single-excitation subspace has exactly one spin in state $|1\rangle$ and dimension $N$. Excitation-conserving exchange interactions preserve it. Its restricted Hamiltonian is a hopping matrix whose entries connect the corresponding sites. Controllability within this subspace need not imply controllability on the full $2^N$-dimensional space.

###### XY exchange interaction

↑ **Parent:** [Single-excitation subspace](#single-excitation-subspace)

The isotropic XY exchange interaction between two [qubits](#qubit) is $E=(X\otimes X+Y\otimes Y)/2$. Its action is

$$
E|00\rangle=E|11\rangle=0,\qquad E|01\rangle=|10\rangle,\qquad E|10\rangle=|01\rangle.
$$

Indeed, $X|0\rangle=|1\rangle$, $X|1\rangle=|0\rangle$, $Y|0\rangle=i|1\rangle$, and $Y|1\rangle=-i|0\rangle$. The two terms cancel on equal bits and add on unequal bits. Thus a network [Hamiltonian operator](#hamiltonian-quantum-mechanics) $H=\sum_{a,b}K_{ab}E_{ab}$ preserves excitation number; in the [single-excitation subspace](#single-excitation-subspace), it is the weighted adjacency [matrix](vector-space.md#matrix), moving an excitation from $a$ to $b$ with hopping coefficient $K_{ab}$.

###### Symmetric-arm reduction of an exchange Hamiltonian

↑ **Parent:** [XY exchange interaction](#xy-exchange-interaction)

Consider $q$ identical length-$n$ arms joined to one hub, with [XY exchange interactions](#xy-exchange-interaction) of strength $J_0/\sqrt q$ from the hub to each first site and strength $J_k$ between sites $k,k+1$ on each arm. Let $|s_0\rangle$ be the hub excitation and $|s_k\rangle=q^{-1/2}\sum_{a=1}^q|a,k\rangle$. This [orthonormal](linear-algebra.md#orthonormal-set) symmetric [single-excitation subspace](#single-excitation-subspace) is invariant, and its restricted [Hamiltonian operator](#hamiltonian-quantum-mechanics) is

$$
H|s_0\rangle=J_0|s_1\rangle,\qquad H|s_k\rangle=J_{k-1}|s_{k-1}\rangle+J_k|s_{k+1}\rangle,
$$

with endpoint terms omitted. At the first link the $q$ hub contributions add to $J_0$; all other links act identically on the arms. Thus the [linear isometry](hilbert-space.md#linear-isometry-of-hilbert-spaces) $F|k\rangle=|s_k\rangle$ intertwines $H$ with the path [Hamiltonian operator](#hamiltonian-quantum-mechanics) $H_T=\sum_{k=0}^{n-1}J_k(|k\rangle\langle k+1|+|k+1\rangle\langle k|)$: $HF=FH_T$. Expanding the [matrix exponential](linear-operator-theory.md#matrix-exponential) gives $e^{-iHt}F=Fe^{-iH_Tt}$. [Perfect quantum state transfer](#perfect-quantum-state-transfer) from zero to $n$ on the path therefore produces an equal excitation superposition at the $q$ arm tips. Since all other [qubits](#qubit) are zero, the tip state is a pure [W state](#w-state), up to the transfer's common phase.

###### Endpoint control of an XX spin chain

↑ **Parent:** [Single-excitation subspace](#single-excitation-subspace)

In the [single-excitation subspace](#single-excitation-subspace), take a connected real nearest-neighbor hopping matrix $A$ with every coupling nonzero and endpoint control $B=\operatorname{diag}(-1,1,\ldots,1)$. Endpoint commutators isolate the first transition, then propagate along the chain to generate both off-diagonal skew-Hermitian directions and adjacent diagonal differences. These generate $\mathfrak{su}(N)$. For $N\ge3$, $\operatorname{Tr}B=N-2\ne0$ supplies the central direction, giving $\mathfrak u(N)$. For $N=2$ the algebra is $\mathfrak{su}(2)$, which still gives full state controllability but omits an arbitrary global phase. A broken coupling separates an unreachable chain component.

##### Heisenberg antiferromagnet

↑ **Parent:** [Heisenberg model](#heisenberg-model)

A Heisenberg antiferromagnet has positive exchange coupling in $H=J\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j$, so neighboring spins energetically prefer antiparallel alignment.

###### Bipartite spin rotation

↑ **Parent:** [Heisenberg antiferromagnet](#heisenberg-antiferromagnet)

A [bipartite spin rotation](#bipartite-spin-rotation) rotates the [spin](#spin) on one sublattice by $\pi$, converting an alternating classical [Néel state](statistical-physics.md#neel-state) to an all-up reference state. Rotation about $x$ sends $S^z\mapsto-S^z$ and $S^\pm\mapsto S^\mp$ on that sublattice. For an isotropic nearest-neighbor [Heisenberg antiferromagnet](#heisenberg-antiferromagnet), a bond becomes $-S_i^zS_j^z+(S_i^+S_j^++S_i^-S_j^-)/2$. The transformation is unitary and preserves the [spin commutation relations](#spin-commutation-relations); it changes the reference frame, not the model's spectrum.

##### Heisenberg ferromagnet

↑ **Parent:** [Heisenberg model](#heisenberg-model)

A Heisenberg ferromagnet has negative exchange coupling in $H=J\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j$, so neighboring spins energetically prefer parallel alignment.

###### Ferromagnetic ground-state multiplet

↑ **Parent:** [Heisenberg ferromagnet](#heisenberg-ferromagnet)

A connected isotropic spin-$S$ ferromagnet with positive exchanges has a fully polarized [ground state](#ground-state) and a maximal-total-spin multiplet. For $N$ sites the total spin is $NS$, with $2NS+1$ magnetic states generated by total-spin lowering. Global rotations span the same degenerate space. Slowly varying reorientations produce gapless [ferromagnetic magnons](statistical-physics.md#ferromagnetic-magnon); finite-volume degeneracy must be distinguished from a thermodynamic statement about spontaneous order.

##### Two-spin Heisenberg Hamiltonian in an opposing longitudinal field

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For two spin-one-half particles,

$$
H=\alpha\mathbf S^{(1)}\mathbin\cdot\mathbf S^{(2)}
+B(S_z^{(1)}-S_z^{(2)})
$$

has two eigenvalues $\alpha\hbar^2/4$ and two further eigenvalues

$$
-\frac{\alpha\hbar^2}{4}
\pm\sqrt{B^2\hbar^2+\frac{\alpha^2\hbar^4}{4}}.
$$

For positive $\alpha$, the zero-field limit has a unique [spin-one-half singlet state](#spin-one-half-singlet-state) ground state and a triply degenerate [spin-one-half triplet state](#spin-one-half-triplet-state) excited level.

##### All-to-all Heisenberg model

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For $N$ spin-one-half systems and one term per unordered pair,

$$
\sum_{i<j}\boldsymbol\sigma_i\mathbin{\cdot}\boldsymbol\sigma_j
=2\mathbf S^2-\frac{3N}{2},
\qquad
\mathbf S=\frac12\sum_i\boldsymbol\sigma_i.
$$

Its minimum lies in the smallest available total-spin sector.

##### Infinite-coordination Heisenberg antiferromagnet

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For a bipartite spin-one-half Heisenberg antiferromagnet with coordination $z\to\infty$, the two-sublattice mean-field state becomes exact. Antiparallel pure Bloch vectors give bond energy $-J/4$ for the convention $J\mathbf S_i\cdot\mathbf S_j$.

## Infinite square well

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infinite_square_well)

### Energy form of a half-well sine state

↑ **Parent:** [Infinite square well](#infinite-square-well)

In the [infinite square well](#infinite-square-well) on $(-a,a)$, extend $\sqrt{2/a}\sin(\pi x/a)$ from $(0,a)$ by zero. It is normalized and continuous, but its [derivative](calculus.md#derivative) jumps at zero. Its energy [expectation value](#expectation-value) is the [quadratic form of a positive quantum Hamiltonian](#quadratic-form-of-a-positive-quantum-hamiltonian) $\hbar^2\int|\psi'|^2/(2m)$, giving the displayed value. It is not in the operator domain of the Dirichlet [Hamiltonian operator](#hamiltonian-quantum-mechanics): its distributional second [derivative](calculus.md#derivative) contains a [Dirac delta](distribution-theory.md#dirac-delta-function). Its sine-basis coefficients are $a_2=-1/\sqrt2$, all other even coefficients zero, and $a_{2p+1}=4\sqrt2(-1)^p/[\pi(4-(2p+1)^2)]$. These make $\sum_nE_n|a_n|^2$ finite but $\sum_nE_n^2|a_n|^2$ divergent, independently distinguishing the form domain from the operator domain.

### Ramp-state expansion in a symmetric infinite well

↑ **Parent:** [Infinite square well](#infinite-square-well)

In a well $-a<x<a$, the normalized state proportional to $x$ on $0<x<a$ and zero elsewhere has stationary-state coefficients

$$
c_n=-\frac{2\sqrt3(-1)^n}{n\pi}-\frac{4\sqrt3\sin(n\pi/2)}{n^2\pi^2}.
$$

They follow from the [orthonormal basis](linear-algebra.md#orthonormal-basis) inner products. Their squared magnitudes give energy-measurement probabilities by the [Born rule](#born-rule); splitting even and odd indices in the [Parseval identity](fourier-analysis.md#parseval-identity) gives convergent integer-coefficient series identities. The expansion is interpreted in the square-integrable state norm.

### Particle in a rectangular box

↑ **Parent:** [Infinite square well](#infinite-square-well)

Dirichlet separation in a rectangular box gives products of sine waves and energy proportional to $n_x^2/a^2+n_y^2/b^2+n_z^2/c^2$.

The [infinite square well](#infinite-square-well) supplies the one-dimensional factors of this rectangular-box construction.

## Degenerate energy levels

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degenerate_energy_levels)

An energy level is degenerate when its eigenspace has dimension greater than one.

## Orbital angular momentum

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Orbital angular momentum is $L=-i\hbar,x\times\nabla$; in particular $L_3=-i\hbar(x_1\partial_{x_2}-x_2\partial_{x_1})$.

### Highest-weight complex-coordinate orbital wavefunction

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

For a differentiable radial factor and integer $n\geq0$, the coordinate polynomial obeys $L_3\psi=n\hbar\psi$ and $L_+\psi=0$. The identity $L^2=L_-L_++L_3^2+\hbar L_3$ gives the displayed angular [eigenvalue](linear-operator-theory.md#eigenvalue). Lowering gives $L_-\psi=-2n\hbar z(x+iy)^{n-1}f(r)$, a nonzero [eigenfunction](linear-operator-theory.md#eigenfunction) with the same angular [eigenvalue](linear-operator-theory.md#eigenvalue) when $n>0$ and the original state is nonzero. At $n=0$ lowering gives the zero function, which is not an [eigenfunction](linear-operator-theory.md#eigenfunction). Negative powers satisfy local differential identities off the axis but are not regular angular states.

### Angular momentum of a homogeneous harmonic polynomial

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

For a homogeneous [harmonic polynomial](partial-differential-equation.md#harmonic-polynomial) $H_l$ of degree $l$ in three dimensions, the [Euler theorem for homogeneous functions](real-analysis.md#euler-theorem-for-homogeneous-functions) gives $DH_l=lH_l$, where $D=\mathbf x\cdot\nabla$. The [orbital angular momentum](#orbital-angular-momentum) identity $\hat L^2=-\hbar^2(r^2\Delta-D^2-D)$ therefore gives $\hat L^2H_l=l(l+1)\hbar^2H_l$. This constructs [angular momentum eigenstates](#angular-momentum-eigenstate) directly from polynomials.

### Angular momentum of a radial function times a linear polynomial

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

Orbital [angular momentum operators](#angular-momentum-operator) annihilate a radial multiplier $H(r)$. Their squared sum sends every degree-one homogeneous [polynomial](polynomial.md) to $2\hbar^2$ times that polynomial, so a nonzero normalizable state $H(r)(\mathbf a\cdot\mathbf x)$ has angular momentum quantum number $l=1$. With real $H$ and real coefficients, its third-component [expected value](probability-theory.md#expected-value) is zero by angular symmetry, though it need not be an eigenstate of that component.

### Magnetic quantum number

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_quantum_number)

The magnetic quantum number $m$ labels an eigenvalue of $L_z$: $L_z|\ell,m\rangle=m\hbar|\ell,m\rangle$, with $m=-\ell,-\ell+1,\ldots,\ell$.

### Rotation commutators for orbital angular momentum

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

For $L_i=\varepsilon_{ik\ell}X_kP_\ell$ and $[X_i,P_j]=i\hbar\delta_{ij}$,

$$
[L_i,X_j]=i\hbar\varepsilon_{ijk}X_k,
\qquad
[L_i,P_j]=i\hbar\varepsilon_{ijk}P_k.
$$

### Orbital angular momentum commutation relations

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

The canonical position-momentum commutators imply

$$
[L_i,L_j]=i\hbar\varepsilon_{ijk}L_k,
\qquad
[L^2,L_i]=0.
$$

### Angular momentum ladder operator

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

The operators $L_\pm=L_x\pm iL_y$ satisfy

$$
[L_z,L_\pm]=\pm\hbar L_\pm,
\qquad
[L^2,L_\pm]=0.
$$

They therefore change the [magnetic quantum number](#magnetic-quantum-number) $m$ by $\pm1$ while preserving the total angular-momentum quantum number $\ell$.

### Squared orbital angular momentum in position and momentum operators

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

Operator ordering gives

$$
L^2=X^2P^2-(X\cdot P)^2+i\hbar X\cdot P.
$$

#### Spherical Laplacian from orbital angular momentum

↑ **Parent:** [Squared orbital angular momentum in position and momentum operators](#squared-orbital-angular-momentum-in-position-and-momentum-operators)

In position representation,

$$
\boxed{L^2=-\hbar^2\nabla_{S^2}^2}.
$$

The radial derivatives cancel after substituting $P=-i\hbar\nabla$ into the Cartesian identity for $L^2$.

### Angular momentum ladder variable

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

The coordinate combinations $x_1\pm ix_2$ have $L_3$ eigenvalues $\pm\hbar$, so their powers carry [magnetic quantum numbers](#magnetic-quantum-number) $\pm m$.

#### Angular momentum of a complex-coordinate Gaussian state

↑ **Parent:** [Angular momentum ladder variable](#angular-momentum-ladder-variable)

If $\psi=z e^{-r^2/(2a^2)}$ in two dimensions, then $L_z\psi=\hbar\psi$ and $L_z\psi^*=-\hbar\psi^*$. Orthogonality therefore makes the angular-momentum expectation of $\alpha\psi+\beta\psi^*$ equal to $(|\alpha|^2-|\beta|^2)\hbar$ for normalized coefficients.

### Rotational invariance of a central-potential Hamiltonian

↑ **Parent:** [Orbital angular momentum](#orbital-angular-momentum)

For

$$
H=\frac{P^2}{2m}+U(|X|),
$$

both $P^2$ and $|X|^2$ are rotational scalars, so $[H,L_i]=0$. Consequently $H,L^2,L_3$ commute pairwise and can be simultaneously diagonalized.

#### Separation of a two-dimensional central-potential eigenstate

↑ **Parent:** [Rotational invariance of a central-potential Hamiltonian](#rotational-invariance-of-a-central-potential-hamiltonian)

An energy and [orbital angular momentum](#orbital-angular-momentum) [eigenstate](#eigenstate) for a real two-dimensional [central potential](classical-mechanics.md#central-potential) can be chosen with integer $k$ and real radial function $f$. Its radial equation is

$$
-\frac{\hbar^2}{2m}\left(f''+r^{-1}f'-k^2r^{-2}f\right)+Vf=Ef,\qquad \int_0^\infty r f^2\,dr=1.
$$

[Quantum degeneracy](#degenerate-energy-levels) permits other [stationary states](#stationary-state), including $f(r)\cos(k\phi)/\sqrt\pi$, which are not single angular exponentials. [Separation of variables](partial-differential-equation.md#separation-of-variables) supplies a basis rather than describing every superposition in a degenerate eigenspace.

## Quantum harmonic oscillator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_harmonic_oscillator)

In units with $\hbar=1$, a harmonic oscillator of angular frequency $\omega$ has

$$
H=\omega\left(N+\frac12\right),
\qquad N=A^\dagger A.
$$

### Stability of monomial ladder-operator perturbations

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)

The perturbation $\lambda\hbar\omega(a^r+(a^\dagger)^r)$ couples the oscillator vacuum only to $|r\rangle$ at first order. Its squared coupling is $(\hbar\omega)^2r!$ and the [energy](classical-mechanics.md#energy) denominator is $-r\hbar\omega$, giving the displayed formal second-order coefficient. For $r>2$ and nonzero real $\lambda$, coherent-state expectations contain $R^2+2\lambda R^r\cos r\theta$; choosing its phase negative proves the [Hamiltonian](classical-mechanics.md#hamiltonian) is unbounded below. The formal vacuum branch must therefore not be called an exact ground state. For $r=2$ boundedness requires $|\lambda|<1/2$, while the displaced $r=1$ oscillator is stable for every real strength.

### Harmonic oscillator transition kernel

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)

For [action](classical-mechanics.md#action) $\frac m2\int(\dot q^2-\omega^2q^2)dt$, the kernel is $\sqrt{m\omega/(2\pi i\sin\omega T)}\exp\{im\omega[(q_f^2+q_i^2)\cos\omega T-2q_fq_i]/(2\sin\omega T)\}$. The [Dirichlet oscillator determinant ratio](quantum-field-theory.md#dirichlet-oscillator-determinant-ratio) supplies its prefactor, while the classical boundary [action](classical-mechanics.md#action) supplies its exponent. The [Feynman i-epsilon prescription](quantum-field-theory.md#feynman-i-epsilon-prescription) specifies its continuation through caustics.

### Minimum-energy normalized oscillator mode

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)

For a [quantum harmonic oscillator](#quantum-harmonic-oscillator) with $\omega>0$, a complex mode satisfying the [Wronskian normalization](quantum-field-theory.md#wronskian-normalization) $q\dot q^*-\dot q q^*=i$ can be written $q=re^{is}$ with $\dot s=-1/(2r^2)$. Its [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy) is $\dot r^2/2+1/(8r^2)+\omega^2r^2/2$. This is at least $\omega/2$, with equality exactly when $\dot r=0$ and $r^2=1/(2\omega)$. The same argument fixes the subhorizon positive-frequency normalization in the [Bunch-Davies vacuum](cosmic-inflation.md#bunch-davies-vacuum) of a canonical cosmological mode.

### One-dimensional harmonic oscillator form domain

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)

This [Hilbert space](hilbert-space.md) has norm $\|u\|_X^2=\|u\|_2^2+\|u'\|_2^2+\|xu\|_2^2$. Completeness follows from completeness of [H1 space](sobolev-space.md#h1-space) and closedness of the [multiplication operator](vector-space.md#multiplication-operator) $u\mapsto xu$. Smooth cutoffs followed by convolution with a [mollifier](distribution-theory.md#mollifier) show that smooth compactly supported functions are dense. The space is the natural energy domain of the dimensionless [quantum harmonic oscillator](#quantum-harmonic-oscillator), whereas the operator domain additionally requires $u''$ and $x^2u$ to lie in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space).

#### Graph estimate for the harmonic oscillator

↑ **Parent:** [One-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain)

For $c>0$ and smooth compactly supported $u$, [integration by parts](calculus.md#integration-by-parts) gives

$$
\|-u''+(c+x^2)u\|_2^2
=\|u''\|_2^2+\|(c+x^2)u\|_2^2+2\int(c+x^2)|u'|^2\,dx-2\|u\|_2^2.
$$

Dropping the nonnegative weighted derivative term proves the displayed bound. For a weak resolvent solution in the [one-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain), apply the bound to $\chi_Ru$, where $\chi_R$ is a smooth cutoff. The cutoff error $-2\chi_R'u'-\chi_R''u$ is bounded in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) and tends to zero. The [Fatou lemma](measure-theory.md#fatou-s-lemma) then shows that $u''$ and $x^2u$ belong to [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), identifying the strong operator domain.

##### Resolvent of the shifted harmonic oscillator

↑ **Parent:** [Graph estimate for the harmonic oscillator](#graph-estimate-for-the-harmonic-oscillator)

For $Au=u''-(1+x^2)u$ on $D(A)=\{u\in H^2(\mathbb R):x^2u\in L^2\}$, the form $a_\lambda(u,v)=\int u'\overline{v'}+(1+\lambda+x^2)u\bar v$ is coercive on the [one-dimensional harmonic oscillator form domain](#one-dimensional-harmonic-oscillator-form-domain) when $\lambda>0$. The [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) gives a unique weak solution of $(\lambda-A)u=g$. The [graph estimate for the harmonic oscillator](#graph-estimate-for-the-harmonic-oscillator) puts it in $D(A)$, and $a_\lambda(u,u)\geq(1+\lambda)\|u\|_2^2$ gives the displayed [resolvent](functional-analysis.md#resolvent-of-an-operator) bound. The domain is dense and the bounded resolvent proves closedness, so the [Hille-Yosida theorem](functional-analysis.md#hille-yosida-theorem) gives a [contraction semigroup](functional-analysis.md#contraction-semigroup). An [exponentially shifted semigroup](functional-analysis.md#exponentially-shifted-semigroup) with generator $A+I$ solves the heat equation with oscillator potential.

### Thermal partition function of a quantum harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)

For a [quantum harmonic oscillator](#quantum-harmonic-oscillator) with $\hbar=1$, $\omega>0$ and [inverse temperature](thermodynamics.md#inverse-temperature) $\beta>0$, the [canonical partition function](statistical-physics.md#canonical-partition-function) is $\sum_{r\ge0}e^{-\beta\omega(r+1/2)}$. The [geometric series](real-analysis.md#geometric-series) gives the displayed formula. Keeping the [zero-point energy](#zero-point-energy) is essential to its prefactor.

### Displaced quantum harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)

Adding $-Fx$ to the [quantum harmonic oscillator](#quantum-harmonic-oscillator) potential gives $\frac12m\omega^2(x-d)^2-F^2/(2m\omega^2)$, where $d=F/(m\omega^2)$. Translation preserves the oscillator spectrum, apart from the displayed constant shift. Eigenfunctions are translated by $d$ and the energy spacing is unchanged.

#### Ground-state overlap after sudden oscillator displacement

↑ **Parent:** [Displaced quantum harmonic oscillator](#displaced-quantum-harmonic-oscillator)

In the [sudden approximation](#sudden-approximation), an initial oscillator [ground state](#ground-state) overlaps the displaced ground state by $\exp[-m\omega d^2/(4\hbar)]$. Completing the square in the product of the two normalized Gaussian wavefunctions and using the [Gaussian integral](calculus.md#gaussian-integral) proves this amplitude. Squaring it gives the displayed probability. Only an irrelevant overall phase evolves before the sudden switch.

### Zero-point energy

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zero-point_energy)

Zero-point energy is the nonzero ground-state energy left by quantum fluctuations. One harmonic oscillator contributes $\omega/2$ before any regularization or normal-ordering subtraction.

### Squeezed coherent state

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squeezed_coherent_state)

A [squeezed coherent state](#squeezed-coherent-state) is obtained from the vacuum by a squeeze operator and a displacement operator. Its quadrature variances can differ while saturating the uncertainty product. With zero displacement it is a [squeezed vacuum state](#squeezed-vacuum-state).

### Creation and annihilation operators

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Creation_and_annihilation_operators)

The bosonic ladder operators satisfy

$$
[A,A^\dagger]=1,
\qquad
A|n\rangle=\sqrt n\,|n-1\rangle,
\qquad
A^\dagger|n\rangle=\sqrt{n+1}\,|n+1\rangle.
$$

#### Annihilation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

An annihilation operator lowers the occupation [number operator](#number-operator) eigenvalue by one and annihilates the [Fock vacuum](quantum-field-theory.md#fock-vacuum).

#### Creation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

A creation operator raises the occupation [number operator](#number-operator) eigenvalue of a [quantum harmonic oscillator](#quantum-harmonic-oscillator) by one. Repeated application builds [Fock states](quantum-field-theory.md#fock-state).

#### Bosonic creation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

#### Bosonic annihilation operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

#### Single-mode squeeze operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)

For a real squeezing parameter $\gamma$, the single-mode squeeze operator is

$$
S(\gamma)=\exp\left[-\frac\gamma2\left(A^{\dagger2}-A^2\right)\right].
$$

Its exponent is [skew-adjoint](functional-analysis.md#skew-adjoint-generator), so $S(\gamma)$ is a [unitary operator](vector-space.md#unitary-operator), and it implements the [Bogoliubov transformation](quantum-field-theory.md#bogoliubov-transformation)

$$
S^\dagger AS=A\cosh\gamma-A^\dagger\sinh\gamma.
$$

##### Squeezed vacuum state

↑ **Parent:** [Single-mode squeeze operator](#single-mode-squeeze-operator)

The squeezed vacuum is the zero-displacement [squeezed coherent state](#squeezed-coherent-state) $|\gamma\rangle=S(\gamma)|0\rangle$. Its position and momentum variances are rescaled in opposite directions,

$$
(\Delta X)^2=\frac{\hbar}{2m\omega}e^{-2\gamma},
\qquad
(\Delta P)^2=\frac{m\hbar\omega}{2}e^{2\gamma},
$$

so it remains an [minimum-uncertainty state](quantum-theory.md#equality-case-of-the-heisenberg-uncertainty-relation) with $\Delta X\Delta P=\hbar/2$.

###### Multimode squeezed vacuum

↑ **Parent:** [Squeezed vacuum state](#squeezed-vacuum-state)

For an invertible finite-mode [Bogoliubov transformation](quantum-field-theory.md#bogoliubov-transformation) $a=Aa'+Ba'{}^\dagger$, the symmetric squeezing matrix is $M=-A^{-1}B$. The [canonical commutation relations](#canonical-commutation-relation) make its singular values strictly less than one. The normalized state has $|C|=\det(I-MM^\dagger)^{1/4}$. Infinitely many modes additionally require [bosonic mode mixing implementability](quantum-field-theory.md#bosonic-mode-mixing-implementability).

#### Number operator

↑ **Parent:** [Creation and annihilation operators](#creation-and-annihilation-operators)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Number_operator)

The number operator $N=A^\dagger A$ satisfies

$$
[N,A]=-A,
\qquad
[N,A^\dagger]=A^\dagger.
$$

It is self-adjoint and positive semidefinite.

##### Number state

↑ **Parent:** [Number operator](#number-operator)

A number state is a normalized [eigenstate](#eigenstate) of the [number operator](#number-operator):

$$
N|n\rangle=n|n\rangle,
\qquad n\in\mathbb Z_{\geq0}.
$$

For a single [quantum harmonic oscillator](#quantum-harmonic-oscillator), it is also an [energy eigenstate](#energy-eigenstate) with energy $\hbar\omega(n+1/2)$.

##### Integer spectrum of the number operator

↑ **Parent:** [Number operator](#number-operator)

If $N|\nu\rangle=\nu|\nu\rangle$, then $A$ lowers the eigenvalue by one and $\|A|\nu\rangle\|^2=\nu\|\nu\rangle\|^2$. Positivity forces the lowering ladder to terminate at eigenvalue zero, so every eigenvalue is a nonnegative integer.

### Two commensurate quantum harmonic oscillators

↑ **Parent:** [Quantum harmonic oscillator](#quantum-harmonic-oscillator)

For independent frequencies $1$ and $2$,

$$
H_0=N_A+2N_B+\frac32,
$$

so the eigenspace at energy $k+3/2$ has one basis state $|n,m\rangle$ for each nonnegative solution of $n+2m=k$.

## Three-dimensional isotropic harmonic oscillator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Its energies are $E_N=\hbar\omega(N+3/2)$, and level $N$ has degeneracy $\binom{N+2}{2}$.

### Cartesian number state of the three-dimensional isotropic harmonic oscillator

↑ **Parent:** [Three-dimensional isotropic harmonic oscillator](#three-dimensional-isotropic-harmonic-oscillator)

From the normalized [ground state](#ground-state) annihilated by every $A_i$, the normalized Cartesian number states are

$$
|n_1,n_2,n_3\rangle
=\prod_{i=1}^3\frac{(A_i^\dagger)^{n_i}}{\sqrt{n_i!}}|0\rangle.
$$

They have energy $\hbar\omega(n_1+n_2+n_3+3/2)$.

### Orbital angular momentum in oscillator ladder operators

↑ **Parent:** [Three-dimensional isotropic harmonic oscillator](#three-dimensional-isotropic-harmonic-oscillator)

For the [three-dimensional isotropic harmonic oscillator](#three-dimensional-isotropic-harmonic-oscillator), substituting $X_i=\sqrt{\hbar/(2\mu\omega)}(A_i+A_i^\dagger)$ and $P_i=i\sqrt{\mu\hbar\omega/2}(A_i^\dagger-A_i)$ into $L_i=\varepsilon_{ijk}X_jP_k$ gives $L_i=-i\hbar\varepsilon_{ijk}A_j^\dagger A_k$. On the first-excited Cartesian states $|j\rangle=A_j^\dagger|0\rangle$, this is the three-dimensional vector representation and $L^2|j\rangle=2\hbar^2|j\rangle$, so the whole first-excited level has orbital quantum number $\ell=1$.

## Two-dimensional isotropic harmonic oscillator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

For unit mass and angular frequency,

$$
H=a_x^\dagger a_x+a_y^\dagger a_y+1.
$$

The level with total occupation $N=n_x+n_y$ has energy $N+1$ and degeneracy $N+1$ in units where $\hbar=1$.

### Shifted two-dimensional oscillator in a uniform electric field

↑ **Parent:** [Two-dimensional isotropic harmonic oscillator](#two-dimensional-isotropic-harmonic-oscillator)

Completing the square in $H'=\tfrac12(p_x^2+p_y^2+x^2+y^2)-e\mathcal E x$ shifts the oscillator centre to $(a,0)$ and lowers every energy by $a^2/2$. Translated eigenfunctions keep their normalization. The [angular momentum](classical-mechanics.md#angular-momentum) about the new centre is $L'=(x-a)p_y-yp_x$, which commutes with $H'$, whereas the [angular momentum](classical-mechanics.md#angular-momentum) about the old centre has $[L,H']=-i\hbar ay$. For $a\ne0$, a common normalizable eigenfunction of $L,H'$ would have $y\psi=0$ and hence vanish in $L^2(\mathbb R^2)$. This stronger argument excludes individual common eigenstates; noncommutativity alone generally excludes only a complete common eigenbasis.

### Oscillator bilinear commutator

↑ **Parent:** [Two-dimensional isotropic harmonic oscillator](#two-dimensional-isotropic-harmonic-oscillator)

For bosonic modes satisfying $[a_i,a_j^\dagger]=\delta_{ij}$, the number-preserving bilinears $T_{ij}=a_i^\dagger a_j$ obey

$$
[T_{ij},T_{kl}]=\delta_{jk}T_{il}-\delta_{il}T_{kj}.
$$

### Schwinger boson representation

↑ **Parent:** [Two-dimensional isotropic harmonic oscillator](#two-dimensional-isotropic-harmonic-oscillator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schwinger_boson_representation)

Contracting two-mode oscillator bilinears with the Pauli matrices,

$$
T^a=\frac12\sigma^a_{ij}a_i^\dagger a_j,
$$

gives $[T^a,T^b]=i\varepsilon_{abc}T^c$. The subspace with total occupation $N$ is the spin-$N/2$ irreducible representation and has dimension $N+1$.

## Fermi oscillator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

A Fermi oscillator has nilpotent lowering operator $B$, anticommutator $BB^\dagger+B^\dagger B=1$, and occupation Hamiltonian $B^\dagger B$ with levels zero and one.

### Projection Hamiltonian

↑ **Parent:** [Fermi oscillator](#fermi-oscillator)

The fermionic occupation Hamiltonian satisfies $H^2=H$, so its spectrum lies in $\{0,1\}$.

### Fermionic raising and lowering operator

↑ **Parent:** [Fermi oscillator](#fermi-oscillator)

The lowering operator sends the occupied state to the vacuum and kills the vacuum; its adjoint performs the reverse and kills the occupied state.

## Tensor product of quantum systems

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Independent quantum systems combine by tensor product, with local operators acting as $A\otimes I$ or $I\otimes B$.

### Jaynes-Cummings model

↑ **Parent:** [Tensor product of quantum systems](#tensor-product-of-quantum-systems)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jaynes-Cummings_model)

The Jaynes-Cummings model couples a two-level atom to one quantized oscillator mode through

$$
H_{\rm int}=\hbar g(\sigma_+A+\sigma_-A^\dagger).
$$

The first term excites the atom while annihilating one field quantum; the second performs the Hermitian-conjugate process.

### Multiparticle quantum state

↑ **Parent:** [Tensor product of quantum systems](#tensor-product-of-quantum-systems)

For distinguishable particles with one-particle Hilbert spaces $\mathcal H_i$, the multiparticle state space is $\bigotimes_i\mathcal H_i$. A product state is a tensor product of one-particle states, while a general state is a linear combination of product states.

#### Particle exchange operator

↑ **Parent:** [Multiparticle quantum state](#multiparticle-quantum-state)

For two particles, the exchange operator sends $|\alpha\rangle\otimes|\beta\rangle$ to $|\beta\rangle\otimes|\alpha\rangle$. It has eigenvalues $+1$ on symmetric states and $-1$ on antisymmetric states.

##### Indistinguishable particles

↑ **Parent:** [Particle exchange operator](#particle-exchange-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indistinguishable_particles)

Physical states of identical particles have definite symmetry under every [particle exchange operator](#particle-exchange-operator): symmetric for bosons and antisymmetric for fermions.

###### Boson

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boson)

Bosons are identical particles whose total multiparticle state is symmetric under exchange. In three-dimensional relativistic quantum theory they have integer spin.

###### Bosonic exchange symmetry

↑ **Parent:** [Boson](#boson)

[Bosonic exchange symmetry](#bosonic-exchange-symmetry) is the symmetric exchange statistics of identical [bosons](#boson). Commuting [creation operators](#creation-operator) build the symmetric [bosonic Fock space](quantum-field-theory.md#bosonic-fock-space); a normalized one-particle mode has occupation states $(a^\dagger)^n|0\rangle/\sqrt{n!}$ for every nonnegative integer $n$. At thermal equilibrium this symmetry leads to [Bose-Einstein statistics](statistical-physics.md#bose-einstein-statistics) and the [Bose-Einstein distribution](statistical-physics.md#bose-einstein-distribution). Exchange symmetry itself does not require thermal equilibrium.

###### Bosonic statistics from commuting creation operators

↑ **Parent:** [Bosonic exchange symmetry](#bosonic-exchange-symmetry)

Commuting [creation operators](#creation-operator) make multiparticle states invariant under exchange of their labels. With $[a,a^\dagger]=1$, the normalized number states $(a^\dagger)^r|0\rangle/\sqrt{r!}$ exist for all $r\ge0$, giving unrestricted [bosonic occupation numbers](quantum-field-theory.md#bosonic-occupation-number). The single-mode thermal sum is $Z=\sum_{r\ge0}e^{-\beta Er}=(1-e^{-\beta E})^{-1}$ and the mean occupation is $(e^{\beta E}-1)^{-1}$. Thus the exchange symmetry and the [Bose-Einstein distribution](statistical-physics.md#bose-einstein-distribution) are two expressions of the same bosonic algebra.

###### Fermion

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermion)

Fermions are identical particles whose total multiparticle state is antisymmetric under exchange. In three-dimensional relativistic quantum theory they have half-integer spin.

###### Fermi-Dirac statistics

↑ **Parent:** [Fermion](#fermion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermi-Dirac_statistics)

The antisymmetric exchange statistics of identical [fermions](#fermion). Interchanging two one-particle labels reverses the total state, and fermionic [creation operators](#creation-operator) anticommute. Occupation of a one-particle mode is therefore zero or one, giving the [Pauli exclusion principle](#pauli-exclusion-principle); thermal equilibrium leads to the [Fermi-Dirac distribution](statistical-physics.md#fermi-dirac-distribution). Color, flavor, spin and orbital factors must together have the required antisymmetry, even if one factor is symmetric.

###### Exchange symmetry of two identical spin-one-half fermions

↑ **Parent:** [Fermion](#fermion)

For two identical spin-one-half fermions with no additional antisymmetric internal factor, the antisymmetric [spin-one-half singlet state](#spin-one-half-singlet-state) combines with an even-$\ell$ symmetric orbital state, while the symmetric [spin-one-half triplet state](#spin-one-half-triplet-state) combines with an odd-$\ell$ antisymmetric orbital state.

###### Pauli exclusion principle

↑ **Parent:** [Fermion](#fermion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pauli_exclusion_principle)

No two identical fermions may occupy the same one-particle quantum state. At zero temperature, noninteracting fermions fill the available one-particle states in increasing order of energy.

###### Spin-statistics theorem

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin-statistics_theorem)

The spin-statistics theorem associates integer-spin particles with bosonic exchange symmetry and half-integer-spin particles with fermionic exchange symmetry in relativistic quantum field theory under the standard locality and positivity assumptions.

###### Two identical spin-one bosons

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)

For two spin-one particles, the spin tensor product has a six-dimensional symmetric subspace and a three-dimensional antisymmetric subspace. A symmetric spatial state combines with symmetric spin, while an antisymmetric spatial state combines with antisymmetric spin, so that the total bosonic state remains symmetric.

###### Degeneracy of two identical spin-one bosons with equally spaced orbital levels

↑ **Parent:** [Two identical spin-one bosons](#two-identical-spin-one-bosons)

If $E_n=E_0+n\Delta$, the two-particle level $2E_0+N\Delta$ has degeneracy

$$
g_N=\begin{cases}
\dfrac92N+6,&N\text{ even},\\[3pt]
\dfrac92(N+1),&N\text{ odd}.
\end{cases}
$$

Each unequal orbital pair contributes six symmetric-spin states and three antisymmetric-spin states; an equal orbital pair exists only for even $N$ and contributes six states.

### Decoupled Fermi oscillators

↑ **Parent:** [Tensor product of quantum systems](#tensor-product-of-quantum-systems)

Two decoupled Fermi oscillators have product occupation states and additive energies $E_1n_1+E_2n_2$.

### Kronecker product representation of local operators

↑ **Parent:** [Tensor product of quantum systems](#tensor-product-of-quantum-systems)

In a product basis, an operator local to one subsystem is represented by its matrix Kronecker the identity on every other subsystem.

### Decoupled commuting Hamiltonian terms

↑ **Parent:** [Tensor product of quantum systems](#tensor-product-of-quantum-systems)

Commuting Hamiltonian terms on separate factors are simultaneously diagonalized by tensor products of their eigenvectors and have additive eigenvalues.

## Time-dependent perturbation theory

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Expanding a state in unperturbed energy eigenstates with their free phases converts the time-dependent Schrodinger equation into coupled equations for slowly varying amplitudes. To first order, the perturbation on the right-hand side acts on the initial unperturbed state.

This is the time-dependent branch of [perturbation theory](#perturbation-theory-quantum-mechanics); its corrections describe transition amplitudes.

### Electric-dipole interaction

↑ **Parent:** [Time-dependent perturbation theory](#time-dependent-perturbation-theory)

In the long-wavelength approximation, a particle of charge $q$ in a spatially uniform electric field has perturbation

$$
\Delta(t)=-q\mathbf E(t)\mathbin{\cdot}\mathbf r.
$$

Its transition amplitudes are controlled by matrix elements of the position operator.

#### Electric-dipole selection rule

↑ **Parent:** [Electric-dipole interaction](#electric-dipole-interaction)

Because the position operator has odd [parity](#parity), an electric-dipole matrix element vanishes between states of the same parity. For orbital-angular-momentum eigenstates, the full rule is $\Delta\ell=\pm1$ and $\Delta m=0,\pm1$, with the field polarization selecting the allowed change in $m$.

### Continuum transition probability at long times

↑ **Parent:** [Time-dependent perturbation theory](#time-dependent-perturbation-theory)

For a harmonic perturbation and continuum detuning $\Omega(k)$, first-order amplitudes contain

$$
\frac{\sin(\Omega(k)t/2)}{\Omega(k)/2}.
$$

The distributional limit

$$
\frac{\sin^2(\Omega t/2)}{(\Omega/2)^2}
\longrightarrow 2\pi t\,\delta(\Omega)
$$

selects energy-conserving continuum states and produces a transition probability linear in time.

## Time-independent perturbation theory

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Time-independent perturbation theory expands the eigenvalues and eigenstates of $H_0+V$ in powers of a small perturbation $V$.

This is the stationary branch of [perturbation theory](#perturbation-theory-quantum-mechanics).

<h3 id="hellmann-feynman-theorem">Hellmann–Feynman theorem</h3>

↑ **Parent:** [Time-independent perturbation theory](#time-independent-perturbation-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hellmann–Feynman_theorem)

For a differentiable normalized [eigenstate](#eigenstate) of a differentiable [self-adjoint](linear-operator-theory.md#self-adjoint-operator) [Hamiltonian](classical-mechanics.md#hamiltonian), differentiate $H\psi=E\psi$ and pair with $\psi$. The terms involving $\psi'$ cancel because $H$ is [self-adjoint](linear-operator-theory.md#self-adjoint-operator), leaving the stated formula. It turns energy [derivatives](calculus.md#derivative) into observable expectations. A smoothly chosen eigenbranch and suitable operator-domain regularity are required, particularly at degeneracies or crossings.

### First-order energy correction

↑ **Parent:** [Time-independent perturbation theory](#time-independent-perturbation-theory)

The first-order energy correction is the coefficient of the perturbation parameter in the expansion of an energy eigenvalue.

### Nondegenerate energy eigenvalue

↑ **Parent:** [Time-independent perturbation theory](#time-independent-perturbation-theory)

An [energy eigenvalue](#energy-eigenvalue) is nondegenerate when its [eigenspace](linear-operator-theory.md#eigenspace) is one-dimensional. Its normalized [eigenstate](#eigenstate) is then unique up to a complex phase.

### First-order nondegenerate perturbation theory

↑ **Parent:** [Time-independent perturbation theory](#time-independent-perturbation-theory)

For a normalized eigenstate $|n\rangle$ belonging to a [nondegenerate energy eigenvalue](#nondegenerate-energy-eigenvalue),

$$
E_n^{(1)}=\langle n|V|n\rangle,
\qquad
|n^{(1)}\rangle
=\sum_{m\ne n}|m\rangle
\frac{\langle m|V|n\rangle}{E_n^{(0)}-E_m^{(0)}}.
$$

#### First-order ground state of the quartic oscillator

↑ **Parent:** [First-order nondegenerate perturbation theory](#first-order-nondegenerate-perturbation-theory)

For a [quantum harmonic oscillator](#quantum-harmonic-oscillator) perturbed by $\lambda X^4$, write $X=\sqrt{\hbar/(2m\omega)}(A+A^\dagger)$. Since

$$
(A+A^\dagger)^4|0\rangle=3|0\rangle+6\sqrt2|2\rangle+2\sqrt6|4\rangle,
$$

[first-order nondegenerate perturbation theory](#first-order-nondegenerate-perturbation-theory) gives

$$
\boxed{|0_\lambda\rangle
=|0\rangle-\frac{\hbar\lambda}{4m^2\omega^3}
\left(3\sqrt2|2\rangle+\sqrt{\frac32}|4\rangle\right)+O(\lambda^2).}
$$

### Second-order nondegenerate perturbation theory

↑ **Parent:** [Time-independent perturbation theory](#time-independent-perturbation-theory)

For a normalized nondegenerate eigenstate $|n\rangle$,

$$
E_n^{(2)}
=\sum_{m\ne n}
\frac{|\langle m|V|n\rangle|^2}
{E_n^{(0)}-E_m^{(0)}}.
$$

For a ground state, every denominator is negative, so the correction is nonpositive.

### Imaginary-coupled two-level Hamiltonian

↑ **Parent:** [Time-independent perturbation theory](#time-independent-perturbation-theory)

For

$$
H=\begin{pmatrix}E_-&-i\lambda\\i\lambda&E_+\end{pmatrix},
\qquad \Delta=E_+-E_->0,
$$

the exact energies are

$$
E_{\pm}^{\rm exact}
=\frac{E_-+E_+}{2}
\pm\sqrt{\frac{\Delta^2}{4}+\lambda^2}.
$$

The perturbation series around $\lambda=0$ has radius $\Delta/2$, set by the branch points $\lambda=\pm i\Delta/2$.

### Bright and dark state reduction of a star-coupled Hamiltonian

↑ **Parent:** [Time-independent perturbation theory](#time-independent-perturbation-theory)

Suppose one state $|0\rangle$ couples to degenerate states $|1\rangle,\ldots,|m\rangle$ with amplitudes $v_1,\ldots,v_m$, while the degenerate states do not couple to each other. The normalized bright state proportional to $\sum_jv_j|j\rangle$ is the only combination coupled to $|0\rangle$. Every orthogonal combination is a dark state and remains an exact eigenstate at the degenerate energy. The remaining spectrum comes from a two-dimensional Hamiltonian whose off-diagonal entry is $(\sum_j|v_j|^2)^{1/2}$.

## Degenerate perturbation theory

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degenerate_perturbation_theory)

First-order degenerate perturbation theory diagonalizes the perturbing operator within each degenerate eigenspace of the unperturbed Hamiltonian.

### Perturbation diagonal within a degenerate eigenspace

↑ **Parent:** [Degenerate perturbation theory](#degenerate-perturbation-theory)

If the perturbation is already diagonal in a basis of a degenerate eigenspace, those basis vectors receive its diagonal entries as first-order shifts.

### Exact diagonalization within a degenerate subspace

↑ **Parent:** [Degenerate perturbation theory](#degenerate-perturbation-theory)

When a perturbation preserves each unperturbed degenerate block and has no inter-block coupling, diagonalizing each block can give the exact spectrum.

#### Resonant two-to-one oscillator coupling

↑ **Parent:** [Exact diagonalization within a degenerate subspace](#exact-diagonalization-within-a-degenerate-subspace)

For oscillators of frequencies $1$ and $2$, the perturbation

$$
H'=A^{\dagger2}B+A^2B^\dagger
$$

preserves $N_A+2N_B$. On the energy-$9/2$ basis $|3,0\rangle,|1,1\rangle$, it is the matrix

$$
\begin{pmatrix}0&\sqrt6\\\sqrt6&0\end{pmatrix},
$$

so the symmetric and antisymmetric combinations are exact eigenstates with shifts $\pm\sqrt6\lambda$.

## Pauli X eigenstate

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

The Pauli $X$ eigenstates are $(|0\rangle\pm|1\rangle)/\sqrt2$ with eigenvalues $\pm1$.

These are the eigenvectors of one [Pauli matrix](algebra.md#pauli-matrices), not an alternative name for the whole matrix family.

## Rectangular potential barrier

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rectangular_potential_barrier)

A [rectangular potential barrier](#rectangular-potential-barrier) has a constant elevated potential over a finite interval and a lower constant potential outside it. Matching wavefunctions and derivatives at the interval endpoints gives its reflection and transmission amplitudes. It is a special [potential barrier](#potential-barrier).

## Perturbation theory (quantum mechanics)

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perturbation_theory_(quantum_mechanics))

[Perturbation theory](#perturbation-theory-quantum-mechanics) expands a quantum problem around a solvable Hamiltonian. [Time-independent perturbation theory](#time-independent-perturbation-theory) expands stationary energies and eigenstates; [time-dependent perturbation theory](#time-dependent-perturbation-theory) expands dynamical amplitudes and transitions.

## Hartree equations

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hartree_equations)

The [Hartree equations](#hartree-equations) are self-consistent one-particle equations obtained by approximating a many-body [wave function](#wave-function) by a [tensor product](linear-algebra.md#tensor-product) of orbital [wave functions](#wave-function). Each orbital sees the potential averaged over the other particles' [probability densities](#probability-density); attractive Newtonian mean-field variants include the [Gravitational Hartree equation](nonlinear-analysis.md#gravitational-hartree-equation).

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)
