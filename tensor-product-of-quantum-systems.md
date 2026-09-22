# Tensor product of quantum systems

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)

Independent quantum systems combine by tensor product, with local operators acting as $A\otimes I$ or $I\otimes B$.

**Table of contents**

- [Spin-boson model](#spin-boson-model)
  - [Golden-rule relaxation of a spin coupled to an oscillator bath](#golden-rule-relaxation-of-a-spin-coupled-to-an-oscillator-bath)
- [Jaynes-Cummings model](#jaynes-cummings-model)
- [Multiparticle quantum state](#multiparticle-quantum-state)
  - [Particle exchange operator](#particle-exchange-operator)
    - [Indistinguishable particles](#indistinguishable-particles)
      - [Two spin-one-half fermions on a ring](#two-spin-one-half-fermions-on-a-ring)
      - [Exchange operator](#exchange-operator)
      - [Symmetrization postulate](#symmetrization-postulate)
      - [Boson](#boson)
        - [Bosonic exchange symmetry](#bosonic-exchange-symmetry)
          - [Bosonic coincidence enhancement in two orthogonal orbitals](#bosonic-coincidence-enhancement-in-two-orthogonal-orbitals)
          - [Bosonic statistics from commuting creation operators](#bosonic-statistics-from-commuting-creation-operators)
      - [Fermion](#fermion)
        - [Pauli principle](#pauli-principle)
        - [Fermi-Dirac statistics](#fermi-dirac-statistics)
          - [Normalized complete Fermi-Dirac integral](#normalized-complete-fermi-dirac-integral)
            - [Carrier densities with chemical potential pinned to a band edge](#carrier-densities-with-chemical-potential-pinned-to-a-band-edge)
            - [Boltzmann limit of the normalized Fermi-Dirac integral](#boltzmann-limit-of-the-normalized-fermi-dirac-integral)
            - [Fermi-Dirac half-order integral at zero argument](#fermi-dirac-half-order-integral-at-zero-argument)
        - [Exchange symmetry of two identical spin-one-half fermions](#exchange-symmetry-of-two-identical-spin-one-half-fermions)
          - [Two-electron states in the first two shells of an isotropic oscillator](#two-electron-states-in-the-first-two-shells-of-an-isotropic-oscillator)
            - [Spin-orbit splitting of the first excited two-electron oscillator level](#spin-orbit-splitting-of-the-first-excited-two-electron-oscillator-level)
          - [Exchange-coupled spin-one-half particles in an infinite square well](#exchange-coupled-spin-one-half-particles-in-an-infinite-square-well)
          - [Contact shifts of two spin-one-half fermions in a harmonic trap](#contact-shifts-of-two-spin-one-half-fermions-in-a-harmonic-trap)
        - [Pauli exclusion principle](#pauli-exclusion-principle)
          - [Spin degeneracy in filling a one-dimensional well](#spin-degeneracy-in-filling-a-one-dimensional-well)
          - [Balanced two-mode fermion antibunching](#balanced-two-mode-fermion-antibunching)
          - [Pauli blocking](#pauli-blocking)
          - [Spectroscopic origin of the Pauli exclusion principle](#spectroscopic-origin-of-the-pauli-exclusion-principle)
          - [Counting spin orbitals in an electron shell](#counting-spin-orbitals-in-an-electron-shell)
          - [Spatial orbital](#spatial-orbital)
            - [Spin orbital](#spin-orbital)
          - [Two-particle antisymmetrization](#two-particle-antisymmetrization)
            - [Slater determinant](#slater-determinant)
              - [Slater-Condon rules](#slater-condon-rules)
          - [Exclusion versus particle position](#exclusion-versus-particle-position)
          - [Zero-temperature filling of finite fermion levels](#zero-temperature-filling-of-finite-fermion-levels)
            - [Fermionic state counting](#fermionic-state-counting)
            - [Exclusion and the energy of two electrons in three spatial levels](#exclusion-and-the-energy-of-two-electrons-in-three-spatial-levels)
          - [Fermionic atom antibunching](#fermionic-atom-antibunching)
            - [Pair detection correlation](#pair-detection-correlation)
            - [Magnetic trapping of neutral atoms](#magnetic-trapping-of-neutral-atoms)
            - [Time-of-flight atom detection](#time-of-flight-atom-detection)
              - [Microchannel plate detector](#microchannel-plate-detector)
      - [Spin-statistics theorem](#spin-statistics-theorem)
        - [Vector decay into identical spin-zero mesons](#vector-decay-into-identical-spin-zero-mesons)
        - [Nuclear spin statistics](#nuclear-spin-statistics)
        - [Composite statistics of neutral atoms](#composite-statistics-of-neutral-atoms)
      - [Two identical spin-one bosons](#two-identical-spin-one-bosons)
        - [Degeneracy of two identical spin-one bosons with equally spaced orbital levels](#degeneracy-of-two-identical-spin-one-bosons-with-equally-spaced-orbital-levels)
- [Decoupled Fermi oscillators](#decoupled-fermi-oscillators)
- [Kronecker product representation of local operators](#kronecker-product-representation-of-local-operators)
- [Decoupled commuting Hamiltonian terms](#decoupled-commuting-hamiltonian-terms)

## Spin-boson model

↑ **Parent:** [Tensor product of quantum systems](tensor-product-of-quantum-systems.md)

A spin-boson model couples a two-state [quantum system](quantum-system.md) to a collection of [quantum harmonic oscillators](quantum-harmonic-oscillator.md). The oscillator modes provide environmental degrees of freedom that can exchange energy with the [spin](angular-momentum-operator.md#spin) and change its [reduced density matrix](bell-state.md#reduced-density-matrix). One transverse-coupling convention is

$$
H=\frac{\hbar\Omega}2\sigma_z+\sum_j\hbar\omega_j(a_j^\dagger a_j+1/2)
+\sigma_x\sum_j\lambda_j(a_j^\dagger+a_j).
$$

The choice of coupling axis matters: here the [Pauli matrix](algebra.md#pauli-matrices) $\sigma_x$ flips the energy-basis [spin](angular-momentum-operator.md#spin) states. Coupling only through $\sigma_z$ has a different effect, since it commutes with the free spin [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics).

### Golden-rule relaxation of a spin coupled to an oscillator bath

↑ **Parent:** [Spin-boson model](#spin-boson-model)

For transverse coupling with equal mode amplitudes $\lambda$, [Fermi's golden rule](quantum-mechanics.md#fermi-s-golden-rule) and the oscillator [creation operator](quantum-harmonic-oscillator.md#creation-operator) and [annihilation operator](quantum-harmonic-oscillator.md#annihilation-operator) give

$$
\Gamma_{\downarrow\uparrow}=\Gamma_0(n_\Omega+1),\qquad
\Gamma_{\uparrow\downarrow}=\Gamma_0n_\Omega,\qquad
\Gamma_0=\frac{2\pi\lambda^2}{\hbar^2}g(\Omega),
$$

where the first index is the final spin and $g$ is the [density of states](quantum-ideal-gas-statistics.md#density-of-states) per unit angular frequency. Decay creates a quantum and carries the factor $n_\Omega+1$; excitation annihilates one and carries $n_\Omega$. For nonuniform resonant occupations, $n_\Omega$ is their density-weighted mean.

With a thermal [Bose-Einstein distribution](quantum-ideal-gas-statistics.md#bose-einstein-distribution), $n_\Omega/(n_\Omega+1)=e^{-\beta\hbar\Omega}$. The two-state [master equation](continuous-time-markov-chain.md#master-equation) therefore has the [Boltzmann distribution](thermodynamics.md#boltzmann-distribution) as its unique stationary populations when $\Gamma_0>0$. The population deviation relaxes at rate $\Gamma_0(2n_\Omega+1)$. If there is no resonant coupling, both rates vanish and stationarity does not determine the populations.

## Jaynes-Cummings model

↑ **Parent:** [Tensor product of quantum systems](tensor-product-of-quantum-systems.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jaynes-Cummings_model)

The Jaynes-Cummings model couples a two-level atom to one quantized oscillator mode through

$$
H_{\rm int}=\hbar g(\sigma_+A+\sigma_-A^\dagger).
$$

The first term excites the atom while annihilating one field quantum; the second performs the Hermitian-conjugate process.

## Multiparticle quantum state

↑ **Parent:** [Tensor product of quantum systems](tensor-product-of-quantum-systems.md)

For distinguishable particles with one-particle Hilbert spaces $\mathcal H_i$, the multiparticle state space is $\bigotimes_i\mathcal H_i$. A product state is a tensor product of one-particle states, while a general state is a linear combination of product states.

### Particle exchange operator

↑ **Parent:** [Multiparticle quantum state](#multiparticle-quantum-state)

For two particles, the exchange operator sends $|\alpha\rangle\otimes|\beta\rangle$ to $|\beta\rangle\otimes|\alpha\rangle$. It has eigenvalues $+1$ on symmetric states and $-1$ on antisymmetric states.

#### Indistinguishable particles

↑ **Parent:** [Particle exchange operator](#particle-exchange-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indistinguishable_particles)

Physical states of identical particles have definite symmetry under every [particle exchange operator](#particle-exchange-operator): symmetric for bosons and antisymmetric for fermions.

##### Two spin-one-half fermions on a ring

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)

For free [fermions](#fermion) on a ring, each one-particle orbital has integer [angular momentum](momentum.md#angular-momentum) label $l$ and two [spin](angular-momentum-operator.md#spin) states. Two particles occupy the $l=0$ orbital in a unique [singlet state](angular-momentum-operator.md#singlet-state) at zero kinetic [energy](energy.md). At the next distinct [energy](energy.md) $\hbar^2/(2mR^2)$, orbitals $0,+1$ or $0,-1$ can be combined with one [singlet state](angular-momentum-operator.md#singlet-state) or three [triplet state](angular-momentum-operator.md#spin-one-half-triplet-state) [spin](angular-momentum-operator.md#spin) states, giving total [quantum degeneracy](quantum-mechanics.md#degenerate-energy-levels) eight. The lowest [triplet state](angular-momentum-operator.md#spin-one-half-triplet-state) has six states and its antisymmetric spatial factor vanishes when the particles coincide.

##### Exchange operator

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)

The operator $\hat P_{12}$ interchanges all one-particle variables for particles 1 and 2. Since $\hat P_{12}^2=\hat I$, a state of definite exchange symmetry has [eigenvalue](linear-operator-theory.md#eigenvalue) $+1$ or $-1$.

##### Symmetrization postulate

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)

The complete state of identical [bosons](#boson) is symmetric under exchange, while that of identical [fermions](#fermion) is antisymmetric. The condition includes [spin](angular-momentum-operator.md#spin) and other internal variables as well as spatial coordinates.

##### Boson

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boson)

Bosons are identical particles whose total multiparticle state is symmetric under exchange. In three-dimensional relativistic quantum theory they have integer spin.

###### Bosonic exchange symmetry

↑ **Parent:** [Boson](#boson)

[Bosonic exchange symmetry](#bosonic-exchange-symmetry) is the symmetric exchange statistics of identical [bosons](#boson). Commuting [creation operators](quantum-harmonic-oscillator.md#creation-operator) build the symmetric [bosonic Fock space](quantum-field-theory.md#bosonic-fock-space); a normalized one-particle mode has occupation states $(a^\dagger)^n|0\rangle/\sqrt{n!}$ for every nonnegative integer $n$. At thermal equilibrium this symmetry leads to [Bose-Einstein statistics](quantum-ideal-gas-statistics.md#bose-einstein-statistics) and the [Bose-Einstein distribution](quantum-ideal-gas-statistics.md#bose-einstein-distribution). Exchange symmetry itself does not require thermal equilibrium.

###### Bosonic coincidence enhancement in two orthogonal orbitals

↑ **Parent:** [Bosonic exchange symmetry](#bosonic-exchange-symmetry)

Place one noninteracting spin-zero [boson](#boson) in each of two orthonormal orbitals $a,b$. Its normalized symmetric spatial [wavefunction](wave-function.md) is $[a(\mathbf r_1)b(\mathbf r_2)+b(\mathbf r_1)a(\mathbf r_2)]/\sqrt2$. At coincident positions the [probability density](wave-function.md#probability-density) is $2|a(\mathbf r)|^2|b(\mathbf r)|^2$, twice the labelled distinguishable-product value. Coincidence at an exact point is understood as a density or the limit of small detector volumes. If both particles occupy the same orbital, the normalized product is already symmetric and this comparison gives factor one instead; the factor two is not a universal property of every two-boson state.

###### Bosonic statistics from commuting creation operators

↑ **Parent:** [Bosonic exchange symmetry](#bosonic-exchange-symmetry)

Commuting [creation operators](quantum-harmonic-oscillator.md#creation-operator) make multiparticle states invariant under exchange of their labels. With $[a,a^\dagger]=1$, the normalized number states $(a^\dagger)^r|0\rangle/\sqrt{r!}$ exist for all $r\ge0$, giving unrestricted [bosonic occupation numbers](quantum-field-theory.md#bosonic-occupation-number). The single-mode thermal sum is $Z=\sum_{r\ge0}e^{-\beta Er}=(1-e^{-\beta E})^{-1}$ and the mean occupation is $(e^{\beta E}-1)^{-1}$. Thus the exchange symmetry and the [Bose-Einstein distribution](quantum-ideal-gas-statistics.md#bose-einstein-distribution) are two expressions of the same bosonic algebra.

##### Fermion

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermion)

Fermions are identical particles whose total multiparticle state is antisymmetric under exchange. In three-dimensional relativistic quantum theory they have half-integer spin.

###### Pauli principle

↑ **Parent:** [Fermion](#fermion)

The complete [wavefunction](wave-function.md) of identical [fermions](#fermion) changes sign on exchange of two particles, including their spatial and internal coordinates. The [Pauli exclusion principle](#pauli-exclusion-principle) follows because an antisymmetrized product with two identical complete [spin orbitals](#spin-orbital) is zero. Antisymmetry concerns the total state; a spin-antisymmetric [singlet state](angular-momentum-operator.md#singlet-state) can have a symmetric spatial factor.

###### Fermi-Dirac statistics

↑ **Parent:** [Fermion](#fermion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermi-Dirac_statistics)

The antisymmetric exchange statistics of identical [fermions](#fermion). Interchanging two one-particle labels reverses the total state, and fermionic [creation operators](quantum-harmonic-oscillator.md#creation-operator) anticommute. Occupation of a one-particle mode is therefore zero or one, giving the [Pauli exclusion principle](#pauli-exclusion-principle); thermal equilibrium leads to the [Fermi-Dirac distribution](quantum-ideal-gas-statistics.md#fermi-dirac-distribution). Color, flavor, spin and orbital factors must together have the required antisymmetry, even if one factor is symmetric.

###### Normalized complete Fermi-Dirac integral

↑ **Parent:** [Fermi-Dirac statistics](#fermi-dirac-statistics)

The convention $F_j(\eta)=\Gamma(j+1)^{-1}\int_0^\infty x^j/[1+e^{x-\eta}]\,dx$ is useful for parabolic-band carrier densities. In three dimensions, a spin-degenerate single valley has $n=2[mk_BT/(2\pi\hbar^2)]^{3/2}F_{1/2}[(\mu-E_c)/(k_BT)]$. Other conventions omit the gamma normalization, so prefactors must be stated.

###### Carrier densities with chemical potential pinned to a band edge

↑ **Parent:** [Normalized complete Fermi-Dirac integral](#normalized-complete-fermi-dirac-integral)

For equal-mass conduction and valence edges at $0,-E_g$ and fixed $\mu=0$, $n=N(T)F_{1/2}(0)$ and $p=N(T)F_{1/2}[-E_g/(k_BT)]$, where $N(T)=2[mk_BT/(2\pi\hbar^2)]^{3/2}$. Other states pinning the [chemical potential](chemical-potential.md) can compensate the unequal carrier charges; imposing intrinsic [charge neutrality](electric-charge.md#charge-neutrality) in addition would change the problem.

###### Boltzmann limit of the normalized Fermi-Dirac integral

↑ **Parent:** [Normalized complete Fermi-Dirac integral](#normalized-complete-fermi-dirac-integral)

###### Fermi-Dirac half-order integral at zero argument

↑ **Parent:** [Normalized complete Fermi-Dirac integral](#normalized-complete-fermi-dirac-integral)

Expanding the Fermi denominator as an alternating exponential series gives $F_{1/2}(0)=(1-2^{-1/2})\zeta(3/2)\simeq0.765147$. Thus a band with [chemical potential](chemical-potential.md) pinned exactly at its lower edge has $n=F_{1/2}(0)N_c$, rather than the classical result $N_c$.

###### Exchange symmetry of two identical spin-one-half fermions

↑ **Parent:** [Fermion](#fermion)

For two identical spin-one-half fermions with no additional antisymmetric internal factor, the antisymmetric [spin-one-half singlet state](angular-momentum-operator.md#spin-one-half-singlet-state) combines with an even-$\ell$ symmetric orbital state, while the symmetric [spin-one-half triplet state](angular-momentum-operator.md#spin-one-half-triplet-state) combines with an odd-$\ell$ antisymmetric orbital state.

###### Two-electron states in the first two shells of an isotropic oscillator

↑ **Parent:** [Exchange symmetry of two identical spin-one-half fermions](#exchange-symmetry-of-two-identical-spin-one-half-fermions)

The spatial ground orbital of a three-dimensional [quantum harmonic oscillator](quantum-harmonic-oscillator.md) has $l=0$ and energy $3\hbar\omega_0/2$; its first excited shell has $l=1$ and energy $5\hbar\omega_0/2$. Two identical [electrons](physics.md#electron) both in the ground orbital must form the [singlet state](angular-momentum-operator.md#singlet-state), giving one state at total energy $3\hbar\omega_0$.

At energy $4\hbar\omega_0$, one electron occupies each shell. There are two ground-shell spin orbitals and six first-excited-shell spin orbitals, hence twelve [Slater determinants](#slater-determinant). Equivalently, $0\otimes1$ gives $L=1$; symmetric spatial combinations with the [singlet state](angular-momentum-operator.md#singlet-state) give three states, while antisymmetric spatial combinations with the [triplet states](angular-momentum-operator.md#spin-one-half-triplet-state) give nine. Distinct occupied orbitals allow both spatial exchange symmetries, so both spin sectors must be kept.

###### Spin-orbit splitting of the first excited two-electron oscillator level

↑ **Parent:** [Two-electron states in the first two shells of an isotropic oscillator](#two-electron-states-in-the-first-two-shells-of-an-isotropic-oscillator)

For the interaction $\lambda\mathbf S\cdot\mathbf L$ built from the total two-electron [spin](angular-momentum-operator.md#spin) and [orbital angular momentum](quantum-mechanics.md#orbital-angular-momentum), set $\mathbf J=\mathbf L+\mathbf S$. The [spin-dot-product eigenvalue](angular-momentum-operator.md#spin-dot-product-eigenvalue) identity then gives the shift in the title. In the first excited two-electron oscillator manifold, the singlet has $L=1,S=0,J=1$ and zero shift with multiplicity three. The triplet has $L=S=1$, with $J=0,1,2$ shifts $-2\lambda\hbar^2,-\lambda\hbar^2,+\lambda\hbar^2$ and multiplicities $1,3,5$.

The multiplicities sum to twelve, and their weighted shift sums to zero. The specified interaction preserves both $L^2$ and $S^2$; it is distinct from summing separate single-electron spin-orbit interactions. Its shifts are exact within this model's invariant oscillator manifold, with weak coupling ensuring the original level ordering remains useful.

###### Exchange-coupled spin-one-half particles in an infinite square well

↑ **Parent:** [Exchange symmetry of two identical spin-one-half fermions](#exchange-symmetry-of-two-identical-spin-one-half-fermions)

For well width $a$, put $\varepsilon=\pi^2\hbar^2/(2ma^2)$ and $J=\lambda\hbar^2$ when the interaction is $-\lambda\mathbf S_1\cdot\mathbf S_2$. The [spin-dot-product eigenvalue](angular-momentum-operator.md#spin-dot-product-eigenvalue) gives exchange energies $3J/4$ for the [singlet state](angular-momentum-operator.md#singlet-state) and $-J/4$ for the [triplet states](angular-momentum-operator.md#spin-one-half-triplet-state). Identical [fermions](#fermion) require symmetric spatial orbitals with the singlet and antisymmetric orbitals with the triplet. Two particles in the same orbital can therefore only be singlets.

For $0<J\ll\varepsilon$, the three lowest distinct [energy levels](quantum-mechanics.md#energy-level) are the orbital-$11$ singlet at $2\varepsilon+3J/4$, orbital-$12$ triplet at $5\varepsilon-J/4$, and orbital-$12$ singlet at $5\varepsilon+3J/4$, with multiplicities $1,3,1$. Distinguishable particles instead allow an orbital-$11$ triplet, making the lowest three levels $2\varepsilon-J/4$, $2\varepsilon+3J/4$, and $5\varepsilon-J/4$, with multiplicities $3,1,6$. The sixfold level includes both orbital orderings. For negative $J$, the spin-sector orderings reverse within each fixed orbital sum.

###### Contact shifts of two spin-one-half fermions in a harmonic trap

↑ **Parent:** [Exchange symmetry of two identical spin-one-half fermions](#exchange-symmetry-of-two-identical-spin-one-half-fermions)

For two identical [fermions](#fermion) of mass $m$ in the same one-dimensional [quantum harmonic oscillator](quantum-harmonic-oscillator.md), use [center of mass](classical-mechanics.md#center-of-mass) $X=(x_1+x_2)/2$ and separation $r=x_1-x_2$. The corresponding oscillator masses are $2m$ and [reduced mass](classical-mechanics.md#reduced-mass) $m/2$, with the same frequency $\omega$. If $N,n$ are their occupation numbers, the unperturbed energy is $\hbar\omega(N+n+1)$. The [fermionic exchange symmetry](#fermi-dirac-statistics) requires even $n$ with a [spin-one-half singlet state](angular-momentum-operator.md#spin-one-half-singlet-state) and odd $n$ with a [spin-one-half triplet state](angular-momentum-operator.md#spin-one-half-triplet-state).

For a [delta potential](quantum-mechanics.md#delta-potential) $\lambda\delta(r)$ the first-order shift is $\lambda|\varphi_n^{\mathrm{rel}}(0)|^2$. Every odd relative [wavefunction](wave-function.md) vanishes at contact, so these states remain exact unaffected eigenstates of the spatial problem. For the even relative ground state, the [oscillator length](quantum-harmonic-oscillator.md#oscillator-length) is $\sqrt2\ell$, where $\ell=\sqrt{\hbar/(m\omega)}$, and the shift is $\lambda/(\sqrt{2\pi}\ell)$, independent of $N$. This separates interaction-sensitive singlets from contact-insensitive triplets.

###### Pauli exclusion principle

↑ **Parent:** [Fermion](#fermion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pauli_exclusion_principle)

The [Pauli exclusion principle](#pauli-exclusion-principle) says that each complete [one-particle state](quantum-field-theory.md#one-particle-state) can have [fermionic occupation number](quantum-field-theory.md#fermionic-occupation-number) zero or one. “Complete” includes [spin](angular-momentum-operator.md#spin) and any other internal labels, as well as the spatial [wavefunction](wave-function.md). Thus two [electrons](physics.md#electron) can share a [spatial orbital](#spatial-orbital) with opposite [spin](angular-momentum-operator.md#spin) projections: these are two different [spin orbitals](#spin-orbital). Equal energy alone does not mean equal [quantum state](quantum-system.md#quantum-state), because [degenerate energy levels](quantum-mechanics.md#degenerate-energy-levels) contain several independent [one-particle states](quantum-field-theory.md#one-particle-state).

This distinction explains how an [electron shell](chemistry.md#electron-shell) can accommodate several [electrons](physics.md#electron) while exclusion still allows only one per complete [one-particle state](quantum-field-theory.md#one-particle-state). It also makes a finite model of [fermionic state counting](#fermionic-state-counting) surprisingly simple: two [spatial orbitals](#spatial-orbital) with two [spin](angular-momentum-operator.md#spin) choices each give four complete [one-particle states](quantum-field-theory.md#one-particle-state), and exactly six two-[electron](physics.md#electron) basis states. The following diagram enumerates them; its boxes represent [occupation numbers](quantum-field-theory.md#occupation-number), not locations in space.

<a id="image-six-two-electron-occupation-states-in-two-spatial-orbitals-with-two-spin-projections-each"></a>
![](pauli-spin-orbital-occupancy.png)

**[Figure 1](#image-six-two-electron-occupation-states-in-two-spatial-orbitals-with-two-spin-projections-each). Six two-electron occupation states in two spatial orbitals with two spin projections each**.

Pauli's [Exclusion principle and quantum mechanics by Wolfgang Pauli](physics-bibliography.md#exclusion-principle-and-quantum-mechanics-by-wolfgang-pauli) is his retrospective account, delivered on 13 December 1946 for the 1945 Nobel Prize. On printed pp. 29–30, he describes proposing an extra two-valued [electron](physics.md#electron) property in autumn 1924 and formulating exclusion in 1925. The crucial clue linked counts of resolved [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) in alkali spectra under a [magnetic field](magnetic-field.md) with the populations of closed [electron shells](chemistry.md#electron-shell). Resolving every label turned a complicated shell capacity into one [electron](physics.md#electron) per complete [one-particle state](quantum-field-theory.md#one-particle-state). This historical route preceded the modern [spin](angular-momentum-operator.md#spin) interpretation and the antisymmetric [wavefunction](wave-function.md) formulation; it was not originally a deduction from a [Slater determinant](#slater-determinant).

###### Spin degeneracy in filling a one-dimensional well

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

When [spin](angular-momentum-operator.md#spin) does not split the orbital energies, a fermionic orbital can contain $2s+1$ particles with distinct [spin](angular-momentum-operator.md#spin) projections. Fill these complete states in order of increasing [energy](energy.md) to find a noninteracting many-particle [ground state](quantum-mechanics.md#ground-state). Pauli exclusion does not require different spatial orbitals for particles with different available [spin](angular-momentum-operator.md#spin) states. Imposed [spin](angular-momentum-operator.md#spin) polarization or interactions can change the filling.

###### Balanced two-mode fermion antibunching

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

One identical [fermion](#fermion) in each of two input modes remains one in each output after a lossless two-mode unitary transformation. The fully occupied two-mode state transforms by the [determinant](multilinear-algebra.md#determinant) phase. Pauli exclusion prevents double occupation of either specified mode.

###### Pauli blocking

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

Suppression of a transition when its required final [fermion](#fermion) state is already occupied. In a low-temperature [Fermi gas](quantum-ideal-gas-statistics.md#fermi-gas), an otherwise allowed collision must place outgoing particles in empty states; occupation restricts its available [phase space](hamiltonian-mechanics.md#phase-space). This does not mean that [fermions](#fermion) cease interacting.

###### Spectroscopic origin of the Pauli exclusion principle

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

In 1925, [Wolfgang Pauli](physicist.md#wolfgang-pauli) connected two puzzles: [alkali metal](chemical-substance.md#alkali-metal) doublets and their [anomalous Zeeman effect](atomic-physics.md#anomalous-zeeman-effect), and the capacities of closed [electron shells](chemistry.md#electron-shell). His paper assigned the extra two-valued property to the optically active [electron](physics.md#electron), rather than an angular momentum of the closed core. Its [Paschen-Back effect](atomic-physics.md#paschen-back-effect) classification used four [quantum numbers](quantum-system.md#quantum-number); these historical labels should not be identified literally with modern $n,\ell,m_\ell,m_s$. The exclusion rule forbade matching all four. This connected resolved one-[electron](physics.md#electron) states with closed-group populations. An additional test was the missing triplet counterpart of the equivalent two-$s$-[electron](physics.md#electron) [ground state](quantum-mechanics.md#ground-state) in [alkaline earth metals](chemical-substance.md#alkaline-earth-metal). Pauli explicitly claimed counts of allowed states, not their [energies](energy.md) or ordering.[Pauli 1925, §§1–2: four labels, closed groups, exclusion statement and absent triplet s-term; English translation](https://www.chemteam.info/Chem-History/Pauli-1925/Pauli-1925.html)

The modern question is especially concrete: if a [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) has a lowest [one-particle state](quantum-field-theory.md#one-particle-state), why cannot every [electron](physics.md#electron) occupy it? Minimizing [energy](energy.md) answers which of the allowed [quantum states](quantum-system.md#quantum-state) is preferred; the [Pauli exclusion principle](#pauli-exclusion-principle) determines which [quantum states](quantum-system.md#quantum-state) are allowed in the first place. [Spectral lines](stellar-astrophysics.md#spectral-line) then test [energy](energy.md) differences between allowed [multiparticle quantum states](#multiparticle-quantum-state). A line count is not itself a direct count of occupied [spin orbitals](#spin-orbital): transitions also depend on [selection rules](atomic-physics.md#selection-rule) and the prepared [quantum state populations](density-matrix.md#quantum-state-population). The observed [anomalous Zeeman effect](atomic-physics.md#anomalous-zeeman-effect) supplied constraints for the historical classification; the [two-particle antisymmetrization](#two-particle-antisymmetrization) below supplies the modern mathematical explanation of exclusion.

###### Counting spin orbitals in an electron shell

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

Choose the [one-particle states](quantum-field-theory.md#one-particle-state) of a [hydrogen atom](mathematical-physics.md#hydrogen-atom), or a central-field description of a [chemical atom](physics.md#atom-physics), with labels

$$
n=1,2,\ldots,\qquad \ell=0,1,\ldots,n-1,\qquad m_\ell=-\ell,\ldots,\ell,\qquad m_s=\pm\tfrac12.
$$

The [principal quantum number](mathematical-physics.md#principal-quantum-number) $n$ identifies the [electron shell](chemistry.md#electron-shell). The [orbital angular momentum](quantum-mechanics.md#orbital-angular-momentum) label $\ell$ identifies the [electron subshell](chemistry.md#electron-subshell); the [magnetic quantum number](quantum-mechanics.md#magnetic-quantum-number) $m_\ell$ labels $2\ell+1$ independent [spatial orbitals](#spatial-orbital). Each has two [spin one-half along an axis](angular-momentum-operator.md#spin-one-half-along-an-axis) choices, hence $2(2\ell+1)$ [spin orbitals](#spin-orbital). Applying the [Pauli exclusion principle](#pauli-exclusion-principle) once per [spin orbital](#spin-orbital) gives

$$
N_{\max}(n)=\sum_{\ell=0}^{n-1}2(2\ell+1)=2\left(2\frac{n(n-1)}2+n\right)=2n^2.
$$

These [quantum numbers](quantum-system.md#quantum-number) label [wavefunctions](wave-function.md) and [spin](angular-momentum-operator.md#spin) projections, not [electron](physics.md#electron) trajectories. They need not resolve exact [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) in the presence of [spin-orbit interaction](atomic-physics.md#spin-orbit-interaction); changing to coupled [angular momentum eigenstates](angular-momentum-operator.md#angular-momentum-eigenstate) preserves the count of independent [one-particle states](quantum-field-theory.md#one-particle-state) within this shell model.

<a id="image-counting-complete-spin-orbitals-gives-electron-shell-capacities-2-8-18-32"></a>
![](pauli-shell-capacity-counting.png)

**[Figure 2](#image-counting-complete-spin-orbitals-gives-electron-shell-capacities-2-8-18-32). Counting complete spin orbitals gives electron-shell capacities $2,8,18,32$**. Original counting diagram. The left bars add [electron subshell](chemistry.md#electron-subshell) capacities $2,6,10,14$; the right panel resolves the $n=3$ [electron shell](chemistry.md#electron-shell) into eighteen [spin orbitals](#spin-orbital). Each small cell denotes a label choice, not a region of space.

For example, $n=3$ allows $\ell=0,1,2$, conventionally $3s,3p,3d$. Their [spatial orbital](#spatial-orbital) counts are $1,3,5$; their [spin orbital](#spin-orbital) counts are $2,6,10$. The sum is eighteen. The algebra behind “one per complete state” is short: [two-particle antisymmetrization](#two-particle-antisymmetrization) gives $u\wedge u=(u\otimes u-u\otimes u)/\sqrt2=0$, and the zero [vector](vector-space.md#vector) cannot be a normalized [quantum state](quantum-system.md#quantum-state). Opposite-[spin](angular-momentum-operator.md#spin) [electrons](physics.md#electron) in the same [spatial orbital](#spatial-orbital) have distinct complete states, so their antisymmetric product survives.

This supplies a structural link to the [periodic table](chemical-substance.md#periodic-table): finite [electron subshell](chemistry.md#electron-subshell) capacities make repeated patterns of occupied [electron configurations](chemistry.md#electron-configuration) possible. It does not predict the exact [ground state](quantum-mechanics.md#ground-state) [electron configuration](chemistry.md#electron-configuration) or [energy](energy.md) of a many-[electron](physics.md#electron) [chemical atom](physics.md#atom-physics). Different [electron subshells](chemistry.md#electron-subshell) overlap in [energy](energy.md), and [electron](physics.md#electron) interactions change their ordering. In particular, the [periodic table period](chemical-substance.md#period-periodic-table) lengths are not simply successive $2n^2$ values: the third [periodic table period](chemical-substance.md#period-periodic-table) has eight [chemical elements](chemical-substance.md#chemical-element), although the full $n=3$ [electron shell](chemistry.md#electron-shell) has eighteen available states. A capacity counts available [spin orbitals](#spin-orbital); an actual filling order requires a [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics).

###### Spatial orbital

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

A [spatial orbital](#spatial-orbital) is a normalized spatial [wavefunction](wave-function.md) used in a one-particle description. An [atomic orbital](chemistry.md#atomic-orbital) is the corresponding notion for a [chemical atom](physics.md#atom-physics); a [molecular orbital](chemistry.md#molecular-orbital) belongs to a [molecule](molecule.md). A [spatial orbital](#spatial-orbital) is not a trajectory and does not by itself specify [spin](angular-momentum-operator.md#spin).

###### Spin orbital

↑ **Parent:** [Spatial orbital](#spatial-orbital)

When spatial and [spin](angular-momentum-operator.md#spin) factors separate, a [spin orbital](#spin-orbital) combines a [spatial orbital](#spatial-orbital) $\phi_a$ with a normalized [spin](angular-momentum-operator.md#spin) state $\chi_\sigma$. For an [electron](physics.md#electron), choose [spin one-half along an axis](angular-momentum-operator.md#spin-one-half-along-an-axis) with $\sigma=\uparrow,\downarrow$. The two [spin orbitals](#spin-orbital) $u_{a\uparrow}$ and $u_{a\downarrow}$ are [orthogonal](inner-product.md#orthogonal-vectors) even though their [spatial orbital](#spatial-orbital) is identical, since their [inner product](inner-product.md) contains $\langle\chi_\uparrow|\chi_\downarrow\rangle=0$. When spatial and [spin](angular-momentum-operator.md#spin) variables do not separate, the complete [one-particle state](quantum-field-theory.md#one-particle-state) is instead a multicomponent [wavefunction](wave-function.md) $u(\mathbf r,s)$; exclusion still applies to that complete [quantum state](quantum-system.md#quantum-state).

###### Two-particle antisymmetrization

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

The [particle exchange operator](#particle-exchange-operator) $P_{12}$ swaps the complete particle slots, including [spin](angular-momentum-operator.md#spin). Its antisymmetric [projector](vector-space.md#projection-linear-algebra) is $A_{12}=(I-P_{12})/2$. For [orthonormal](inner-product.md#orthonormal-set) [one-particle states](quantum-field-theory.md#one-particle-state) $u,v$, the normalized [multiparticle quantum state](#multiparticle-quantum-state) is

$$
|u\wedge v\rangle=\frac{|u\rangle\otimes|v\rangle-|v\rangle\otimes|u\rangle}{\sqrt2}.
$$

But attempting the same construction with $v=u$ gives the zero vector:

$$
A_{12}(|u\rangle\otimes|u\rangle)=\frac{|u\rangle\otimes|u\rangle-|u\rangle\otimes|u\rangle}{2}=0.
$$

The zero vector cannot be normalized to a [quantum state](quantum-system.md#quantum-state). This is exclusion as cancellation of [probability amplitudes](wave-function.md#probability-amplitude), rather than a repulsive force. More generally, for normalized $u,v$ the squared [norm](normed-vector-space.md#norm) of the numerator divided by $\sqrt2$ is $1-|\langle u|v\rangle|^2$; the expression has unit [norm](normed-vector-space.md#norm) only when $u,v$ are [orthogonal](inner-product.md#orthogonal-vectors). An overall [quantum phase](quantum-system.md#quantum-phase) difference between $u,v$ describes the same [one-particle state](quantum-field-theory.md#one-particle-state) and also gives zero. Pauli explicitly connects exclusion with a vanishing antisymmetric [wavefunction](wave-function.md).[p. 31, antisymmetric functions with repeated states](physics-bibliography.md#exclusion-principle-and-quantum-mechanics-by-wolfgang-pauli)

<a id="image-antisymmetrization-removes-equal-state-pairs-and-pairs-the-twelve-remaining-ordered-products-into-six-fermionic-basis-states"></a>
![](pauli-antisymmetric-state-pairs.png)

**[Figure 3](#image-antisymmetrization-removes-equal-state-pairs-and-pairs-the-twelve-remaining-ordered-products-into-six-fermionic-basis-states). Antisymmetrization removes equal-state pairs and pairs the twelve remaining ordered products into six fermionic basis states**.

###### Slater determinant

↑ **Parent:** [Two-particle antisymmetrization](#two-particle-antisymmetrization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slater_determinant)

A [Slater determinant](#slater-determinant) extends [two-particle antisymmetrization](#two-particle-antisymmetrization) to $N$ [fermions](#fermion). Here $x_i$ contains position and [spin](angular-momentum-operator.md#spin) or other internal variables. Distinct [orthonormal](inner-product.md#orthonormal-set) [one-particle states](quantum-field-theory.md#one-particle-state) give the normalized [wavefunction](wave-function.md) displayed in the title. Repeating a [one-particle state](quantum-field-theory.md#one-particle-state) repeats a column of the [determinant](multilinear-algebra.md#determinant), so the [wavefunction](wave-function.md) vanishes. Exchanging particle slots exchanges rows and reverses its sign. A general [fermionic](#fermion) [quantum state](quantum-system.md#quantum-state) can be a [quantum superposition](quantum-system.md#quantum-superposition) of [Slater determinants](#slater-determinant); it need not be one [Slater determinant](#slater-determinant).

###### Slater-Condon rules

↑ **Parent:** [Slater determinant](#slater-determinant)

Rules expressing Hamiltonian matrix elements between [Slater determinants](#slater-determinant) through one- and two-electron orbital integrals. A two-body Hamiltonian cannot connect determinants differing in more than two spin-orbitals.

###### Exclusion versus particle position

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

Exclusion constrains complete [one-particle states](quantum-field-theory.md#one-particle-state), not a collection of little spatial boxes. In particular, two opposite-[spin](angular-momentum-operator.md#spin) [electrons](physics.md#electron) in the same [spatial orbital](#spatial-orbital) have

$$
\Psi(\mathbf r_1,s_1;\mathbf r_2,s_2)=\phi_a(\mathbf r_1)\phi_a(\mathbf r_2)\frac{\chi_\uparrow(s_1)\chi_\downarrow(s_2)-\chi_\downarrow(s_1)\chi_\uparrow(s_2)}{\sqrt2}.
$$

The spatial factor is symmetric; the [spin-one-half singlet state](angular-momentum-operator.md#spin-one-half-singlet-state) supplies the required antisymmetry. At $\mathbf r_1=\mathbf r_2$, this [wavefunction](wave-function.md) need not vanish for opposite [spin](angular-momentum-operator.md#spin) labels. For equal [spin](angular-momentum-operator.md#spin) labels it does vanish. In a continuous position description, an exact coincident point has zero measure anyway; the useful comparison concerns joint [probability densities](wave-function.md#probability-density) or detection in finite regions. Equal positions do not imply equal complete [quantum states](quantum-system.md#quantum-state).

The [fermionic occupation numbers](quantum-field-theory.md#fermionic-occupation-number) $n_\alpha=0,1$ refer to a chosen [orthonormal basis](inner-product.md#orthonormal-basis) of [one-particle states](quantum-field-theory.md#one-particle-state). A [quantum superposition](quantum-system.md#quantum-superposition) need not have definite [occupation numbers](quantum-field-theory.md#occupation-number) in that basis, and an [expectation value](quantum-system.md#expectation-value) $\langle n_\alpha\rangle$ can be fractional. For example, one [electron](physics.md#electron) in $(u+v)/\sqrt2$ has mean [occupation number](quantum-field-theory.md#occupation-number) $1/2$ in each of two [orthogonal](inner-product.md#orthogonal-vectors) [spin orbitals](#spin-orbital), without splitting into two particles. The [canonical anticommutation relations](supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations) give $(a_\alpha^\dagger)^2=0$ and make $a_\alpha^\dagger a_\alpha$ a [projector](vector-space.md#projection-linear-algebra), so its [expectation value](quantum-system.md#expectation-value) stays between zero and one in every normalized [quantum state](quantum-system.md#quantum-state).

###### Zero-temperature filling of finite fermion levels

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

For $M$ complete [energy eigenstates](energy-eigenvalue.md#energy-eigenstate) of a one-particle [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) for identical noninteracting [fermions](#fermion), order their energies $\epsilon_1\le\cdots\le\epsilon_M$. At fixed particle number $0\le N\le M$, the [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) and the particle-number constraint are

$$
H=\sum_{\alpha=1}^M\epsilon_\alpha n_\alpha,\qquad \sum_{\alpha=1}^Mn_\alpha=N,\qquad n_\alpha\in\{0,1\}.
$$

The [ground state](quantum-mechanics.md#ground-state) occupies the $N$ lowest complete [one-particle states](quantum-field-theory.md#one-particle-state). A short minimization argument suffices: moving an occupant from a higher energy to an empty lower energy decreases the total energy. This filling describes the [ground state](quantum-mechanics.md#ground-state) at [temperature](temperature.md) $T=0$; exclusion by itself also applies to excited [quantum states](quantum-system.md#quantum-state) and at positive [temperature](temperature.md). The underlying thermal description is the [Fermi-Dirac distribution](quantum-ideal-gas-statistics.md#fermi-dirac-distribution).[Sections 3.6–3.6.2, occupation restriction, spin multiplicity and zero-temperature filling](physics-bibliography.md#statistical-physics-by-david-tong/3-quantum-gases)

If the last occupied energy belongs to a group of $g$ [one-particle states](quantum-field-theory.md#one-particle-state) at the same energy and $q$ of them must be occupied, with all lower states filled, the [ground state](quantum-mechanics.md#ground-state) subspace has [dimension](vector-space.md#dimension-vector-space) $\binom gq$. Exclusion does not select a particular [basis](vector-space.md#basis) or a particular [quantum superposition](quantum-system.md#quantum-superposition) in that subspace. The factor of two for an [electron](physics.md#electron) [spatial orbital](#spatial-orbital) assumes both [spin](angular-momentum-operator.md#spin) projections are included; a model restricted to one [spin](angular-momentum-operator.md#spin) projection has only one state per [spatial orbital](#spatial-orbital). A [magnetic field](magnetic-field.md) can split the [degenerate energy levels](quantum-mechanics.md#degenerate-energy-levels), and interactions can change the lowest-energy [electron configuration](chemistry.md#electron-configuration). Thus this finite noninteracting filling rule is not a complete prescription for interacting [chemical atoms](physics.md#atom-physics).

###### Fermionic state counting

↑ **Parent:** [Zero-temperature filling of finite fermion levels](#zero-temperature-filling-of-finite-fermion-levels)

Choosing $N$ different complete [one-particle states](quantum-field-theory.md#one-particle-state) from an [orthonormal basis](inner-product.md#orthonormal-basis) of size $M$ gives $\binom MN$ independent [Slater determinants](#slater-determinant). This is the [binomial coefficient](binomial-coefficient.md) because only the occupied subset matters: permutations change the sign of the [Slater determinant](#slater-determinant), not the physical [quantum state](quantum-system.md#quantum-state). Summing over particle numbers gives $2^M$ states in the finite [fermionic Fock space](supersymmetric-quantum-mechanics.md#fermionic-fock-space).

For the diagram's two [spatial orbitals](#spatial-orbital) $A,B$, take energies $0,\Delta$ with $\Delta>0$, each independent of [spin](angular-momentum-operator.md#spin). In the complete-state order $(A\uparrow,A\downarrow,B\uparrow,B\downarrow)$, the six $N=2$ [occupation number](quantum-field-theory.md#occupation-number) strings are $1100,1010,1001,0110,0101,0011$. Their total energies are $0,\Delta,\Delta,\Delta,\Delta,2\Delta$, giving energy multiplicities $1,4,1$. For $N=3$, the [ground state](quantum-mechanics.md#ground-state) energy is $\Delta$ with two independent [ground states](quantum-mechanics.md#ground-state), according to which [spin orbital](#spin-orbital) in $B$ is occupied. Across $N=0,1,2,3,4$, the counts are $1,4,6,4,1$, summing to $16$. These are exact counts for this model, not measured atomic energies.

###### Exclusion and the energy of two electrons in three spatial levels

↑ **Parent:** [Zero-temperature filling of finite fermion levels](#zero-temperature-filling-of-finite-fermion-levels)

Consider an original noninteracting model with three [orthonormal](inner-product.md#orthonormal-set) [spatial orbitals](#spatial-orbital) $A,B,C$ at [energies](energy.md) $0,\Delta,3\Delta$, where $\Delta>0$. Both [spin](angular-momentum-operator.md#spin) projections are available at each [energy](energy.md), so there are six [spin orbitals](#spin-orbital). The [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) is $H=h\otimes I+I\otimes h$, with no interaction between particles and no dependence on [spin](angular-momentum-operator.md#spin). Comparing its allowed [ground states](quantum-mechanics.md#ground-state) isolates the effect of [fermionic](#fermion) exchange symmetry.

For two distinguishable spin-one-half particles, the spatial [ground state](quantum-mechanics.md#ground-state) is $A\otimes A$ and any of four independent two-[spin](angular-momentum-operator.md#spin) states is possible: $E_0=0$ and [ground-state degeneracy](quantum-mechanics.md#ground-state-degeneracy) four. For two identical [electrons](physics.md#electron), both can still occupy $A$, using $A\uparrow$ and $A\downarrow$, but there is just one allowed [ground state](quantum-mechanics.md#ground-state): the symmetric spatial factor times the [spin-one-half singlet state](angular-momentum-operator.md#spin-one-half-singlet-state),

$$
\Psi_0=A(\mathbf r_1)A(\mathbf r_2)\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2},\qquad E_0=0.
$$

Exclusion has reduced the [ground-state degeneracy](quantum-mechanics.md#ground-state-degeneracy) without raising the [ground state](quantum-mechanics.md#ground-state) [energy](energy.md).

Now restrict both particles to the same [spin](angular-momentum-operator.md#spin) projection $\uparrow$. Distinguishable particles can still both occupy $A\uparrow$, so $E_0=0$. Identical [electrons](physics.md#electron) must occupy different [spatial orbitals](#spatial-orbital); the lowest choice is $A,B$, with

$$
\Psi_{\uparrow\uparrow}=\frac{A(\mathbf r_1)B(\mathbf r_2)-B(\mathbf r_1)A(\mathbf r_2)}{\sqrt2}|\uparrow\uparrow\rangle,\qquad E_0=\Delta.
$$

The [spin](angular-momentum-operator.md#spin) factor is a [spin-one-half triplet state](angular-momentum-operator.md#spin-one-half-triplet-state), and the spatial factor is antisymmetric. These are [ground states](quantum-mechanics.md#ground-state) within the restricted parallel-[spin](angular-momentum-operator.md#spin) sector, not the unrestricted two-[electron](physics.md#electron) [ground state](quantum-mechanics.md#ground-state). Both restricted models have [ground-state degeneracy](quantum-mechanics.md#ground-state-degeneracy) one.

<a id="image-ground-energies-in-a-three-spatial-level-model-depend-on-which-spin-states-are-available"></a>
![](pauli-three-level-ground-energy.png)

**[Figure 4](#image-ground-energies-in-a-three-spatial-level-model-depend-on-which-spin-states-are-available). Ground energies in a three-spatial-level model depend on which spin states are available**. Original model with chosen [spatial orbital](#spatial-orbital) [energies](energy.md) $0,\Delta,3\Delta$, no interactions and no [spin](angular-momentum-operator.md#spin) splitting. The first pair of panels allows both [spin](angular-momentum-operator.md#spin) projections; the second pair restricts both to $\uparrow$. Labels $g_0$ count independent [ground states](quantum-mechanics.md#ground-state); particle subscripts appear only in the distinguishable cases.

The first excited two-[electron](physics.md#electron) [energy](energy.md) in the unrestricted model is $\Delta$, with four independent [quantum states](quantum-system.md#quantum-state): one occupant in $A$, one in $B$, and two [spin](angular-momentum-operator.md#spin) choices for each. A basis adapted to [particle exchange operators](#particle-exchange-operator) separates these into one [spin-one-half singlet state](angular-momentum-operator.md#spin-one-half-singlet-state) with symmetric spatial factor and three [spin-one-half triplet states](angular-momentum-operator.md#spin-one-half-triplet-state) with antisymmetric spatial factor. All four have equal [energy](energy.md) in this model. Singlet versus triplet does not by itself determine an [energy](energy.md) gap; an interaction or a [spin](angular-momentum-operator.md#spin)-dependent term is needed to split them.

As a further count, the full two-[electron](physics.md#electron) space has [dimension](vector-space.md#dimension-vector-space) $\binom62=15$. Its [energies](energy.md) in units of $\Delta$ and corresponding multiplicities are $(0,1,2,3,4,6)$ and $(1,4,1,4,4,1)$. For distinguishable spin-one-half particles the ordered [tensor product](multilinear-algebra.md#tensor-product) instead has [dimension](vector-space.md#dimension-vector-space) $6^2=36$, with multiplicities $(4,8,4,8,8,4)$ at those same [energies](energy.md). These are exact model counts, not atomic measurements. The higher restricted [ground state](quantum-mechanics.md#ground-state) [energy](energy.md) follows from removing forbidden [quantum states](quantum-system.md#quantum-state); the [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) contains no additional “exclusion force”.

###### Fermionic atom antibunching

↑ **Parent:** [Pauli exclusion principle](#pauli-exclusion-principle)

The 2007 paper [Comparison of the Hanbury Brown-Twiss effect for bosons and fermions by T. Jeltes and others](physics-bibliography.md#comparison-of-the-hanbury-brown-twiss-effect-for-bosons-and-fermions-by-t-jeltes-and-others) compares polarized [helium-3](chemical-substance.md#helium-3) [fermions](#fermion) with [helium-4](chemical-substance.md#helium-4) [bosons](#boson). The [chemical atoms](physics.md#atom-physics) occupy a [metastable atomic level](atomic-physics.md#metastable-atomic-level). Switching off [magnetic trapping of neutral atoms](#magnetic-trapping-of-neutral-atoms) releases them onto a [microchannel plate detector](#microchannel-plate-detector) with a delay-line anode, 63 cm below. Position and arrival-time readouts give three-dimensional pair separations by [time-of-flight atom detection](#time-of-flight-atom-detection). About 1000 clouds per [isotope](chemical-substance.md#isotope) supply [histograms](probability-and-statistics.md#histogram); normalization removes the broad cloud shape.

The [pair detection correlation](#pair-detection-correlation) dips below one for [helium-3](chemical-substance.md#helium-3) and rises above one for [helium-4](chemical-substance.md#helium-4). The same apparatus, matched [temperatures](temperature.md) near $0.5\,\mu\mathrm K$, nearly identical trapping potentials, negligible interactions, and [magnetic field](magnetic-field.md) gradient checks of [spin](angular-momentum-operator.md#spin) polarization support an exchange-statistics interpretation. Finite detector resolution suppresses contrast; trap switch-off and resolution uncertainties limit quantitative agreement. A diverging [laser](laser.md) lens deepens the dip, but its aberrations preclude a precise lens-model test. This detects exchange correlations, rather than measuring occupation of one selected [spin orbital](#spin-orbital).[pp. 3–7, Methods, Figs. 1–3; supplementary pp. 14–16](physics-bibliography.md#comparison-of-the-hanbury-brown-twiss-effect-for-bosons-and-fermions-by-t-jeltes-and-others)

###### Pair detection correlation

↑ **Parent:** [Fermionic atom antibunching](#fermionic-atom-antibunching)

The [pair detection correlation](#pair-detection-correlation) divides joint detection probability by the product of single detection probabilities. The baseline $g^{(2)}=1$ means independent detection; $g^{(2)}<1$ means suppressed pairs. Its value depends on the prepared [quantum state](quantum-system.md#quantum-state) and detector resolution, so exclusion alone does not require every experimental curve to reach zero.

###### Magnetic trapping of neutral atoms

↑ **Parent:** [Fermionic atom antibunching](#fermionic-atom-antibunching)

###### Time-of-flight atom detection

↑ **Parent:** [Fermionic atom antibunching](#fermionic-atom-antibunching)

###### Microchannel plate detector

↑ **Parent:** [Time-of-flight atom detection](#time-of-flight-atom-detection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Microchannel_plate_detector)

The experiment above combines a [microchannel plate detector](#microchannel-plate-detector) with a delay-line anode to record individual atom arrivals. The apparatus is described in the paper's Fig. 1 and Methods.

##### Spin-statistics theorem

↑ **Parent:** [Indistinguishable particles](#indistinguishable-particles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin-statistics_theorem)

The spin-statistics theorem associates integer-spin particles with bosonic exchange symmetry and half-integer-spin particles with fermionic exchange symmetry in relativistic quantum field theory under the standard locality and positivity assumptions.

###### Vector decay into identical spin-zero mesons

↑ **Parent:** [Spin-statistics theorem](#spin-statistics-theorem)

A spin-one parent cannot decay into two identical spin-zero particles in the same internal state while preserving rotational [symmetry](physics.md#symmetry-physics) and Bose exchange [symmetry](physics.md#symmetry-physics). Their final total [angular momentum](momentum.md#angular-momentum) is orbital $L=1$, which is antisymmetric under interchange. Bose [symmetry](physics.md#symmetry-physics) requires even $L$ instead. An energetically allowed decay with matching [parity](quantum-mechanics.md#parity) can therefore remain forbidden independently of the interaction's coupling strength.

###### Nuclear spin statistics

↑ **Parent:** [Spin-statistics theorem](#spin-statistics-theorem)

Restrictions linking the exchange symmetry of nuclear spin and spatial wavefunctions. For identical nuclei, the total wavefunction must be antisymmetric for fermions and symmetric for bosons. Electronic and vibrational exchange parity must be included before assigning rotational parity.

###### Composite statistics of neutral atoms

↑ **Parent:** [Spin-statistics theorem](#spin-statistics-theorem)

Exchanging two identical bound atoms exchanges their constituent [fermions](#fermion). An atom with mass number $A$ and atomic number $Z$ contains $A$ nucleons and $Z$ electrons, so its exchange sign is $(-1)^{A+Z}$ when its internal state is preserved. An odd count gives a composite [fermion](#fermion); an even count gives a composite [boson](#boson). This is equivalently the integer-versus-half-integer total-spin distinction in the [Spin-statistics theorem](#spin-statistics-theorem). For example, neutral lithium-6 has nine fermionic constituents and is a fermion, while neutral lithium-7 has ten and is a boson. Counting nucleons alone instead classifies the nucleus, not the neutral atom. This effective composite-particle description requires energies and separations where the bound atom remains intact.

##### Two identical spin-one bosons

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

## Decoupled Fermi oscillators

↑ **Parent:** [Tensor product of quantum systems](tensor-product-of-quantum-systems.md)

Two decoupled Fermi oscillators have product occupation states and additive energies $E_1n_1+E_2n_2$.

## Kronecker product representation of local operators

↑ **Parent:** [Tensor product of quantum systems](tensor-product-of-quantum-systems.md)

In a product basis, an operator local to one subsystem is represented by its matrix Kronecker the identity on every other subsystem.

## Decoupled commuting Hamiltonian terms

↑ **Parent:** [Tensor product of quantum systems](tensor-product-of-quantum-systems.md)

Commuting Hamiltonian terms on separate factors are simultaneously diagonalized by tensor products of their eigenvectors and have additive eigenvalues.

## ↑ Ancestors (4)

1. [Quantum mechanics](quantum-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#32b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325.md#1/solution)
- [Trapped-ion internal and motional states](atomic-physics.md#trapped-ion-internal-and-motional-states)
