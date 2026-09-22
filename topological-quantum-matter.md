# Topological quantum matter

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_quantum_matter)

Topological quantum matter has robust low-energy properties controlled by global topology rather than local order parameters.

**Table of contents**

- [Topological quantum order](#topological-quantum-order)
  - [Backward preservation of local indistinguishability](#backward-preservation-of-local-indistinguishability)
- [Local indistinguishability](#local-indistinguishability)
- [Abelian Chern--Simons theory](#abelian-chern-simons-theory)
  - [Chern-Simons source stress convention](#chern-simons-source-stress-convention)
  - [K-matrix](#k-matrix)
    - [Anyon lattice of an Abelian Chern--Simons theory](#anyon-lattice-of-an-abelian-chern-simons-theory)
    - [Chern--Simons flux attachment](#chern-simons-flux-attachment)
    - [Lagrangian subgroup of Abelian anyons](#lagrangian-subgroup-of-abelian-anyons)
  - [Torus ground-state degeneracy of an Abelian Chern--Simons theory](#torus-ground-state-degeneracy-of-an-abelian-chern-simons-theory)
    - [Wilson-loop algebra of an Abelian Chern--Simons theory](#wilson-loop-algebra-of-an-abelian-chern-simons-theory)
- [Anyon](#anyon)
  - [Topological spin](#topological-spin)
  - [Charge-flux composite](#charge-flux-composite)
    - [Aharonov-Bohm effect](#aharonov-bohm-effect)
    - [Aharonov-Casher effect](#aharonov-casher-effect)
  - [Mutual semion](#mutual-semion)
  - [Anyon condensation at a boundary](#anyon-condensation-at-a-boundary)
    - [Electric and magnetic boundaries of the surface code](#electric-and-magnetic-boundaries-of-the-surface-code)
- [Topological superconductor](#topological-superconductor)
  - [Quadratic fermion Hamiltonian](#quadratic-fermion-hamiltonian)
    - [Bogoliubov--de Gennes Hamiltonian](#bogoliubov-de-gennes-hamiltonian)
      - [Particle-hole symmetry of a Bogoliubov--de Gennes Hamiltonian](#particle-hole-symmetry-of-a-bogoliubov-de-gennes-hamiltonian)
    - [Majorana fermion operator](#majorana-fermion-operator)
      - [Majorana zero mode](#majorana-zero-mode)
        - [Majorana zero mode at a mass domain wall](#majorana-zero-mode-at-a-mass-domain-wall)
          - [Continuum p-wave Majorana interface mode](#continuum-p-wave-majorana-interface-mode)
        - [Dense encoding with Majorana zero modes](#dense-encoding-with-majorana-zero-modes)
        - [Local indistinguishability of separated Majorana zero modes](#local-indistinguishability-of-separated-majorana-zero-modes)
        - [Majorana braiding operator](#majorana-braiding-operator)
          - [Measurement-only Majorana braiding](#measurement-only-majorana-braiding)
            - [Forced Majorana parity measurement](#forced-majorana-parity-measurement)
    - [Fermion parity](#fermion-parity)
      - [Fermion-parity measurement](#fermion-parity-measurement)
  - [Chiral Majorana edge mode](#chiral-majorana-edge-mode)
    - [Boundary condition of a chiral Majorana edge mode](#boundary-condition-of-a-chiral-majorana-edge-mode)
  - [Kitaev chain](#kitaev-chain)
- [Topological equivalence of gapped Hamiltonians](#topological-equivalence-of-gapped-hamiltonians)
  - [Quasi-adiabatic continuation](#quasi-adiabatic-continuation)
  - [Winding number of a one-dimensional Bogoliubov--de Gennes Hamiltonian](#winding-number-of-a-one-dimensional-bogoliubov-de-gennes-hamiltonian)
- [Symmetry-protected topological phase](#symmetry-protected-topological-phase)
  - [Projective virtual symmetry of a matrix product state](#projective-virtual-symmetry-of-a-matrix-product-state)
    - [Protected edge state of a symmetry-protected topological phase](#protected-edge-state-of-a-symmetry-protected-topological-phase)
  - [Cluster state](#cluster-state)
- [Intrinsic topological order](#intrinsic-topological-order)
- [Kramers--Wannier duality](#kramers-wannier-duality)
  - [Kramers--Wannier intertwiner](#kramers-wannier-intertwiner)
  - [Kramers--Wannier projected entangled pair operator](#kramers-wannier-projected-entangled-pair-operator)
- [One-form symmetry](#one-form-symmetry)

## Topological quantum order

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)

The local-pair condition for [topological quantum order](#topological-quantum-order) asks for an orthogonal partner state with [local indistinguishability](#local-indistinguishability) on supports of diameter at most a fixed fraction of the system diameter, with a fixed error smaller than one. This criterion captures a form of macroscopic information hidden from local observables; it is not a complete definition of every topological phase.

### Backward preservation of local indistinguishability

↑ **Parent:** [Topological quantum order](#topological-quantum-order)

Undo a short evolution of two orthogonal locally indistinguishable states. Orthogonality is preserved exactly. A [Lieb-Robinson bound](quantum-theory.md#lieb-robinson-bound) localizes every backward-evolved observable within an expanded region and bounds its norm error. After normalizing the approximate observable, the initial expectation difference is at most $\varepsilon(1+\delta)+2\delta$. Polynomial volume growth in the system diameter controls the localization prefactor and yields preservation for sufficiently small linear-time coefficient.

## Local indistinguishability

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)

Two [quantum states](quantum-mechanics.md#quantum-state) are [locally indistinguishable](#local-indistinguishability) at a prescribed scale if all operators of norm at most one supported below that scale have nearly equal expectation values. This is a statement about restricted observables, not equality of the global states. An orthogonal pair can be locally indistinguishable on macroscopically large regions.

<h2 id="abelian-chern-simons-theory">Abelian Chern--Simons theory</h2>

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abelian_Chern--Simons_theory)

An Abelian Chern--Simons theory with integer symmetric invertible matrix $K$ describes Abelian anyons whose braiding phases are determined by $K^{-1}$.

### Chern-Simons source stress convention

↑ **Parent:** [Abelian Chern--Simons theory](#abelian-chern-simons-theory)

The pure [Abelian Chern--Simons theory](#abelian-chern-simons-theory) has zero metric stress. For a source written as $-c\int\star J\wedge A$, holding the covariant components of the [one-forms](differential-form.md#one-form) $J,A$ fixed makes the source equal to $-c\int\sqrt{-g}\,g^{\mu\nu}J_\mu A_\nu\,d^3x$. Variation using $\delta\sqrt{-g}=-\sqrt{-g}g_{\mu\nu}\delta g^{\mu\nu}/2$ gives the displayed [stress-energy tensor](general-relativity.md#stress-energy-tensor). If the independent source is instead the fixed [two-form](differential-form.md#2-form) $\mathcal J=\star J$, the source action is metric-independent and its stress vanishes. The variational data must therefore be stated.

### K-matrix

↑ **Parent:** [Abelian Chern--Simons theory](#abelian-chern-simons-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/K-matrix)

The K-matrix is the integral bilinear form multiplying the Abelian Chern--Simons gauge fields. Integer unimodular basis changes send $K$ to $WKW^T$ without changing the phase.

<h4 id="anyon-lattice-of-an-abelian-chern-simons-theory">Anyon lattice of an Abelian Chern--Simons theory</h4>

↑ **Parent:** [K-matrix](#k-matrix)

For an invertible integer $K$-matrix, Abelian anyons are integer vectors $q$ modulo local particles $K\mathbb Z^N$. Their mutual full-braiding phase is $\exp(2\pi i q^TK^{-1}q')$.

<h4 id="chern-simons-flux-attachment">Chern--Simons flux attachment</h4>

↑ **Parent:** [K-matrix](#k-matrix)

In an Abelian Chern--Simons theory, the equation of motion ties a quasiparticle's gauge charge $q$ to gauge flux $\Phi=2\pi\hbar K^{-1}q$. A quasiparticle of charge $q'$ encircling it therefore acquires the [Aharonov--Bohm phase](#aharonov-bohm-effect) $2\pi q'^TK^{-1}q$.

#### Lagrangian subgroup of Abelian anyons

↑ **Parent:** [K-matrix](#k-matrix)

A Lagrangian subgroup is a maximal set of mutually bosonic anyons that can consistently condense at a gapped boundary. An anyon can join the condensate only if it braids trivially with every already-condensed anyon.

<h3 id="torus-ground-state-degeneracy-of-an-abelian-chern-simons-theory">Torus ground-state degeneracy of an Abelian Chern--Simons theory</h3>

↑ **Parent:** [Abelian Chern--Simons theory](#abelian-chern-simons-theory)

An Abelian K-matrix Chern--Simons theory has $|\det K|$ topologically distinct ground states on a torus.

<h4 id="wilson-loop-algebra-of-an-abelian-chern-simons-theory">Wilson-loop algebra of an Abelian Chern--Simons theory</h4>

↑ **Parent:** [Torus ground-state degeneracy of an Abelian Chern--Simons theory](#torus-ground-state-degeneracy-of-an-abelian-chern-simons-theory)

Quasiparticle transport around the two fundamental cycles of a torus gives loop operators obeying

$$
T_x(q')T_y(q)=e^{2\pi i q'^TK^{-1}q}T_y(q)T_x(q').
$$

The induced pairing on $\mathbb Z^n/K\mathbb Z^n$ is nondegenerate, so this algebra has a representation of dimension at least $|\det K|$.

## Anyon

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Anyon)

An anyon is a two-dimensional quasiparticle whose exchange or braiding statistics can differ from bosonic and fermionic statistics.

### Topological spin

↑ **Parent:** [Anyon](#anyon)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_spin)

The topological spin $\theta_a$ is the phase produced by a $2\pi$ rotation of anyon $a$, equivalently its self-exchange phase in an Abelian anyon theory. The two-dimensional spin-statistics relation is $\theta_a=e^{2\pi i s_a}$.

### Charge-flux composite

↑ **Parent:** [Anyon](#anyon)

A charge-flux composite carries electric charge $q$ and localized magnetic flux $\Phi$. Mutual encircling of $(q_1,\Phi_1)$ and $(q_2,\Phi_2)$ produces the phase $\exp[i(q_1\Phi_2+q_2\Phi_1)/\hbar]$ from the Aharonov-Bohm and Aharonov-Casher effects.

#### Aharonov-Bohm effect

↑ **Parent:** [Charge-flux composite](#charge-flux-composite)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aharonov-Bohm_effect)

The Aharonov-Bohm effect is the phase $q\Phi/\hbar$ acquired when a charge $q$ encircles magnetic flux $\Phi$, even when the magnetic field vanishes along the charge's path.

#### Aharonov-Casher effect

↑ **Parent:** [Charge-flux composite](#charge-flux-composite)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aharonov-Casher_effect)

The Aharonov-Casher effect is the electromagnetic dual in which a magnetic moment or flux acquires a phase by encircling electric charge.

### Mutual semion

↑ **Parent:** [Anyon](#anyon)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mutual_semion)

Two particle types are mutual semions when taking either once around the other multiplies the state by $-1$.

### Anyon condensation at a boundary

↑ **Parent:** [Anyon](#anyon)

An anyon condenses at a boundary when its string operator may terminate there without leaving an excitation, so the boundary can absorb or emit that anyon.

#### Electric and magnetic boundaries of the surface code

↑ **Parent:** [Anyon condensation at a boundary](#anyon-condensation-at-a-boundary)

An electric boundary of the [surface code](quantum-error-correction.md#surface-code) condenses electric anyons, while a magnetic boundary condenses magnetic anyons. A local boundary Pauli can create a single condensed excitation because its string may end at that boundary.

## Topological superconductor

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_superconductor)

A topological superconductor is a gapped paired-fermion phase supporting protected boundary Majorana modes.

### Quadratic fermion Hamiltonian

↑ **Parent:** [Topological superconductor](#topological-superconductor)

A quadratic fermion Hamiltonian is bilinear in creation and annihilation operators. In a Majorana basis it is determined, up to a constant, by a real antisymmetric matrix.

<h4 id="bogoliubov-de-gennes-hamiltonian">Bogoliubov--de Gennes Hamiltonian</h4>

↑ **Parent:** [Quadratic fermion Hamiltonian](#quadratic-fermion-hamiltonian)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bogoliubov--de_Gennes_Hamiltonian)

A Bogoliubov--de Gennes Hamiltonian acts on a Nambu particle-hole spinor and describes quadratic fermion hopping and pairing.

<h5 id="particle-hole-symmetry-of-a-bogoliubov-de-gennes-hamiltonian">Particle-hole symmetry of a Bogoliubov--de Gennes Hamiltonian</h5>

↑ **Parent:** [Bogoliubov--de Gennes Hamiltonian](#bogoliubov-de-gennes-hamiltonian)

Particle-hole symmetry relates $H_{\rm BdG}(k)$ to $-H_{\rm BdG}^*(-k)$. Consequently every energy $E$ at momentum $k$ is paired with energy $-E$ at momentum $-k$.

#### Majorana fermion operator

↑ **Parent:** [Quadratic fermion Hamiltonian](#quadratic-fermion-hamiltonian)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Majorana_fermion_operator)

A Majorana fermion operator is self-adjoint and obeys $\{c_j,c_k\}=2\delta_{jk}$.

##### Majorana zero mode

↑ **Parent:** [Majorana fermion operator](#majorana-fermion-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Majorana_zero_mode)

A Majorana zero mode is a spatially localized Majorana operator that commutes with a gapped quadratic Hamiltonian, exactly or up to exponentially small finite-size corrections.

###### Majorana zero mode at a mass domain wall

↑ **Parent:** [Majorana zero mode](#majorana-zero-mode)

Two counterpropagating Majorana fields coupled by a real mass $m(x)$ bind a Majorana zero mode when $m$ changes sign. Its envelope is proportional to $\exp[-\int^x m(s)ds/(\hbar v)]$ up to orientation conventions, so a constant asymptotic mass gives localization length $\hbar v/|m|$.

###### Continuum p-wave Majorana interface mode

↑ **Parent:** [Majorana zero mode at a mass domain wall](#majorana-zero-mode-at-a-mass-domain-wall)

For the long-wavelength Bogoliubov--de Gennes Hamiltonian $H=-\mu(x)\tau_z-i\hbar\Delta\tau_x\partial_x$, a sign change from $\mu>0$ in a one-dimensional p-wave superconductor to $\mu<0$ in the vacuum binds a zero mode of width $\xi=\hbar\Delta/|\mu|$. Neglecting the quadratic kinetic term is valid when $|\mu|\ll m\Delta^2$ up to an inessential numerical factor.

###### Dense encoding with Majorana zero modes

↑ **Parent:** [Majorana zero mode](#majorana-zero-mode)

$2M$ Majorana zero modes define $M$ complex fermionic modes. Fixing total [fermion parity](#fermion-parity) leaves a $2^{M-1}$-dimensional ground space, encoding $M-1$ qubits.

###### Local indistinguishability of separated Majorana zero modes

↑ **Parent:** [Majorana zero mode](#majorana-zero-mode)

When Majorana zero modes have disjoint exponentially localized supports, every local parity-even observable acts as a scalar on the fixed-parity ground space. Finite overlap changes this by terms exponentially small in separation divided by localization length.

###### Majorana braiding operator

↑ **Parent:** [Majorana zero mode](#majorana-zero-mode)

The unitary $R_{ab}=\exp(\pi\gamma_a\gamma_b/4)$ exchanges two Majorana operators by conjugation, sending one to the other and the other to its negative, with signs fixed by braid orientation.

###### Measurement-only Majorana braiding

↑ **Parent:** [Majorana braiding operator](#majorana-braiding-operator)

Pairwise [fermion-parity measurements](#fermion-parity-measurement) involving an ancillary Majorana mode can reproduce a [Majorana braiding operator](#majorana-braiding-operator) without physically moving the zero modes. Projecting the ancilla back to its initial parity sector turns the product of projectors into the braid unitary up to normalization and known outcome-dependent signs.

###### Forced Majorana parity measurement

↑ **Parent:** [Measurement-only Majorana braiding](#measurement-only-majorana-braiding)

A forced Majorana parity measurement alternates an undesired pairwise measurement with a reference parity measurement until the desired outcome occurs. Anticommuting parity observables give either result with probability one half, so the protocol terminates almost surely with a geometric waiting time.

#### Fermion parity

↑ **Parent:** [Quadratic fermion Hamiltonian](#quadratic-fermion-hamiltonian)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermion_parity)

Fermion parity is $(-1)^F$. It acts as plus one on bosonic states and minus one on fermionic states. Even operators commute with it and odd operators, including supersymmetry generators, anticommute with it. Local observables are parity even because observable algebras of spacelike separated regions must commute.

##### Fermion-parity measurement

↑ **Parent:** [Fermion parity](#fermion-parity)

A fermion-parity measurement projects onto an eigenspace of the parity of a chosen collection of fermionic modes. For two [Majorana fermion operators](#majorana-fermion-operator) $\gamma_a$ and $\gamma_b$, the projectors are $(1\pm i\gamma_a\gamma_b)/2$.

### Chiral Majorana edge mode

↑ **Parent:** [Topological superconductor](#topological-superconductor)

A chiral Majorana edge mode is a self-adjoint one-way boundary field with Hamiltonian proportional to $-i\int c\,\partial_xc\,dx$. Its group velocity has one sign throughout the low-energy branch.

#### Boundary condition of a chiral Majorana edge mode

↑ **Parent:** [Chiral Majorana edge mode](#chiral-majorana-edge-mode)

On a closed boundary, a chiral Majorana field is antiperiodic in the sector with even enclosed vortex parity and periodic in the sector with odd enclosed vortex parity. Only the periodic sector contains a zero-momentum Majorana mode.

### Kitaev chain

↑ **Parent:** [Topological superconductor](#topological-superconductor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kitaev_chain)

The Kitaev chain is a one-dimensional spinless p-wave superconductor. Its topological phase has a Majorana zero mode at each end of an open chain.

## Topological equivalence of gapped Hamiltonians

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)

Two local gapped Hamiltonians are topologically equivalent when they are connected by a continuous path of local Hamiltonians with a nonzero bulk gap, equivalently when their ground spaces are related by quasi-local evolution.

### Quasi-adiabatic continuation

↑ **Parent:** [Topological equivalence of gapped Hamiltonians](#topological-equivalence-of-gapped-hamiltonians)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-adiabatic_continuation)

Quasi-adiabatic continuation implements a gapped path of local Hamiltonians by a quasi-local unitary. It dresses local operators with exponentially decaying tails while preserving their action within the corresponding low-energy spaces.

<h3 id="winding-number-of-a-one-dimensional-bogoliubov-de-gennes-hamiltonian">Winding number of a one-dimensional Bogoliubov--de Gennes Hamiltonian</h3>

↑ **Parent:** [Topological equivalence of gapped Hamiltonians](#topological-equivalence-of-gapped-hamiltonians)

For a two-component gapped BdG Hamiltonian constrained to a plane, the winding number counts how many times its coefficient vector encircles the origin as crystal momentum traverses the Brillouin zone.

## Symmetry-protected topological phase

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetry-protected_topological_phase)

A symmetry-protected topological phase is short-range entangled but cannot be deformed to a product state without breaking a protecting symmetry or closing the gap.

### Projective virtual symmetry of a matrix product state

↑ **Parent:** [Symmetry-protected topological phase](#symmetry-protected-topological-phase)

An on-site symmetry of an injective MPS acts on virtual indices by matrices defined up to phase. Their projective cohomology class is the one-dimensional SPT invariant.

#### Protected edge state of a symmetry-protected topological phase

↑ **Parent:** [Projective virtual symmetry of a matrix product state](#projective-virtual-symmetry-of-a-matrix-product-state)

On an open chain, a nontrivial virtual projective representation appears as edge degrees of freedom. Symmetry-preserving local perturbations cannot remove their projective class without a bulk phase transition or symmetry breaking.

### Cluster state

↑ **Parent:** [Symmetry-protected topological phase](#symmetry-protected-topological-phase)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cluster_state)

The one-dimensional cluster state is the common positive eigenstate of commuting stabilizers $Z_{j-1}X_jZ_{j+1}$ and realizes a nontrivial $\mathbb Z_2\times\mathbb Z_2$ SPT phase.

## Intrinsic topological order

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)

Intrinsic topological order survives without a protecting symmetry and is characterized by features such as topology-dependent ground-state degeneracy and anyonic excitations. One-dimensional bosonic gapped systems have no intrinsic topological order, although they can have [symmetry-protected topological order](#symmetry-protected-topological-phase).

<h2 id="kramers-wannier-duality">Kramers--Wannier duality</h2>

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kramers--Wannier_duality)

Kramers--Wannier duality exchanges order variables with domain-wall or disorder variables. In multiple dimensions it naturally appears as a tensor-network map with a nontrivial symmetry-sector kernel.

<h3 id="kramers-wannier-intertwiner">Kramers--Wannier intertwiner</h3>

↑ **Parent:** [Kramers--Wannier duality](#kramers-wannier-duality)

For a one-dimensional periodic spin chain, a Kramers--Wannier intertwiner maps vertex spins in the $X$ basis to edge domain walls. It obeys $D(X_iX_{i+1})=\widetilde Z_{i+1/2}D$ and $DZ_i=(\widetilde X_{i-1/2}\widetilde X_{i+1/2})D$ and identifies spin configurations related by the global $\mathbb Z_2$ symmetry.

<h3 id="kramers-wannier-projected-entangled-pair-operator">Kramers--Wannier projected entangled pair operator</h3>

↑ **Parent:** [Kramers--Wannier duality](#kramers-wannier-duality)

In two dimensions, vertex COPY tensors and edge XOR tensors form a PEPO that maps vertex spins to edge domain walls. Its image obeys a zero-flux constraint around every plaquette.

## One-form symmetry

↑ **Parent:** [Topological quantum matter](topological-quantum-matter.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/One-form_symmetry)

A one-form symmetry is generated on closed codimension-one manifolds and acts on line operators rather than local point operators.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)
