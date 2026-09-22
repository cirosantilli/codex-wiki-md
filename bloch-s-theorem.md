# Bloch's theorem

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bloch's_theorem)

In a periodic potential, energy eigenstates have the form $e^{ik\cdot x}u_k(x)$ with lattice-periodic $u_k$.

**Table of contents**

- [State counting in a Bloch band](#state-counting-in-a-bloch-band)
- [Inversion symmetry](#inversion-symmetry)
- [Bloch Hamiltonian](#bloch-hamiltonian)
  - [Momentum matrix-element expansion of band energy](#momentum-matrix-element-expansion-of-band-energy)
- [Particle in a one-dimensional lattice](#particle-in-a-one-dimensional-lattice)
  - [Kronig-Penney model](#kronig-penney-model)
    - [Band edges of a repulsive delta-comb potential](#band-edges-of-a-repulsive-delta-comb-potential)
    - [Floquet discriminant of the delta-comb Kronig-Penney model](#floquet-discriminant-of-the-delta-comb-kronig-penney-model)
    - [Attractive delta-comb Kronig-Penney model](#attractive-delta-comb-kronig-penney-model)
      - [Negative-energy band of an attractive delta comb](#negative-energy-band-of-an-attractive-delta-comb)
    - [Scattering-amplitude equations for one-dimensional band edges](#scattering-amplitude-equations-for-one-dimensional-band-edges)
- [Electronic band structure](#electronic-band-structure)
  - [k·p perturbation theory](#k·p-perturbation-theory)
  - [Parabolic band dispersion](#parabolic-band-dispersion)
  - [Interband transition](#interband-transition)
    - [Indirect optical transition](#indirect-optical-transition)
    - [Direct optical transition](#direct-optical-transition)
      - [Parabolic-band optical energy sharing](#parabolic-band-optical-energy-sharing)
    - [Interband absorption](#interband-absorption)
  - [Superlattice](#superlattice)
  - [Flat band](#flat-band)
  - [Band hybridization](#band-hybridization)
    - [Flat-band hybridization Fermi-velocity suppression](#flat-band-hybridization-fermi-velocity-suppression)
    - [Fermi-volume conservation in two hybridized electron bands](#fermi-volume-conservation-in-two-hybridized-electron-bands)
    - [Hybridization gap](#hybridization-gap)
  - [Mott insulator](#mott-insulator)
  - [Energy band](#energy-band)
    - [Energy-band width](#energy-band-width)
    - [Electronic bandwidth](#electronic-bandwidth)
    - [Dirac cone](#dirac-cone)
      - [Dirac valley](#dirac-valley)
      - [Dirac point](#dirac-point)
    - [Electronic valley](#electronic-valley)
    - [Impurity level in a crystal](#impurity-level-in-a-crystal)
      - [Occupation of an interacting localized electron level](#occupation-of-an-interacting-localized-electron-level)
    - [Band effective mass](#band-effective-mass)
      - [Hole mass from a valence-band maximum](#hole-mass-from-a-valence-band-maximum)
      - [Effective mass for overlap-weighted exponential hopping](#effective-mass-for-overlap-weighted-exponential-hopping)
      - [Effective-mass tensor](#effective-mass-tensor)
      - [Band-edge effective mass in a weak periodic potential](#band-edge-effective-mass-in-a-weak-periodic-potential)
      - [Band curvature](#band-curvature)
      - [Effective mass for exponentially decaying tight-binding hopping](#effective-mass-for-exponentially-decaying-tight-binding-hopping)
    - [Cyclotron effective mass](#cyclotron-effective-mass)
    - [Shubnikov-de Haas effect](#shubnikov-de-haas-effect)
      - [Thermal damping of quantum oscillations](#thermal-damping-of-quantum-oscillations)
      - [Dingle factor](#dingle-factor)
    - [Allowed energy band](#allowed-energy-band)
    - [Band gap](#band-gap)
      - [Positive direct gaps can coexist with band overlap](#positive-direct-gaps-can-coexist-with-band-overlap)
      - [Indirect band gap](#indirect-band-gap)
        - [Indirect gap of a separable square cosine potential](#indirect-gap-of-a-separable-square-cosine-potential)
      - [Direct band gap](#direct-band-gap)
      - [Avoided crossing](#avoided-crossing)
    - [Band filling](#band-filling)
      - [Carrier compensation and even band filling in a square lattice](#carrier-compensation-and-even-band-filling-in-a-square-lattice)
        - [Translation-symmetry breaking changes the band-filling constraint](#translation-symmetry-breaking-changes-the-band-filling-constraint)
      - [Band insulator](#band-insulator)
        - [Odd filling obstructs a spin-degenerate band insulator](#odd-filling-obstructs-a-spin-degenerate-band-insulator)
        - [Kondo insulator](#kondo-insulator)
        - [Overlapping energy bands prevent a band insulator](#overlapping-energy-bands-prevent-a-band-insulator)
          - [Indirect gap in a uniformly split zone-boundary model](#indirect-gap-in-a-uniformly-split-zone-boundary-model)
- [Bloch oscillation](#bloch-oscillation)
  - [Excursion amplitude of a Bloch-oscillating wavepacket](#excursion-amplitude-of-a-bloch-oscillating-wavepacket)
  - [Cold-atom Bloch oscillation experiment](#cold-atom-bloch-oscillation-experiment)
- [Translation-character proof of Bloch theorem](#translation-character-proof-of-bloch-theorem)
- [Bloch state](#bloch-state)
  - [Crystal momentum](#crystal-momentum)
- [Periodic potential](#periodic-potential)
- [Nearly-free electron model](#nearly-free-electron-model)
  - [Monovalent BCC direct optical threshold](#monovalent-bcc-direct-optical-threshold)
  - [Zone-face two-plane-wave gap for a cosine potential](#zone-face-two-plane-wave-gap-for-a-cosine-potential)
    - [Four-plane-wave splitting at a square-zone corner](#four-plane-wave-splitting-at-a-square-zone-corner)
  - [Rectangular-lattice Fermi-surface reconstruction](#rectangular-lattice-fermi-surface-reconstruction)
    - [Two-wave estimate of a Bragg-gap coupling from a pocket area](#two-wave-estimate-of-a-bragg-gap-coupling-from-a-pocket-area)
    - [Lens bound on a reconstructed Fermi pocket](#lens-bound-on-a-reconstructed-fermi-pocket)
  - [Bragg gap ladder for a linear dispersion](#bragg-gap-ladder-for-a-linear-dispersion)
  - [Nearly-free electron dispersion near a one-dimensional band gap](#nearly-free-electron-dispersion-near-a-one-dimensional-band-gap)
- [Floquet matrix for a one-dimensional periodic potential](#floquet-matrix-for-a-one-dimensional-periodic-potential)
  - [Floquet discriminant and energy bands](#floquet-discriminant-and-energy-bands)
- [Tight binding](#tight-binding)
  - [Opposite sigma and pi hopping signs in a p-orbital chain](#opposite-sigma-and-pi-hopping-signs-in-a-p-orbital-chain)
  - [s-p mixing in a one-dimensional tight-binding chain](#s-p-mixing-in-a-one-dimensional-tight-binding-chain)
  - [Orbital phase and the sign of one-dimensional hopping](#orbital-phase-and-the-sign-of-one-dimensional-hopping)
  - [Filling fraction of an independent cosine band](#filling-fraction-of-an-independent-cosine-band)
  - [Three-site tight-binding ring](#three-site-tight-binding-ring)
  - [Nonorthogonal nearest-neighbour tight-binding band](#nonorthogonal-nearest-neighbour-tight-binding-band)
  - [Orthogonal tight-binding approximation](#orthogonal-tight-binding-approximation)
    - [Simple-cubic nearest-neighbour tight-binding band](#simple-cubic-nearest-neighbour-tight-binding-band)
  - [Hopping integral](#hopping-integral)
    - [Projected hopping matrix element and sign convention](#projected-hopping-matrix-element-and-sign-convention)
  - [Pseudospin](#pseudospin)
  - [Dilute-hopping lattice propagator](#dilute-hopping-lattice-propagator)
  - [Harmonic approximation near a potential minimum](#harmonic-approximation-near-a-potential-minimum)
  - [Finite periodic tight-binding ring](#finite-periodic-tight-binding-ring)
  - [Two-direction nearest-neighbour tight-binding dispersion](#two-direction-nearest-neighbour-tight-binding-dispersion)
- [Brillouin zone](#brillouin-zone)
  - [Gamma point](#gamma-point)
  - [Reduced Brillouin zone](#reduced-brillouin-zone)
  - [Second Brillouin zone](#second-brillouin-zone)
  - [First Brillouin zone](#first-brillouin-zone)
  - [Zone folding in an equal-mass diatomic chain](#zone-folding-in-an-equal-mass-diatomic-chain)
  - [Bragg point](#bragg-point)
  - [Brillouin zone of a two-dimensional triangular lattice](#brillouin-zone-of-a-two-dimensional-triangular-lattice)

## State counting in a Bloch band

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)

A crystal with $N$ [primitive unit cells](quantum-scattering.md#primitive-unit-cell) has $N$ distinct [wavevectors](elasticity-physics.md#wavevector) in one [Brillouin zone](#brillouin-zone). For a rectangular periodic sample, $k_i=2\pi l_i/L_i$, and the product of the numbers of allowed values along the three directions equals the number of cells. Each orbital-derived [energy band](#energy-band) therefore holds $N$ states per [spin](angular-momentum-operator.md#spin) orientation, or $2N$ with twofold spin degeneracy. This means two states per primitive cell per spin-degenerate band, independently of how many atoms the cell contains.

## Inversion symmetry

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)

Invariance under spatial inversion about a specified origin.

## Bloch Hamiltonian

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)

The [Quantum Hamiltonian](quantum-system.md#hamiltonian-quantum-mechanics) acting on the cell-periodic part of a [Bloch state](#bloch-state) at fixed [wave vector](elasticity-physics.md#wavevector).

### Momentum matrix-element expansion of band energy

↑ **Parent:** [Bloch Hamiltonian](#bloch-hamiltonian)

For a real scalar lattice-periodic potential, let $|n\rangle$ be a nondegenerate zone-centre periodic eigenstate with energy $E_n$. Conjugation by $e^{i\mathbf k\cdot\mathbf r}$ gives $H(\mathbf k)=H(0)+\hbar\mathbf k\cdot\mathbf p/m+\hbar^2k^2/(2m)$. The zone-centre state can be chosen real, so $\langle n|\mathbf p|n\rangle=0$. [Second-order nondegenerate perturbation theory](quantum-mechanics.md#second-order-nondegenerate-perturbation-theory) then gives

$$
E_n(\mathbf k)=E_n+\frac{\hbar^2k^2}{2m}+\frac{\hbar^2}{m^2}\sum_{l\ne n}\frac{|\langle n|\mathbf k\cdot\mathbf p|l\rangle|^2}{E_n-E_l}+O(|\mathbf k|^4).
$$

Time-reversal symmetry makes this isolated spinless band even in $\mathbf k$. In a direction $\mathbf e$, the curvature gives

$$
\frac{m}{m^*_{\mathbf e}}=1+\frac2m\sum_{l\ne n}\frac{|\langle n|\mathbf e\cdot\mathbf p|l\rangle|^2}{E_n-E_l}.
$$

A degeneracy requires a matrix treatment before extracting curvatures; a nonlocal potential or spin-orbit terms can also alter the simple momentum vertex.

## Particle in a one-dimensional lattice

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Particle_in_a_one-dimensional_lattice)

A quantum particle in a one-dimensional lattice experiences a periodic potential. Bloch states organize its spectrum into bands and gaps; the [Kronig-Penney model](#kronig-penney-model) realizes this behavior with an idealized array of barriers or narrow delta barriers.

### Kronig-Penney model

↑ **Parent:** [Particle in a one-dimensional lattice](#particle-in-a-one-dimensional-lattice)

The delta-comb Kronig-Penney potential is

$$
V(x)=V_0\sum_{n\in\mathbb Z}\delta(x-na).
$$

#### Band edges of a repulsive delta-comb potential

↑ **Parent:** [Kronig-Penney model](#kronig-penney-model)

For $V(x)=\alpha\sum_j\delta(x-ja)$ with $\alpha>0$, put $P=m\alpha a/\hbar^2$ and $x=ka$. The [Floquet discriminant of the delta-comb Kronig-Penney model](#floquet-discriminant-of-the-delta-comb-kronig-penney-model) is $f(x)=\cos x+P\sin x/x$. Extended [Bloch states](#bloch-state) require $|f(x)|\leq1$. Since $f(0)=1+P>1$, there is a positive lower band edge; a repulsive potential does not support negative-energy states in this energy convention.

The $j$th positive-energy band ends at $x=j\pi$. Its lower edge lies in $((j-1)\pi,j\pi)$ and solves $f(x)=(-1)^{j-1}$. A finite periodic ring selects only the discrete allowed values of [crystal momentum](#crystal-momentum) within these bands. Nonzero [band gaps](#band-gap) do not by themselves imply an insulator: the [band filling](#band-filling) must also place the [Fermi energy](quantum-ideal-gas-statistics.md#fermi-energy) in a gap.

#### Floquet discriminant of the delta-comb Kronig-Penney model

↑ **Parent:** [Kronig-Penney model](#kronig-penney-model)

For $E=\hbar^2k^2/(2m)$ and $\gamma=mV_0/(\hbar^2k)$,

$$
\frac12\operatorname{tr}M(E)
=\cos(ka)+\gamma\sin(ka).
$$

Thus the allowed bands satisfy $|\cos(ka)+\gamma\sin(ka)|\leq1$.

#### Attractive delta-comb Kronig-Penney model

↑ **Parent:** [Kronig-Penney model](#kronig-penney-model)

For

$$
V(x)=-\frac{\hbar^2\lambda}{m}\sum_{n\in\mathbb Z}\delta(x-na),
$$

the [wavefunction](wave-function.md) is continuous across every lattice point and obeys

$$
\psi'(na^+)-\psi'(na^-)=-2\lambda\psi(na).
$$

At negative energy $E=-\hbar^2\mu^2/(2m)$, an [allowed energy band](#allowed-energy-band) satisfies

$$
\boxed{\lambda\tanh\frac{\mu a}{2}<\mu<\lambda\coth\frac{\mu a}{2}.}
$$

At positive energy $E=\hbar^2k^2/(2m)$, it satisfies

$$
\boxed{\left|\cos(ka)-\frac\lambda k\sin(ka)\right|<1.}
$$

##### Negative-energy band of an attractive delta comb

↑ **Parent:** [Attractive delta-comb Kronig-Penney model](#attractive-delta-comb-kronig-penney-model)

With well strength $\lambda$ and spacing $a$, negative-energy Bloch states obey $\tanh y\leq2y/(\lambda a)\leq\coth y$, where $y=\kappa a/2$. There is one negative band: it reaches zero when $\lambda a\leq2$ and is separated from zero when $\lambda a>2$.

#### Scattering-amplitude equations for one-dimensional band edges

↑ **Parent:** [Kronig-Penney model](#kronig-penney-model)

If one symmetric cell has reflection and transmission amplitudes $r,t$, then

$$
\operatorname{tr}M
=\frac{(t^2-r^2)e^{ika}+e^{-ika}}t.
$$

At a periodic or antiperiodic band edge, with $\operatorname{tr}M=2\sigma$ and $\sigma=\pm1$, setting $z=e^{-ika}$ gives

$$
z^2-2\sigma tz+t^2-r^2=0,
\qquad
z=\sigma t\pm r.
$$

## Electronic band structure

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electronic_band_structure)

Electronic band structure is the collection of allowed electron energy bands and gaps in a periodic medium, usually represented as energy versus crystal momentum. An [energy band](#energy-band) is one branch of that structure.

### k·p perturbation theory

↑ **Parent:** [Electronic band structure](#electronic-band-structure)

For a local periodic scalar potential, writing a Bloch wave as $e^{i\mathbf k\cdot\mathbf r}u_{n\mathbf k}$ gives the displayed cell-periodic Hamiltonian before additional spin-orbit terms. Momentum matrix elements mix zone-centre bands when k is varied. Perturbatively eliminating remote bands changes the [effective mass](#band-effective-mass); a multiband retained subspace describes degeneracy, nonparabolicity and coupled hole bands. Spin-orbit coupling and the chosen reference wavevector must be included consistently.

### Parabolic band dispersion

↑ **Parent:** [Electronic band structure](#electronic-band-structure)

An approximation $E(k)=E_0+\hbar^2k^2/(2m^*)$ defining an [effective mass](#band-effective-mass) near a band extremum. A fitted positive curvature gives positive [effective mass](#band-effective-mass).

### Interband transition

↑ **Parent:** [Electronic band structure](#electronic-band-structure)

An [interband transition](#interband-transition) moves an [electron](physics.md#electron) between distinct [energy bands](#energy-band). A direct optical transition approximately conserves [crystal momentum](#crystal-momentum) because optical [photon](quantum-mechanics.md#photon) momentum is small compared with a [reciprocal lattice](quantum-scattering.md#reciprocal-lattice) vector. A phonon-assisted transition can supply the momentum difference needed near an [indirect band gap](#indirect-band-gap). Transition energies alone do not fix their optical intensities, which also depend on [matrix elements](vector-space.md#matrix-element) and occupations.

#### Indirect optical transition

↑ **Parent:** [Interband transition](#interband-transition)

An optical [interband transition](#interband-transition) that requires another momentum source, commonly a phonon, to connect initial and final electronic wavevectors. Near an [indirect band gap](#indirect-band-gap), phonon emission gives a threshold photon energy $E_g+\hbar\Omega$, while phonon absorption gives $E_g-\hbar\Omega$ and requires an occupied phonon mode. The temperature dependence of the absorption therefore contains phonon-population information in addition to electronic occupations.

#### Direct optical transition

↑ **Parent:** [Interband transition](#interband-transition)

A photon-induced [interband transition](#interband-transition) that approximately preserves the electron's crystal wavevector because the photon momentum is small compared with reciprocal-lattice momenta. Its strength depends on the dipole matrix element and the [joint density of states](quantum-ideal-gas-statistics.md#joint-density-of-states). A [direct band gap](#direct-band-gap) permits such a transition between the band-edge states, but optical selection rules can still suppress it.

##### Parabolic-band optical energy sharing

↑ **Parent:** [Direct optical transition](#direct-optical-transition)

A vertical direct transition at a common [wavevector](elasticity-physics.md#wavevector) puts an [electron](physics.md#electron) above the conduction edge and leaves a hole below the valence edge. Their parabolic kinetic energies are inversely proportional to their effective masses. The excess [photon](quantum-mechanics.md#photon) [energy](energy.md) is therefore split as $K_e/K_h=m_h^*/m_e^*$, rather than equally unless the masses match. The initial valence [electron](physics.md#electron) [energy](energy.md) is $-K_h$ relative to its band maximum; the final conduction [energy](energy.md) is $E_g+K_e$.

#### Interband absorption

↑ **Parent:** [Interband transition](#interband-transition)

Absorption in which a [photon](quantum-mechanics.md#photon) excites an [electron](physics.md#electron) between different [energy bands](#energy-band), requiring an occupied initial state, an available final state and a nonzero transition matrix element. Indirect band-edge transitions also need momentum transfer, commonly through a [phonon](quantum-ideal-gas-statistics.md#phonon). Such absorption can prevent optical transmission even above a metal's free-carrier plasma edge.

### Superlattice

↑ **Parent:** [Electronic band structure](#electronic-band-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superlattice)

A [superlattice](#superlattice) is a spatial periodic structure with a repeat length larger than an underlying atomic lattice period. Its additional [reciprocal lattice](quantum-scattering.md#reciprocal-lattice) vectors fold electronic bands into a smaller [Brillouin zone](#brillouin-zone), and allowed couplings can open small gaps at the folded crossings. The gap sizes depend on potential Fourier components and symmetry, not on the geometric period alone.

### Flat band

↑ **Parent:** [Electronic band structure](#electronic-band-structure)

A [flat band](#flat-band) has energy independent of wavevector, and hence zero [group velocity](dispersion-relation.md#group-velocity). A nearly flat band has small dispersion and, near a parabolic extremum, large [band effective mass](#band-effective-mass). Coupling a [flat band](#flat-band) to a dispersive band can produce an [avoided crossing](#avoided-crossing) and a [hybridization gap](#hybridization-gap).

### Band hybridization

↑ **Parent:** [Electronic band structure](#electronic-band-structure)

[Band hybridization](#band-hybridization) mixes two orbital-derived bands through an off-diagonal [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) matrix element. For a real coupling $\alpha$,

$$
H(k)=\begin{pmatrix}E_a(k)&\alpha\\\alpha&E_b(k)\end{pmatrix},\qquad
E_\pm(k)=\frac{E_a+E_b\pm\sqrt{(E_a-E_b)^2+4\alpha^2}}2.
$$

An allowed bare crossing becomes an [avoided crossing](#avoided-crossing) with direct separation $2|\alpha|$. Orbital character transfers continuously between branches through the crossing. A direct separation alone does not guarantee a global [band gap](#band-gap); the extrema at different wavevectors must also be compared.

#### Flat-band hybridization Fermi-velocity suppression

↑ **Parent:** [Band hybridization](#band-hybridization)

Mix a parabolic [energy band](#energy-band) $\epsilon_k=\hbar^2k^2/(2m)$ with a perfectly [flat band](#flat-band) at $E_d>0$ through momentum-independent $V$. At zero coupling suppose the two orbital sectors have equal populations, with the dispersive sector filled to $k_0=\sqrt{2mE_d}/\hbar$. At fixed total density and sufficiently low temperature, nonzero coupling fills only the monotonic lower hybridized branch, whose [Fermi wavevector](quantum-ideal-gas-statistics.md#fermi-wavevector) is $k_F=2^{1/3}k_0$, provided the available momentum-space states accommodate it. Its small slope at that radius gives the displayed ratio to $v_F^{(1)}=\hbar k_0/m$ for $|V|\ll E_d$. The result uses the singular perfectly flat limit and an empty upper band; it is not implied by [Fermi-volume conservation in two hybridized electron bands](#fermi-volume-conservation-in-two-hybridized-electron-bands) for arbitrary pairs of dispersive bands. The zero-temperature limit must resolve the small hybridization energy scale.

#### Fermi-volume conservation in two hybridized electron bands

↑ **Parent:** [Band hybridization](#band-hybridization)

For two isotropic electron-like bands with equal spin degeneracy, conserving total [carrier density](electric-charge.md#carrier-density) conserves the sum of their occupied momentum-space volumes. If both uncoupled radii equal $k_0$,

$$
k_{F,-}^3+k_{F,+}^3=2k_0^3.
$$

Only when the upper pocket is empty does this imply a single [Fermi wavevector](quantum-ideal-gas-statistics.md#fermi-wavevector) $k_F=2^{1/3}k_0$; a nonzero mixing matrix element alone does not imply that emptying.

For a counterexample at arbitrarily weak coupling, take $E_a=Ak^2$, $E_b=C+Bk^2$, $A>B>0$, and $C=(A-B)k_0^2$. At the uncoupled [chemical potential](chemical-potential.md) $\mu_0=Ak_0^2$, both pockets have radius $k_0$. Let $\mu=\mu_0+\delta\mu$ and $y=k_F^2-k_0^2$. The [characteristic equation](linear-ordinary-differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) at the [Fermi level](quantum-ideal-gas-statistics.md#fermi-level) becomes

$$
(\delta\mu-Ay)(\delta\mu-By)=\alpha^2.
$$

Fixed density cancels the first-order chemical-potential shift. Thus $\delta\mu=O(\alpha^2)$ and $k_{F,\mp}=k_0\pm\alpha/(2k_0\sqrt{AB})+O(\alpha^2)$: both pockets remain occupied at small coupling. This expansion assumes fixed $A,B>0$ before taking $\alpha\to0$.

#### Hybridization gap

↑ **Parent:** [Band hybridization](#band-hybridization)

A [hybridization gap](#hybridization-gap) is a separation in [electronic band structure](#electronic-band-structure) caused by mixing orbital-derived states. For $E_a=Ak^2$, $E_b=E_0>0$, $A>0$ and constant coupling $\alpha>0$, the lower eigenvalue is everywhere below $E_0$ and tends to it as $k\to\infty$. The upper eigenvalue has minimum $(E_0+\sqrt{E_0^2+4\alpha^2})/2$. The unbounded model therefore has an indirect gap of width $(\sqrt{E_0^2+4\alpha^2}-E_0)/2$, approximately $\alpha^2/E_0$ at weak coupling. This differs from the direct separation $2\alpha$ at the bare crossing. A finite [Brillouin zone](#brillouin-zone) bounds the lower band farther below $E_0$.

### Mott insulator

↑ **Parent:** [Electronic band structure](#electronic-band-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mott_insulator)

A [Mott insulator](#mott-insulator) is insulating because of [electron](physics.md#electron) interactions even where a noninteracting [electronic band structure](#electronic-band-structure) would predict conduction. This mechanism differs from disorder-driven [Anderson localization](wave.md#anderson-localization).

### Energy band

↑ **Parent:** [Electronic band structure](#electronic-band-structure)

An energy band is a continuous branch $E_j(k)$ of the [dispersion relation](dispersion-relation.md) of a periodic quantum system.

#### Energy-band width

↑ **Parent:** [Energy band](#energy-band)

The range of [energy](energy.md) within one electronic [energy band](#energy-band), obtained by varying its [wavevector](elasticity-physics.md#wavevector). This differs from an interband [band gap](#band-gap).

#### Electronic bandwidth

↑ **Parent:** [Energy band](#energy-band)

The [electronic bandwidth](#electronic-bandwidth) is the difference between the maximum and minimum of one [energy band](#energy-band) over the [Brillouin zone](#brillouin-zone). It has units of energy, unlike a frequency bandwidth in signal processing. A nearest-neighbour [tight-binding model](#tight-binding) on a [primitive cubic lattice](quantum-scattering.md#primitive-cubic-lattice) with equal real [hopping integrals](#hopping-integral) $t$ has $E(\mathbf k)=E_0+2t\sum_{i=1}^3\cos(k_i a)$ and $W=12|t|$.

#### Dirac cone

↑ **Parent:** [Energy band](#energy-band)

A conical touching of two [energy bands](#energy-band), with locally linear [dispersion relation](dispersion-relation.md). The [nearest-neighbour model of graphene](chemical-substance.md#nearest-neighbour-model-of-graphene) supplies an explicit example.

##### Dirac valley

↑ **Parent:** [Dirac cone](#dirac-cone)

A region of momentum space surrounding a [Dirac cone](#dirac-cone). The two inequivalent [Dirac valleys in graphene](chemical-substance.md#dirac-valleys-in-graphene) provide a familiar example; a valley labels a region and is not the electron spin.

##### Dirac point

↑ **Parent:** [Dirac cone](#dirac-cone)

#### Electronic valley

↑ **Parent:** [Energy band](#energy-band)

A region of [wave vector](elasticity-physics.md#wavevector) space around a low-energy band feature, such as a band minimum or a [Dirac point](#dirac-point).

#### Impurity level in a crystal

↑ **Parent:** [Energy band](#energy-band)

A spatially localized electronic level produced by a defect or foreign atom in a crystalline potential. Such levels can lie in a host band gap, where no extended host state has the same energy, while impurity resonances can also occur inside an [energy band](#energy-band). Dilute localized levels are nearly independent; increasing overlap can broaden them into an impurity band. The location and existence of a bound level depend on the impurity potential.

##### Occupation of an interacting localized electron level

↑ **Parent:** [Impurity level in a crystal](#impurity-level-in-a-crystal)

A localized orbital with two [electron spin](angular-momentum-operator.md#electron-spin) states has [energies](energy.md) $E_0=0$, $E_1=\epsilon$ and $E_2=2\epsilon+U$. Its zero-[temperature](temperature.md) equilibrium occupation minimizes $\mathcal E_N=E_N-\mu N$, where $\mu$ is the [chemical potential](chemical-potential.md). For repulsion $U>0$, the occupation is successively $0,1,2$ as $\mu$ crosses $\epsilon$ and $\epsilon+U$. For attraction $U<0$, the singly occupied state is never the minimum: the occupation jumps from $0$ to $2$ at $\mu=\epsilon+U/2$. Exactly at a crossing the ground-state occupation is not unique.

At positive [temperature](temperature.md), its [grand canonical partition function](statistical-physics.md#grand-canonical-partition-function) is $\Xi=1+2e^{-\beta(\epsilon-\mu)}+e^{-\beta(2\epsilon+U-2\mu)}$, where $\beta=1/(k_BT)$. The [expected value](expected-value.md) of the occupation follows by differentiating: $\langle N\rangle=k_BT\,\partial_\mu\ln\Xi$. The factor two counts the two singly occupied [microstates](statistical-physics.md#microstate), not an additional pair state.

#### Band effective mass

↑ **Parent:** [Energy band](#energy-band)

In one dimension the [band effective mass](#band-effective-mass) is defined by $1/m^*(k)=E''(k)/\hbar^2$. Together with $v=E'(k)/\hbar$ and $\hbar\dot k=F$, this gives $\dot v=F/m^*$. Negative band curvature produces negative [effective mass](#band-effective-mass) for the electron [wave packet](dispersion-relation.md#wave-packet); near a filled-band maximum the equivalent missing-electron description uses positively responding holes. In several dimensions the inverse mass is the Hessian $\partial_i\partial_jE/\hbar^2$.

##### Hole mass from a valence-band maximum

↑ **Parent:** [Band effective mass](#band-effective-mass)

For an isotropic valence-band maximum, the electron curvature is negative. The missing-electron excitation has positive charge and positive mass $m_h^*=\hbar^2/|E\prime\prime|$. Its cyclotron angular frequency is $eB/m_h^*$. An anisotropic orbit requires the corresponding cyclotron mass rather than an arbitrary single directional curvature.

##### Effective mass for overlap-weighted exponential hopping

↑ **Parent:** [Band effective mass](#band-effective-mass)

Take the nearest-neighbour hopping $t(a)=-2E_1(1+a/a_1)e^{-a/a_1}$, with $E_1,a_1>0$, in a [simple-cubic nearest-neighbour tight-binding band](#simple-cubic-nearest-neighbour-tight-binding-band). Substituting into $m^*=-\hbar^2/(2ta^2)$ gives the displayed result. With $s=a/a_1$, its logarithmic derivative is $1-2/s-1/(1+s)$, which vanishes only at $s=1+\sqrt3>0$. The mass diverges at both positive-domain ends in this formula, so that point is its unique minimum. Its bandwidth has derivative $d\ln W/d\ln a=-s^2/(1+s)$: a small compression increases $W$. The small-$a$ continuation lies beyond reliable localized-orbital tight binding.

##### Effective-mass tensor

↑ **Parent:** [Band effective mass](#band-effective-mass)

For a semiclassical [wave packet](dispersion-relation.md#wave-packet) in an isolated [energy band](#energy-band), $v_i=\hbar^{-1}\partial_{k_i}\varepsilon$ and $\hbar\dot k_j=F_j$ imply $\dot v_i=\sum_j(m^{*-1})_{ij}F_j$. The inverse [effective-mass tensor](#effective-mass-tensor) is the [Hessian matrix](multivariable-calculus.md#hessian-matrix) of the dispersion divided by $\hbar^2$. Along a unit vector $\mathbf e$, $1/m^*_{\mathbf e}=\sum_{ij}e_i(m^{*-1})_{ij}e_j$. The [Laplacian](multivariable-calculus.md#laplacian) is its trace: $\hbar^{-2}\nabla_k^2\varepsilon=\operatorname{tr}(m^{*-1})$. Thus in $d$ isotropic dimensions the scalar mass is $d\hbar^2/(\nabla_k^2\varepsilon)$, rather than $\hbar^2/(\nabla_k^2\varepsilon)$.

##### Band-edge effective mass in a weak periodic potential

↑ **Parent:** [Band effective mass](#band-effective-mass)

In a one-dimensional two-wave [nearly-free electron model](#nearly-free-electron-model), set $\varepsilon_B=\hbar^2G^2/(8m)$ and let the coupling magnitude be $U>0$. Near the Bragg plane,

$$
E_\pm(q)=\varepsilon_B+\frac{\hbar^2q^2}{2m}\pm\sqrt{U^2+\left(\frac{\hbar^2Gq}{2m}\right)^2}.
$$

Expansion at $q=0$ gives $E_\pm=\varepsilon_B\pm U+[\hbar^2/(2m)](1\pm2\varepsilon_B/U)q^2+O(q^4)$, hence

$$
\frac{m_\pm^*}{m}=\frac1{1\pm2\varepsilon_B/U}\simeq\pm\frac{U}{2\varepsilon_B}\qquad(U\ll\varepsilon_B).
$$

The lower edge has negative electronic curvature, and the upper edge positive curvature. The last expression is a leading weak-potential approximation, not the exact curvature of the two-wave dispersion.

##### Band curvature

↑ **Parent:** [Band effective mass](#band-effective-mass)

[Band curvature](#band-curvature) is the [Hessian matrix](multivariable-calculus.md#hessian-matrix) of an [energy band](#energy-band) as a function of [wavevector](elasticity-physics.md#wavevector). Dividing it by $\hbar^2$ gives the inverse [band effective mass](#band-effective-mass) tensor. At a one-dimensional band minimum the curvature is positive, whereas at a maximum it is negative. Near a weak two-wave [avoided crossing](#avoided-crossing) with reciprocal [wavenumber](wave-equation.md#wavenumber) $G$ and coupling magnitude $U$, the two edge curvatures are $E_\pm''=\hbar^2/m\pm\hbar^4G^2/(4m^2U)$. This is a crystal response coefficient, not a change in the bare [electron mass](physics.md#electron-mass).

##### Effective mass for exponentially decaying tight-binding hopping

↑ **Parent:** [Band effective mass](#band-effective-mass)

For $t(a)=-2E_1e^{-a/a_1}$ with $E_1,a_1>0$, a nearest-neighbour cubic [tight-binding model](#tight-binding) has zone-centre [band effective mass](#band-effective-mass)

$$
m^*(a)=-\frac{\hbar^2}{2t(a)a^2}=\frac{\hbar^2 e^{a/a_1}}{4E_1a^2}.
$$

Its logarithmic derivative is $1/a_1-2/a$. The unique minimum occurs at $a=2a_1$ and has value $\hbar^2\exp(2)/(16E_1a_1^2)$. The explicit $a^2$ in band curvature competes with the exponentially weakening [hopping integral](#hopping-integral). Extrapolation to vanishing atomic separation lies outside the localized-orbital approximation.

#### Cyclotron effective mass

↑ **Parent:** [Energy band](#energy-band)

For a closed semiclassical orbit with [area](differential-geometry.md#surface-area) $S(E)$ in a plane of [wave vector](elasticity-physics.md#wavevector) space, the [cyclotron effective mass](#cyclotron-effective-mass) is defined by the displayed derivative. It need not equal the local curvature-based [band effective mass](#band-effective-mass).

#### Shubnikov-de Haas effect

↑ **Parent:** [Energy band](#energy-band)

Oscillations of [electrical resistance](electric-charge.md#electrical-resistance) as a [magnetic field](magnetic-field.md) moves [Landau levels](quantum-theory.md#landau-level) through the [Fermi energy](quantum-ideal-gas-statistics.md#fermi-energy).

##### Thermal damping of quantum oscillations

↑ **Parent:** [Shubnikov-de Haas effect](#shubnikov-de-haas-effect)

A finite-temperature measurement averages the oscillatory response over the derivative of the [Fermi-Dirac distribution](quantum-ideal-gas-statistics.md#fermi-dirac-distribution). For the fundamental harmonic and a locally constant [cyclotron effective mass](#cyclotron-effective-mass), this gives $R_T=X/\sinh X$ with $X=2\pi^2k_BT/(\hbar\omega_c)$. The oscillations become small when thermal smearing substantially exceeds their Landau-level spacing.

##### Dingle factor

↑ **Parent:** [Shubnikov-de Haas effect](#shubnikov-de-haas-effect)

The [Dingle factor](#dingle-factor) describes the damping of quantum oscillations by Landau-level broadening. For a Lorentzian half-width $\hbar/(2\tau_q)$, the fundamental harmonic has $R_D=\exp[-\pi/(\omega_c\tau_q)]$. Since $\omega_c$ decreases with field, the amplitude decays at large inverse field. The lifetime here is the [quantum lifetime](physics.md#quantum-lifetime), not automatically the mobility-derived transport time.

#### Allowed energy band

↑ **Parent:** [Energy band](#energy-band)

An allowed energy band is an interval of energies supporting extended [Bloch states](#bloch-state). Adjacent bands may be separated by a [band gap](#band-gap).

#### Band gap

↑ **Parent:** [Energy band](#energy-band)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Band_gap)

A band gap is an energy interval between adjacent [energy bands](#energy-band) containing no allowed bulk state.

##### Positive direct gaps can coexist with band overlap

↑ **Parent:** [Band gap](#band-gap)

A [direct band gap](#direct-band-gap) compares two [energy bands](#energy-band) at the same [crystal momentum](#crystal-momentum). A global gap instead requires the lowest energy of the upper band to exceed the highest energy of the lower band, allowing the two extrema to occur at different momenta. For example, the periodic toy bands $E_1(k)=A\cos k$ and $E_2(k)=A\cos k+\delta$, with $A>0$ and $0<\delta<2A$, have positive direct separation $\delta$ everywhere but global overlap $2A-\delta$. A positive direct splitting at each [Brillouin zone](#brillouin-zone) boundary therefore does not alone establish an insulating filled band. At a suitable electron count the overlap can produce both electron and hole pockets.

##### Indirect band gap

↑ **Parent:** [Band gap](#band-gap)

An [indirect band gap](#indirect-band-gap) separates a [valence band](quantum-mechanics.md#valence-band) maximum and a [conduction band](quantum-mechanics.md#conduction-band) minimum at different values of [crystal momentum](#crystal-momentum). A near-edge radiative transition then usually needs a [phonon](quantum-ideal-gas-statistics.md#phonon) or another momentum-transfer process in addition to the [photon](quantum-mechanics.md#photon), whose momentum is small on the [Brillouin zone](#brillouin-zone) scale. A [direct band gap](#direct-band-gap) has the extrema at the same [crystal momentum](#crystal-momentum) and more readily supports efficient band-edge light emission. A material can have direct transitions at higher energy while its smallest gap is indirect.

###### Indirect gap of a separable square cosine potential

↑ **Parent:** [Indirect band gap](#indirect-band-gap)

For $-V_0(\cos Qx+\cos Qy)$, two-dimensional bands are sums of one-dimensional bands. At first order, the first-band maximum is $E_Q/2-V_0$ at the corner, while the second-band minimum is $E_Q/4+V_0/2$ at an edge centre. Hence $\Delta_{\rm ind}\simeq3V_0/2-E_Q/4$, giving a rough onset $V_0\sim E_Q/6$. Higher plane waves shift this estimate; insulating filling must be checked separately.

##### Direct band gap

↑ **Parent:** [Band gap](#band-gap)

A [band gap](#band-gap) whose [conduction band](quantum-mechanics.md#conduction-band) minimum and [valence band](quantum-mechanics.md#valence-band) maximum occur at the same [crystal momentum](#crystal-momentum), allowing an optical transition without a momentum-balancing [phonon](quantum-ideal-gas-statistics.md#phonon).

##### Avoided crossing

↑ **Parent:** [Band gap](#band-gap)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Avoided_crossing)

An avoided crossing occurs when two parameter-dependent [eigenvalues](linear-operator-theory.md#eigenvalue) approach one another but an interaction prevents equality. Near a two-level crossing, a nonzero off-diagonal [matrix element](vector-space.md#matrix-element) opens a positive minimum gap.

#### Band filling

↑ **Parent:** [Energy band](#energy-band)

For spin-one-half electrons, one nondegenerate orbital band contains two one-particle states per primitive cell, one for each spin. A partially filled band has nearby empty states into which an electric field can move electrons and is ordinarily conducting. A completely filled band carries no net current under a small field because all crystal momenta are occupied symmetrically.

##### Carrier compensation and even band filling in a square lattice

↑ **Parent:** [Band filling](#band-filling)

With [spin degeneracy](statistical-physics.md#spin-degeneracy) two, one full square-zone band has density $Q^2/(2\pi^2)$. Thus $n_e-n_h=n-Q^2/(2\pi^2)$. If $Q=\alpha\sqrt{2\pi n}$, compensation requires $\alpha=\sqrt\pi$ and the real-space cell contains two electrons. A global gap is also necessary for an insulator.

###### Translation-symmetry breaking changes the band-filling constraint

↑ **Parent:** [Carrier compensation and even band filling in a square lattice](#carrier-compensation-and-even-band-filling-in-a-square-lattice)

##### Band insulator

↑ **Parent:** [Band filling](#band-filling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Band_insulator)

A band insulator has an integer number of completely filled [energy bands](#energy-band), with the [Fermi energy](quantum-ideal-gas-statistics.md#fermi-energy) inside a positive [band gap](#band-gap). At zero temperature, no arbitrarily low-energy charged excitation is then available.

###### Odd filling obstructs a spin-degenerate band insulator

↑ **Parent:** [Band insulator](#band-insulator)

In an independent-electron crystal with two spin states and no spin splitting, each completely filled [energy band](#energy-band) contains two [electrons](physics.md#electron) per primitive cell. An odd [electron](physics.md#electron) count per primitive cell therefore cannot fill an integer number of such bands. Enlarging the actual primitive cell, breaking the relevant degeneracy or including correlated-electron physics changes the premises. Even filling is necessary in this model but not sufficient: bands can overlap.

###### Kondo insulator

↑ **Parent:** [Band insulator](#band-insulator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kondo_insulator)

A [Kondo insulator](#kondo-insulator) has a bulk insulating state associated with mixing between relatively localized correlated electronic states and itinerant conduction states. A renormalized two-band picture captures a narrow [hybridization gap](#hybridization-gap), although an uncorrelated orbital-mixing model does not explain the formation and temperature dependence of the coherent low-energy state. [Samarium hexaboride](chemical-substance.md#samarium-hexaboride) is an example.

###### Overlapping energy bands prevent a band insulator

↑ **Parent:** [Band insulator](#band-insulator)

If the minimum of the next [energy band](#energy-band) lies at or below the maximum of the nominally filled band, electrons can lower their energy by occupying the next band and leaving holes in the first. The resulting partially filled bands prevent a band-insulating state.

###### Indirect gap in a uniformly split zone-boundary model

↑ **Parent:** [Overlapping energy bands prevent a band insulator](#overlapping-energy-bands-prevent-a-band-insulator)

Suppose a model replaces a set of free-electron boundary energies $E^{(0)}$ by lower and upper edges $E^{(0)}-V$ and $E^{(0)}+V$, with $V>0$. If these are the relevant global band edges, the [indirect band gap](#indirect-band-gap) is $(E_{\min}^{(0)}+V)-(E_{\max}^{(0)}-V)$, giving the displayed expression. A positive direct gap $2V$ at each crossing need not be enough: a [band insulator](#band-insulator) needs $2V>E_{\max}^{(0)}-E_{\min}^{(0)}$. This is a band-edge estimate, not a general three-dimensional nearly-free-electron theorem; multiple Bragg planes at a corner can require a larger coupling matrix.

## Bloch oscillation

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)

In a single isolated [energy band](#energy-band), a [wave packet](dispersion-relation.md#wave-packet) subject to a constant force satisfies $\hbar\dot k=F$. Its [group velocity](dispersion-relation.md#group-velocity) is periodic in $k$ with reciprocal-lattice period $2\pi/a$, so its position oscillates with period $2\pi\hbar/(|F|a)$ when its mean velocity over a band is zero. For $E(k)=E_0-2J\cos ka$, integrating the sinusoidal velocity gives the oscillation explicitly. This ideal description neglects scattering and interband tunnelling.

### Excursion amplitude of a Bloch-oscillating wavepacket

↑ **Parent:** [Bloch oscillation](#bloch-oscillation)

For $\epsilon(k)=\epsilon_0-2J\cos ka$ and electron force $-eE$, $k(t)=k_0-eEt/\hbar$. Integrating the [group velocity](dispersion-relation.md#group-velocity) gives $x(t)-x(0)=2J[\cos(k_0a-\omega_Bt)-\cos(k_0a)]/(eE)$, with $\omega_B=eEa/\hbar$ for positive $E$. The amplitude about the mean is $2|J|/(e|E|)$ and the peak-to-peak extent is twice that.

### Cold-atom Bloch oscillation experiment

↑ **Parent:** [Bloch oscillation](#bloch-oscillation)

In a 1996 experiment, ultracold cesium atoms were loaded into the lowest band of an optical standing wave made with $852\,\mathrm{nm}$ light. Chirping the frequency difference of its counterpropagating beams accelerated the lattice, producing a constant inertial force in its frame. Switching off the lattice after different evolution times allowed momentum-distribution measurements. The observed oscillations tested the periodic band velocity underlying a [Bloch oscillation](#bloch-oscillation); the lattice period and imposed acceleration controlled the oscillation frequency.[Physical Review Letters 76, pp. 4508–4509: optical preparation, accelerating lattice, time-dependent momentum distribution](physics-bibliography.md#bloch-oscillations-of-atoms-in-an-optical-potential-by-maxime-dahan-and-others)

## Translation-character proof of Bloch theorem

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)

The lattice translations commute with one another and with a lattice-periodic Hamiltonian. They can therefore be diagonalized simultaneously within each energy eigenspace. Every unitary character of a [Bravais lattice](quantum-scattering.md#bravais-lattice) has the form $r\mapsto e^{-ik\cdot r}$, with $k$ defined modulo the [reciprocal lattice](quantum-scattering.md#reciprocal-lattice). Hence $T_r\psi_k=e^{-ik\cdot r}\psi_k$, so $u_k(x)=e^{-ik\cdot x}\psi_k(x)$ is lattice-periodic.

## Bloch state

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)

A Bloch state is an energy eigenstate of a lattice-periodic Hamiltonian that is simultaneously an eigenstate of every lattice translation. It can be written as $\psi_k(x)=e^{ik\cdot x}u_k(x)$ with lattice-periodic $u_k$.

### Crystal momentum

↑ **Parent:** [Bloch state](#bloch-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crystal_momentum)

Crystal momentum is the translation quantum number $\hbar k$ of a [Bloch state](#bloch-state). Since $k$ and $k+G$ give the same translation character whenever $G$ belongs to the [reciprocal lattice](quantum-scattering.md#reciprocal-lattice), crystal momentum is defined modulo reciprocal-lattice vectors.

## Periodic potential

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Periodic_potential)

A periodic potential satisfies $V(x+a)=V(x)$ for some lattice period $a$. Its Fourier coefficients couple plane waves whose wavevectors differ by reciprocal-lattice vectors.

## Nearly-free electron model

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nearly-free_electron_model)

The nearly-free electron model treats a weak [periodic potential](#periodic-potential) by [degenerate perturbation theory](quantum-mechanics.md#degenerate-perturbation-theory). At a Bragg crossing, a Fourier coefficient $V_n$ couples the two degenerate plane waves and opens an energy gap of width $2|V_n|$.

### Monovalent BCC direct optical threshold

↑ **Parent:** [Nearly-free electron model](#nearly-free-electron-model)

For two electrons per conventional monovalent BCC cell, $k_F=(6\pi^2)^{1/3}/a$ lies inside the first zone. The shortest reciprocal vector is $G=2\sqrt2\pi/a$. The free folded-branch difference $\hbar^2(G^2-2Gk)/(2m_e)$ is smallest on the occupied Fermi-sphere point toward G, giving the displayed ratio. The destination has magnitude $G-k_F>k_F$ and is empty. A weak periodic potential supplies band mixing and optical matrix elements; its finite corrections and absorption peak shape are not fixed by this leading threshold.

### Zone-face two-plane-wave gap for a cosine potential

↑ **Parent:** [Nearly-free electron model](#nearly-free-electron-model)

For $-V_0\cos Qx$, the Fourier coupling between the two free states at $k=\pm Q/2$ is $-V_0/2$. The split energies are $E_Q/4\mp V_0/2$, with $E_Q=\hbar^2Q^2/(2m)$. The direct face gap is $V_0$, not $2V_0$.

#### Four-plane-wave splitting at a square-zone corner

↑ **Parent:** [Zone-face two-plane-wave gap for a cosine potential](#zone-face-two-plane-wave-gap-for-a-cosine-potential)

### Rectangular-lattice Fermi-surface reconstruction

↑ **Parent:** [Nearly-free electron model](#nearly-free-electron-model)

Consider a spin-degenerate two-dimensional [free electron model](physics.md#free-electron-model) with rectangular periods $a>b$ and two [electrons](physics.md#electron) per [unit cell](quantum-scattering.md#unit-cell). Write $K=\pi/a$, $L=\pi/b$, and $k_F^2=4\pi/(ab)$. If $K<k_F<L$, the circular [Fermi contour](fermi-liquid.md#fermi-contour) crosses only the vertical boundaries of the first [Brillouin zone](#brillouin-zone). Folding translates its protruding caps back by a [reciprocal lattice](quantum-scattering.md#reciprocal-lattice) vector $(2K,0)$. A weak [periodic potential](#periodic-potential) mixes the intersecting [plane waves](wave-function.md#plane-wave), reconnecting the contours into two open first-band sheets and a closed second-band pocket. The pocket is centred on a zone boundary: its halves on opposite sides of a reduced-zone plot are identified periodically and belong to one closed sheet.

#### Two-wave estimate of a Bragg-gap coupling from a pocket area

↑ **Parent:** [Rectangular-lattice Fermi-surface reconstruction](#rectangular-lattice-fermi-surface-reconstruction)

Put $C=\hbar^2/(2m)$, $v=|V_G|$, $\mathbf G=(2K,0)$, and $k_x=K+q$. The upper [eigenvalue](linear-operator-theory.md#eigenvalue) of the two coupled [plane waves](wave-function.md#plane-wave) is

$$
E_+(q,k_y)=C(K^2+q^2+k_y^2)+\sqrt{4C^2K^2q^2+v^2}.
$$

At fixed [Fermi energy](quantum-ideal-gas-statistics.md#fermi-energy) $Ck_F^2$, its closed [Fermi contour](fermi-liquid.md#fermi-contour) has

$$
y(q)^2=k_F^2-K^2-q^2-\sqrt{4K^2q^2+(v/C)^2},\qquad
q_m^2=k_F^2+K^2-\sqrt{4k_F^2K^2+(v/C)^2}.
$$

Thus $A(v)=4\int_0^{q_m}y(q)\,dq$ can be inverted numerically to estimate the [Bragg scattering](quantum-scattering.md#bragg-scattering) coupling. The pocket disappears at $v=C(k_F^2-K^2)$. The estimate assumes a fixed [chemical potential](chemical-potential.md) and neglects coupling to other [plane waves](wave-function.md#plane-wave); a measured pocket area alone does not determine all [Fourier coefficients](fourier-series.md#fourier-coefficient) of an arbitrary lattice potential.

#### Lens bound on a reconstructed Fermi pocket

↑ **Parent:** [Rectangular-lattice Fermi-surface reconstruction](#rectangular-lattice-fermi-surface-reconstruction)

In [rectangular-lattice Fermi-surface reconstruction](#rectangular-lattice-fermi-surface-reconstruction), the zero-coupling closed orbit is the overlap lens of two equal circles of radius $k_F$ with centres separated by $2K$. Two circular sectors minus their triangular portions give

$$
A_{\max}=2k_F^2\arccos\frac{K}{k_F}-2K\sqrt{k_F^2-K^2}.
$$

At fixed [chemical potential](chemical-potential.md), the upper hybridized [energy band](#energy-band) rises when the magnitude of the [Fourier coefficient](fourier-series.md#fourier-coefficient) increases. Its occupied pocket therefore shrinks, so this lens is an upper bound in the two-wave model. It is not a universal bound for arbitrary changes of [chemical potential](chemical-potential.md) or additional [energy bands](#energy-band).

### Bragg gap ladder for a linear dispersion

↑ **Parent:** [Nearly-free electron model](#nearly-free-electron-model)

For a scalar one-dimensional dispersion $E(k)=\hbar v|k|$ and a potential of period $L$, a reciprocal vector $nG$, $G=2\pi/L$, connects degenerate right- and left-moving states at $k=nG/2$. Their unperturbed energy is $E_n=n\pi\hbar v/L$. Thus consecutive allowed Bragg thresholds have spacing $\pi\hbar v/L$, whereas shifting momentum by a full reciprocal period changes a linear branch's energy by $2\pi\hbar v/L$. The potential's Fourier coefficients and higher-order couplings determine which gaps actually open and their widths, so a geometric period alone does not imply an exactly energy-periodic spectrum. A graphene pseudospin selection rule can further suppress scattering; the scalar-chain model omits that internal structure.

### Nearly-free electron dispersion near a one-dimensional band gap

↑ **Parent:** [Nearly-free electron model](#nearly-free-electron-model)

For

$$
V(x)=\sum_{n\in\mathbb Z}V_ne^{2\pi inx/a},
$$

write $k=n\pi/a+\kappa$. Near the $n$th Bragg crossing,

$$
E_\pm(k)=V_0+\frac{\hbar^2}{2m}
\left[\left(\frac{n\pi}{a}\right)^2+\kappa^2\right]
\pm\sqrt{
\left(\frac{\hbar^2n\pi\kappa}{ma}\right)^2+|V_n|^2}.
$$

At $\kappa=0$, the two branches differ by $2|V_n|$.

## Floquet matrix for a one-dimensional periodic potential

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)

For a potential of period $a$, the Floquet matrix $M(E)$ maps Cauchy data through one cell:

$$
\begin{pmatrix}\psi(x+a)\\\psi'(x+a)\end{pmatrix}
=M(E)\begin{pmatrix}\psi(x)\\\psi'(x)\end{pmatrix}.
$$

For a real Schrodinger equation, $\det M=1$.

### Floquet discriminant and energy bands

↑ **Parent:** [Floquet matrix for a one-dimensional periodic potential](#floquet-matrix-for-a-one-dimensional-periodic-potential)

The Floquet multipliers solve

$$
\mu^2-\operatorname{tr}(M)\mu+1=0.
$$

Bounded Bloch waves occur when $|\operatorname{tr}M|\leq2$, with $\mu=e^{\pm iKa}$. Band edges satisfy $\operatorname{tr}M=\pm2$; outside the bands the multipliers are real reciprocal numbers and one solution grows exponentially.

## Tight binding

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tight_binding)

A tight-binding model expands a particle's state in localized orbitals and represents tunnelling between sites by off-diagonal Hamiltonian matrix elements.

### Opposite sigma and pi hopping signs in a p-orbital chain

↑ **Parent:** [Tight binding](#tight-binding)

For a chain along $x$, translated $p_z$ orbitals form a side-on bonding combination at $k=0$, whereas translated $p_x$ orbitals form an end-on bonding combination at $k=\pi/a$. With $E=\epsilon+2t\cos ka$ and identically translated orbitals, these correspond to $t_\pi<0$ and $t_\sigma>0$. Changing the sign convention of the hopping Hamiltonian changes the parameter signs, not the physical band extrema.

### s-p mixing in a one-dimensional tight-binding chain

↑ **Parent:** [Tight binding](#tight-binding)

Opposite [parity](quantum-mechanics.md#parity) of same-centre [s orbitals](chemistry.md#s-orbital) and axial [p orbitals](chemistry.md#p-orbital) makes their left and right nearest-neighbour [hopping integrals](#hopping-integral) opposite in sign. Their [Bloch wave](#bloch-state) sum is consequently odd in wavevector and vanishes at the zone centre and boundary. Away from those points, [orbital hybridization](chemistry.md#orbital-hybridization) repels coupled levels and can produce an [avoided crossing](#avoided-crossing).

### Orbital phase and the sign of one-dimensional hopping

↑ **Parent:** [Tight binding](#tight-binding)

In an orthogonal one-orbital nearest-neighbor [tight-binding model](#tight-binding), the [hopping integral](#hopping-integral) is $t=\langle\phi_j|H|\phi_{j+1}\rangle$ and the dispersion is the displayed cosine. Using the same orbital-phase convention at every site, equal s-orbital coefficients usually make a bonding state at the zone center, so $t<0$ and $k=0$ is a band minimum. For $p_x$ orbitals along the chain, with every positive lobe pointing right, equal site coefficients bring opposite-sign lobes together between atoms. This is antibonding; alternating coefficients are bonding, giving the usual $t_\sigma>0$ and a band maximum at zero. Changing conventions requires transforming the Bloch basis consistently. The physical statement concerns the curvature and orbital character of a specified Bloch state, not an isolated hopping sign divorced from its basis.

### Filling fraction of an independent cosine band

↑ **Parent:** [Tight binding](#tight-binding)

For a [dispersion relation](dispersion-relation.md) $E(k)=E_0+t\cos(ka)$, $t<0$, occupied states at zero [temperature](temperature.md) form the interval $|k|<k_F$ in the first [Brillouin zone](#brillouin-zone). Its occupied fraction is $f=2k_F/(2\pi/a)=k_Fa/\pi$. A spin-degenerate band therefore holds $2f$ [electrons](physics.md#electron) per site. If the band is independent of the other two wavevector coordinates, its [Fermi surface](fermi-liquid.md#fermi-surface) consists of two planes. For $t>0$ the occupied region is instead near the zone edges, bounded by $|k|=\pi(1-f)/a$.

### Three-site tight-binding ring

↑ **Parent:** [Tight binding](#tight-binding)

In an [orthonormal basis](inner-product.md#orthonormal-basis) of localized [atomic orbitals](chemistry.md#atomic-orbital), a ring of three equivalent sites with real hopping $t$ has [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) $H=(E_0-t)I+tJ$, where $J$ is the three-by-three [all-ones matrix](vector-space.md#all-ones-matrix). The normalized symmetric state $(|1\rangle+|2\rangle+|3\rangle)/\sqrt3$ has energy $E_0+2t$. Its two-dimensional [orthogonal complement](hilbert-space.md#orthogonal-complement) has energy $E_0-t$. Thus the symmetric state is the unique spatial [ground state](quantum-mechanics.md#ground-state) for $t<0$, with an [energy](energy.md) difference $3|t|$ to the excited [eigenstates](energy-eigenvalue.md#eigenstate). Equivalently, the three discrete [Bloch states](#bloch-state) have energies $E_0+2t\cos(2\pi l/3)$, $l=0,\pm1$. Nonorthogonal [atomic orbitals](chemistry.md#atomic-orbital) instead require a [generalized eigenvalue problem](linear-operator-theory.md#generalized-eigenvalue-problem).

### Nonorthogonal nearest-neighbour tight-binding band

↑ **Parent:** [Tight binding](#tight-binding)

For one localized orbital per site in a chain, take on-site matrix elements $H_{jj}=E_0$, nearest-neighbour matrix elements $H_{j,j\pm1}=h$, overlaps $S_{jj}=1$ and $S_{j,j\pm1}=s$, with other terms neglected and $h,s$ real. A [Bloch state](#bloch-state) reduces the [generalized eigenvalue problem](linear-operator-theory.md#generalized-eigenvalue-problem) $Hc=ESc$ to

$$
E_0+2h\cos(ka)=E[1+2s\cos(ka)],\qquad
E(k)=\frac{E_0+2h\cos(ka)}{1+2s\cos(ka)}.
$$

The overlap metric must be positive for the retained model; $|s|<1/2$ is sufficient for all $k$. Dropping it yields the cosine band of the [orthogonal tight-binding approximation](#orthogonal-tight-binding-approximation).

### Orthogonal tight-binding approximation

↑ **Parent:** [Tight binding](#tight-binding)

In the [orthogonal tight-binding approximation](#orthogonal-tight-binding-approximation), localized basis states satisfy $\langle i|j\rangle=\delta_{ij}$ while the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) retains nonzero [hopping integrals](#hopping-integral). These are independent matrix elements: orthogonal states need not have vanishing Hamiltonian coupling. One can construct localized orthonormal orbitals from overlapping atomic orbitals; truncating the resulting Hamiltonian to nearest neighbours is a further approximation. An overlap matrix must instead be retained for raw nonorthogonal orbitals.

#### Simple-cubic nearest-neighbour tight-binding band

↑ **Parent:** [Orthogonal tight-binding approximation](#orthogonal-tight-binding-approximation)

For one orthonormal localized orbital per simple-cubic site and real equal nearest-neighbour [hopping integral](#hopping-integral) $t$, the six neighbours give the displayed [energy band](#energy-band). Each cosine ranges from minus one to one, so the positive bandwidth is $12|t|$, independently of the sign convention for $t$. Near the zone centre, $E=E_0+6t-ta^2k^2+O(k^4)$ and the [band effective mass](#band-effective-mass) is $-\hbar^2/(2ta^2)$. It is positive there for $t<0$; for $t>0$ the zone centre is a maximum instead.

### Hopping integral

↑ **Parent:** [Tight binding](#tight-binding)

A [hopping integral](#hopping-integral) is an off-diagonal [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) matrix element between localized orbitals on different lattice sites. It has units of energy and controls the dispersion in a [tight-binding model](#tight-binding). Its sign and phase depend on the orbital phase convention; observable band energies do not. The sign of a real nearest-neighbour $t$ in $E(k)=E_0+2t\cos(ka)$ determines the location of the minimum in that convention.

#### Projected hopping matrix element and sign convention

↑ **Parent:** [Hopping integral](#hopping-integral)

If a tight-binding [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) is written with coefficient $-t_{ij}$ multiplying $c_i^\dagger c_j$, projecting the one-electron [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) gives the displayed relation. An alternative convention defines the coefficient itself as the [hopping integral](#hopping-integral) and has no leading minus. [Orthogonality](inner-product.md#orthogonal-vectors) removes constant scalar potentials from off-diagonal matrix elements, but does not remove a spatially varying potential. Orbital rephasing changes both matrix elements together and cannot repair an algebraic mismatch between these two conventions in a fixed basis.

### Pseudospin

↑ **Parent:** [Tight binding](#tight-binding)

A two-state degree of freedom represented mathematically like [spin one-half](angular-momentum-operator.md#spin-one-half), without necessarily being physical [spin](angular-momentum-operator.md#spin). The [sublattice pseudospin in graphene](chemical-substance.md#sublattice-pseudospin-in-graphene) labels amplitudes on two sites per primitive cell.

### Dilute-hopping lattice propagator

↑ **Parent:** [Tight binding](#tight-binding)

For equivalent minima with nearest-neighbour hopping magnitude $\Delta$, paths with $r$ right steps and $s$ left steps have $r-s=n-m$. Summing $(\Delta\tau/\hbar)^{r+s}/(r!s!)$ and applying the [Fourier representation of a Kronecker delta](discrete-fourier-transform.md#fourier-representation-of-a-kronecker-delta) gives the displayed [modified Bessel function](bessel-function.md#modified-bessel-function) kernel in a normalized localized-site basis. Its Fourier exponent gives the [tight-binding model](#tight-binding) energy $E(\theta)=E_{\rm well}-2\Delta\cos\theta$. Position-endpoint kernels can have an additional common local-wavefunction prefactor.

### Harmonic approximation near a potential minimum

↑ **Parent:** [Tight binding](#tight-binding)

Near a nondegenerate minimum $x_0$, a smooth potential satisfies

$$
V(x)=V(x_0)+\frac12V''(x_0)(x-x_0)^2+\cdots.
$$

The localized levels are therefore approximately those of a harmonic oscillator of frequency $\sqrt{V''(x_0)/m}$; tunnelling broadens each level into a narrow band.

### Finite periodic tight-binding ring

↑ **Parent:** [Tight binding](#tight-binding)

For $N$ identical sites of spacing $a$ with periodic boundary conditions, translation eigenstates have coefficients

$$
c_n=\frac{1}{\sqrt N}e^{ikna},
\qquad
e^{ikNa}=1.
$$

Thus $k=2\pi j/(Na)$ modulo the reciprocal-lattice period $2\pi/a$.

### Two-direction nearest-neighbour tight-binding dispersion

↑ **Parent:** [Tight binding](#tight-binding)

For hopping amplitude $-\lambda$ from each lattice site to its neighbours at $\pm a_1$ and $\pm a_2$, a Bloch state has energy

$$
E(k)=E_0-2\lambda\bigl(\cos(k\cdot a_1)+\cos(k\cdot a_2)\bigr).
$$

The band ranges from $E_0-4|\lambda|$ to $E_0+4|\lambda|$ and therefore has width $8|\lambda|$.

## Brillouin zone

↑ **Parent:** [Bloch's theorem](bloch-s-theorem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brillouin_zone)

The first Brillouin zone is a fundamental cell in reciprocal space. For a one-dimensional lattice of spacing $a$, one conventional choice is

$$
-\frac{\pi}{a}\leq k<\frac{\pi}{a}.
$$

### Gamma point

↑ **Parent:** [Brillouin zone](#brillouin-zone)

The [Gamma point](#gamma-point) is zero crystal wavevector, modulo reciprocal-lattice vectors. A [direct band gap](#direct-band-gap) at this point allows a low-energy vertical optical transition with negligible photon momentum. Crystal symmetry constrains the degeneracies and symmetry labels of the band-edge states.

### Reduced Brillouin zone

↑ **Parent:** [Brillouin zone](#brillouin-zone)

A [reduced Brillouin zone](#reduced-brillouin-zone) is the reciprocal primitive cell for an enlarged real-space unit cell. Doubling a one-dimensional unit cell halves the [momentum](momentum.md) interval but adds a second internal sublattice degree of freedom. Band folding therefore preserves the number of [normal modes](wave-equation.md#normal-mode).

### Second Brillouin zone

↑ **Parent:** [Brillouin zone](#brillouin-zone)

The extended-zone region reached from the first zone by crossing one Bragg plane from the origin, excluding boundaries. For a one-dimensional lattice with spacing $a$, its two components are $\pi/a<|k|<2\pi/a$. It is not simply a translated first-zone cell.

### First Brillouin zone

↑ **Parent:** [Brillouin zone](#brillouin-zone)

The [Wigner-Seitz cell](quantum-scattering.md#wigner-seitz-cell) of a [reciprocal lattice](quantum-scattering.md#reciprocal-lattice) centered at the origin. It contains wavevectors at least as close to zero as to any other [reciprocal lattice](quantum-scattering.md#reciprocal-lattice) point. Boundary sharing conventions do not change its area or volume.

### Zone folding in an equal-mass diatomic chain

↑ **Parent:** [Brillouin zone](#brillouin-zone)

Putting $M=m$ in the [diatomic-chain dispersion relation with equal springs](quantum-ideal-gas-statistics.md#diatomic-chain-dispersion-relation-with-equal-springs) gives $\omega_-=2\sqrt{K/m}|\sin(kd/2)|$ and $\omega_+=2\sqrt{K/m}|\cos(kd/2)|$ in the reduced zone $|k|\leq\pi/(2d)$. The branches touch at its edge. If the sites are actually identical, the true [primitive unit cell](quantum-scattering.md#primitive-unit-cell) has length $d$; the apparent [optical phonon branch](quantum-ideal-gas-statistics.md#optical-phonon-branch) is the outer part of the [monatomic-chain dispersion relation](quantum-ideal-gas-statistics.md#monatomic-chain-dispersion-relation) folded by an unnecessarily doubled cell. A gap does not appear merely from redrawing the zone.

### Bragg point

↑ **Parent:** [Brillouin zone](#brillouin-zone)

A Bragg point is a [crystal momentum](#crystal-momentum) at which two plane waves differing by a [reciprocal lattice](quantum-scattering.md#reciprocal-lattice) vector are degenerate. A periodic potential mixes the waves there, producing an [avoided crossing](#avoided-crossing) and opening a [band gap](#band-gap).

### Brillouin zone of a two-dimensional triangular lattice

↑ **Parent:** [Brillouin zone](#brillouin-zone)

The reciprocal lattice of a two-dimensional triangular [Bravais lattice](quantum-scattering.md#bravais-lattice) is triangular, so its [Wigner-Seitz cell](quantum-scattering.md#wigner-seitz-cell) is a regular hexagon. Opposite boundary points are identified modulo reciprocal-lattice translations, and the six corners fall into two inequivalent classes of three corners each, conventionally denoted $K$ and $K'$.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (10)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-c/c11/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-c/c11/c/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2.md#section-c/c8/a/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2006.md#section-b/b6/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2007.md#section-b/b4/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2014.md#2/c/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016.md#3/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2019.md#section-a/1/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2021.md#section-b/4/a/solution)
