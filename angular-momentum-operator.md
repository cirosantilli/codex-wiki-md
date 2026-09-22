# Angular momentum operator

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Angular_momentum_operator)

**Table of contents**

- [Common eigenstate of two angular-momentum components](#common-eigenstate-of-two-angular-momentum-components)
- [Spin-independent axis-angle composition](#spin-independent-axis-angle-composition)
- [Half-ring sine-squared angular state](#half-ring-sine-squared-angular-state)
- [Angular momentum expectation](#angular-momentum-expectation)
- [Spherical tensor operator](#spherical-tensor-operator)
- [Atomic orientation](#atomic-orientation)
- [Axially symmetric quadratic orbital eigenfunction](#axially-symmetric-quadratic-orbital-eigenfunction)
- [Angular momentum lowering operator](#angular-momentum-lowering-operator)
  - [Normalized highest-weight lowering formula](#normalized-highest-weight-lowering-formula)
- [Angular momentum eigenstate](#angular-momentum-eigenstate)
- [Angular momentum commutation relations](#angular-momentum-commutation-relations)
- [Addition of angular momentum](#addition-of-angular-momentum)
  - [Magnetic-substate subtraction](#magnetic-substate-subtraction)
  - [Exchange parity of two coupled identical spins](#exchange-parity-of-two-coupled-identical-spins)
  - [Maximum total angular momentum of equivalent fermions](#maximum-total-angular-momentum-of-equivalent-fermions)
  - [Coupled angular-momentum state count](#coupled-angular-momentum-state-count)
  - [Three spin-one-half angular-momentum decomposition](#three-spin-one-half-angular-momentum-decomposition)
  - [LS coupling](#ls-coupling)
    - [Nonequivalent p-s and p-p term counting](#nonequivalent-p-s-and-p-p-term-counting)
    - [Allowed LS terms of a p-squared configuration](#allowed-ls-terms-of-a-p-squared-configuration)
  - [Total angular momentum operator](#total-angular-momentum-operator)
  - [Total-spin sector](#total-spin-sector)
    - [Three spin-one angular-momentum decomposition](#three-spin-one-angular-momentum-decomposition)
      - [Symmetric three-spin-one subspace](#symmetric-three-spin-one-subspace)
    - [Spin-one Cartesian basis](#spin-one-cartesian-basis)
      - [Spin-one reversal under quadratic anisotropy](#spin-one-reversal-under-quadratic-anisotropy)
    - [Spin-dot-product eigenvalue](#spin-dot-product-eigenvalue)
      - [Spin-three-halves pair spectrum](#spin-three-halves-pair-spectrum)
  - [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition)
    - [Lowest-weight coupling of two angular momenta](#lowest-weight-coupling-of-two-angular-momenta)
  - [Highest-weight states in angular momentum addition](#highest-weight-states-in-angular-momentum-addition)
  - [Singlet state](#singlet-state)
    - [Spin-one singlet state](#spin-one-singlet-state)
    - [Spin-one-half singlet state](#spin-one-half-singlet-state)
  - [Spin-one-half triplet state](#spin-one-half-triplet-state)
- [Spin](#spin)
  - [Total spin](#total-spin)
  - [Spin rotation](#spin-rotation)
  - [Spin operator](#spin-operator)
    - [Uniform-field spin precession](#uniform-field-spin-precession)
      - [Spin measurement in the yz plane](#spin-measurement-in-the-yz-plane)
    - [Spin-one-half quadratic anisotropy is constant](#spin-one-half-quadratic-anisotropy-is-constant)
  - [Spin contamination](#spin-contamination)
  - [Spin multiplicity](#spin-multiplicity)
  - [Two-spin XY Hamiltonian](#two-spin-xy-hamiltonian)
  - [Spin eigenstate](#spin-eigenstate)
  - [Spin-spin interaction](#spin-spin-interaction)
  - [Spin polarization](#spin-polarization)
    - [Beam spin polarization](#beam-spin-polarization)
    - [Spin texture](#spin-texture)
  - [Spin-rotation coupling](#spin-rotation-coupling)
  - [Spin relaxation](#spin-relaxation)
    - [Hanle spin-precession measurement](#hanle-spin-precession-measurement)
    - [Spin-memory loss](#spin-memory-loss)
    - [Spin diffusion length](#spin-diffusion-length)
    - [Spin-lattice relaxation](#spin-lattice-relaxation)
      - [Bloembergen-Purcell-Pound relaxation model](#bloembergen-purcell-pound-relaxation-model)
    - [Spin-flip scattering](#spin-flip-scattering)
  - [Jordan–Wigner transformation](#jordan-wigner-transformation)
    - [Bondwise cancellation of a Jordan-Wigner string](#bondwise-cancellation-of-a-jordan-wigner-string)
    - [Parity-dependent boundary condition of the Jordan-Wigner chain](#parity-dependent-boundary-condition-of-the-jordan-wigner-chain)
    - [Two-site Jordan-Wigner normalization and signs](#two-site-jordan-wigner-normalization-and-signs)
  - [Spin one-half](#spin-one-half)
    - [Electron spin](#electron-spin)
    - [Spin measurement](#spin-measurement)
    - [Spin one-half along an axis](#spin-one-half-along-an-axis)
  - [Stern-Gerlach experiment](#stern-gerlach-experiment)
    - [Neutron Stern-Gerlach splitting](#neutron-stern-gerlach-splitting)
    - [Stern-Gerlach apparatus in 1922](#stern-gerlach-apparatus-in-1922)
    - [Stern-Gerlach force and flight model](#stern-gerlach-force-and-flight-model)
    - [Stern-Gerlach discrete and classical profiles](#stern-gerlach-discrete-and-classical-profiles)
    - [Stern-Gerlach historical and modern interpretations](#stern-gerlach-historical-and-modern-interpretations)
  - [Holstein–Primakoff transformation](#holstein-primakoff-transformation)
    - [Holstein-Primakoff matrix-element proof](#holstein-primakoff-matrix-element-proof)
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
    - [Spin-one maximum-projection eigenvector](#spin-one-maximum-projection-eigenvector)
    - [Spin coherent-state path integral](#spin-coherent-state-path-integral)
    - [Equatorial spin-three-halves coherent state](#equatorial-spin-three-halves-coherent-state)
  - [Larmor precession](#larmor-precession)
    - [Larmor frequency](#larmor-frequency)
    - [Larmor precession of a spin coherent state](#larmor-precession-of-a-spin-coherent-state)
      - [Time evolution under a spin-Z Hamiltonian](#time-evolution-under-a-spin-z-hamiltonian)
  - [Heisenberg model](#heisenberg-model)
    - [Two-spin exchange spectrum with unequal signed magnetic moments](#two-spin-exchange-spectrum-with-unequal-signed-magnetic-moments)
      - [Spin-projection-protected crossings in an exchange spectrum](#spin-projection-protected-crossings-in-an-exchange-spectrum)
      - [Parallel-spin degeneracy for equal-and-opposite moments](#parallel-spin-degeneracy-for-equal-and-opposite-moments)
      - [Strong-field limit of a two-spin exchange spectrum](#strong-field-limit-of-a-two-spin-exchange-spectrum)
    - [XXZ spin chain](#xxz-spin-chain)
      - [Classical ground states of an XXZ spin chain](#classical-ground-states-of-an-xxz-spin-chain)
    - [Classical Heisenberg model](#classical-heisenberg-model)
      - [Classical Heisenberg mean-field partition function](#classical-heisenberg-mean-field-partition-function)
        - [Classical Heisenberg Langevin self-consistency](#classical-heisenberg-langevin-self-consistency)
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
- [Space quantization](#space-quantization)

## Common eigenstate of two angular-momentum components

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

A common eigenstate of $J_x$ and $J_y$ must satisfy $J_z\psi=0$ by their [commutator](lie-algebra.md#commutator). Applying the other angular-momentum [commutators](lie-algebra.md#commutator) then forces both remaining [eigenvalues](linear-operator-theory.md#eigenvalue) to vanish. Thus the state lies in a spin-zero sector. Noncommuting components do not possess a general common eigenbasis, but spin-zero states are an important exception to the claim that they can never share any eigenstate.

## Spin-independent axis-angle composition

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

The axis and angle of a product of [rotations](riemannian-geometry.md#rotation-mathematics) are properties of the group elements, independent of which [spin](#spin) [representation](representation-theory.md#group-representation) acts on a state. Higher-spin generators do not obey the two-term Pauli exponential, but [representations](representation-theory.md#group-representation) preserve the resulting [rotation](riemannian-geometry.md#rotation-mathematics) product. The central $2\pi$ [rotation](riemannian-geometry.md#rotation-mathematics) acts as $(-1)^{2S}I$.

## Half-ring sine-squared angular state

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

The normalized periodic state $\psi=\sqrt{8/(3\pi)}\sin^2\phi$ on $0<\phi<\pi$, zero on the remaining semicircle, has $\langle L_z\rangle=0$ and $\operatorname{Var}(L_z)=4\hbar^2/3$. Projection on $e^{i\phi}/\sqrt{2\pi}$ gives probability $64/(27\pi^2)$ for $L_z=\hbar$. Its first derivative is continuous at the joins, so integration by parts has no boundary contribution.

## Angular momentum expectation

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

For a normalized periodic angular [wavefunction](wave-function.md), $\langle L_z\rangle=-i\hbar\int_0^{2\pi}\psi^*\partial_\phi\psi\,d\phi$. A real periodic [wavefunction](wave-function.md) with matching boundary values has zero mean, even though nonzero angular momenta can have positive measurement probabilities.

## Spherical tensor operator

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

A rank-$k$ [spherical tensor operator](#spherical-tensor-operator) has components $T_q^{(k)}$, $-k\leq q\leq k$, that transform under [rotation](riemannian-geometry.md#rotation-mathematics) like an [angular momentum](momentum.md#angular-momentum) $k$. Equivalently, their [commutators](lie-algebra.md#commutator) with the [angular momentum operator](angular-momentum-operator.md) satisfy

$$
[J_z,T_q^{(k)}]=\hbar qT_q^{(k)},\qquad
[J_\pm,T_q^{(k)}]=\hbar\sqrt{k(k+1)-q(q\pm1)}\,T_{q\pm1}^{(k)}.
$$

For a vector operator, the rank is one and a conventional choice is $T_0=V_z$, $T_{\pm1}=\mp(V_x\pm iV_y)/\sqrt2$. The [Wigner-Eckart theorem](representation-theory.md#wigner-eckart-theorem) separates the [matrix elements](vector-space.md#matrix-element) of a [spherical tensor operator](#spherical-tensor-operator) into [Clebsch-Gordan coefficients](representation-theory.md#clebsch-gordan-coefficients) and a [reduced matrix element](representation-theory.md#reduced-matrix-element).

## Atomic orientation

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

A distribution of [quantum state populations](density-matrix.md#quantum-state-population) over atomic [magnetic sublevels](quantum-mechanics.md#magnetic-sublevel) with a nonzero [expectation value](quantum-system.md#expectation-value) of the [angular momentum operator](angular-momentum-operator.md) [vector](vector-space.md#vector).

## Axially symmetric quadratic orbital eigenfunction

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

Each [orbital angular momentum](quantum-mechanics.md#orbital-angular-momentum) operator annihilates a radial factor and $r^2$. Direct differentiation gives $L^2x_3^2=\hbar^2(6x_3^2-2r^2)$ and $L_3x_3^2=0$. Hence the displayed trace-free quadratic polynomial, times any admissible radial factor, has orbital labels $l=2,m=0$. Its angular dependence is proportional to the [spherical harmonic](analysis.md#spherical-harmonic) $Y_{20}$; subtracting $r^2/3$ removes the rotational scalar part.

## Angular momentum lowering operator

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

The operator $J_-=J_x-iJ_y$ acts by $J_-|j,m\rangle=\hbar\sqrt{(j+m)(j-m+1)}|j,m-1\rangle$. It generates lower magnetic states and determines [Clebsch-Gordan coefficients](representation-theory.md#clebsch-gordan-coefficients).

### Normalized highest-weight lowering formula

↑ **Parent:** [Angular momentum lowering operator](#angular-momentum-lowering-operator)

In an [irreducible spin representation](#irreducible-spin-representation), the [angular momentum lowering operator](#angular-momentum-lowering-operator) has squared [norm](normed-vector-space.md#norm) factor $(I+m)(I-m+1)$. Multiplying these factors from the [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) gives the factorial normalization displayed above. All factorial arguments are integers even when $I$ is half-integral. This produces a consistent positive-coefficient phase convention for all weight states and fixes signs in subsequent [isospin rotations](standard-model.md#isorotation).

## Angular momentum eigenstate

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

A joint eigenstate $|j,m\rangle$ of $J^2$ and $J_z$, with eigenvalues $\hbar^2j(j+1)$ and $\hbar m$. Its allowed labels satisfy $j\in\{0,1/2,1,\ldots\}$ and $m=-j,-j+1,\ldots,j$.

## Angular momentum commutation relations

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

Every angular momentum operator satisfies

$$
[J_i,J_j]=i\hbar\varepsilon_{ijk}J_k,
\qquad
[J^2,J_i]=0.
$$

## Addition of angular momentum

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Addition_of_angular_momentum)

For two subsystems, the total operator is $\mathbf J=\mathbf J_1\otimes I+I\otimes\mathbf J_2$, and $J_\pm=J_{1\pm}+J_{2\pm}$. The coupled basis diagonalizes $\mathbf J^2$ and $J_z$.

### Magnetic-substate subtraction

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

Let $d_M$ count states of fixed [angular momentum](momentum.md#angular-momentum) projection $M$ in a finite rotational representation, and $n_J$ its spin-$J$ multiplicity. Every spin-$J$ [irreducible representation](representation-theory.md#irreducible-representation) contributes one state at each $M=-J,\ldots,J$. Thus $d_M=\sum_{J\geq M}n_J$ for nonnegative $M$, and subtraction gives $n_J=d_J-d_{J+1}$. Counting occupation states first incorporates [Bose-Einstein statistics](quantum-ideal-gas-statistics.md#bose-einstein-statistics) before decomposing identical-boson angular states.

### Exchange parity of two coupled identical spins

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

Exchanging the factors in the [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition) of two equal [spins](#spin) gives the phase $(-1)^{2s-j}$. This follows from the exchange symmetry of the [Clebsch-Gordan coefficients](representation-theory.md#clebsch-gordan-coefficients). The total exchange parity includes the spatial state and any other internal factors: the spin parity alone does not impose the full [symmetrization postulate](tensor-product-of-quantum-systems.md#symmetrization-postulate). For two half-integer [spins](#spin), even $j$ is spin-antisymmetric and odd $j$ spin-symmetric.

### Maximum total angular momentum of equivalent fermions

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

For $N$ identical [fermions](tensor-product-of-quantum-systems.md#fermion) restricted to one angular-momentum multiplet $j$, with all other one-particle labels fixed, the [Pauli exclusion principle](tensor-product-of-quantum-systems.md#pauli-exclusion-principle) permits distinct [angular momentum](momentum.md#angular-momentum) projections $j,j-1,\ldots,j-N+1$. Their sum is $Nj-N(N-1)/2$, provided $N\leq2j+1$. The resulting [Slater determinant](tensor-product-of-quantum-systems.md#slater-determinant) is killed by the total raising [angular momentum ladder operator](quantum-mechanics.md#angular-momentum-ladder-operator) because raising any occupied state either exceeds $j$ or duplicates an occupied state. It is therefore a [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) of precisely this total [angular momentum](momentum.md#angular-momentum). The formula is invariant under replacing particles by holes in the full shell.

### Coupled angular-momentum state count

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

Coupling orbital [angular momentum](momentum.md#angular-momentum) $L>0$ to [spin one-half](#spin-one-half) produces $J=L\pm1/2$. The [dimensions](vector-space.md#dimension-vector-space) add as $(2L+2)+2L=2(2L+1)$. A change between coupled and product [bases](vector-space.md#basis) changes labels, not the [dimension](vector-space.md#dimension-vector-space) of the [Hilbert space](hilbert-space.md).

### Three spin-one-half angular-momentum decomposition

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

For three distinguishable [spin one-half](#spin-one-half) systems, the [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition) first combines two spins into $0\oplus1$, then couples the third: $0\otimes1/2=1/2$ and $1\otimes1/2=1/2\oplus3/2$. Thus the [tensor product](multilinear-algebra.md#tensor-product) has one quartet and two doublets. A [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) depending only on the total $S^2$ and $S_z$ acts identically on the two doublet copies. In particular $H=\epsilon_tS^2/\hbar^2+\epsilon_zS_z/\hbar$ has [energy eigenvalues](energy-eigenvalue.md) $\epsilon_tS(S+1)+\epsilon_zM$, generically once for each quartet projection and twice for each doublet projection. Equal numerical energies have their multiplicities added.

### LS coupling

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

An atomic [addition of angular momentum](#addition-of-angular-momentum) scheme in which the individual [orbital angular momentum](quantum-mechanics.md#orbital-angular-momentum) vectors first combine into $\mathbf L$ and the individual [spins](#spin) into $\mathbf S$, then these combine into total [angular momentum](momentum.md#angular-momentum) $\mathbf J$. When [spin-orbit coupling](atomic-physics.md#spin-orbit-interaction) is weak compared with the interactions between [electrons](physics.md#electron) described by [electrostatics](electrostatics.md), $L$ and $S$ remain useful approximate [quantum numbers](quantum-system.md#quantum-number). The [Landé g-factor](atomic-physics.md#lande-g-factor) describes the resulting weak-field magnetic splitting.

#### Nonequivalent p-s and p-p term counting

↑ **Parent:** [LS coupling](#ls-coupling)

For electrons in distinct radial orbitals, angular coupling permits all $L$ from $|l_1-l_2|$ to $l_1+l_2$ and both total [spins](#spin) $S=0,1$. A p-s pair therefore gives singlet and triplet P terms. A nonequivalent p-p pair gives singlet and triplet S, P and D terms. The equivalent-subshell exclusion restrictions do not remove these nonequivalent terms. Counting $(2S+1)(2L+1)$ gives 12 p-s and 36 p-p microstates, matching products of one-electron state counts.

#### Allowed LS terms of a p-squared configuration

↑ **Parent:** [LS coupling](#ls-coupling)

Two equivalent $l=1$ [electrons](physics.md#electron) require an antisymmetric complete state. Orbital exchange has [parity](quantum-mechanics.md#parity) $(-1)^L$ and the [spin](#spin) singlet is antisymmetric, giving allowed $L+S$ even. The terms are ${}^3P_{0,1,2}$, ${}^1D_2$ and ${}^1S_0$, with $9+5+1=15$ states, equal to $\binom62$. Hund ordering puts ${}^3P_0$ lowest for the less-than-half-filled configuration.

### Total angular momentum operator

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

For a composite quantum system, the total angular momentum operator is the sum of the constituent angular momenta, with each summand acting on its own tensor factor. Its simultaneous eigenstates with $J_z$ organize the state space into [total-spin sectors](#total-spin-sector).

### Total-spin sector

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

A total-spin-$J$ sector is an irreducible subspace on which $\mathbf J^2$ has eigenvalue $J(J+1)\hbar^2$. For two spin-one particles, [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition) gives sectors $J=0,1,2$ of dimensions one, three, and five.

#### Three spin-one angular-momentum decomposition

↑ **Parent:** [Total-spin sector](#total-spin-sector)

Coupling three distinguishable spin-one systems gives

$$
1\otimes1\otimes1
=0\oplus3(1)\oplus2(2)\oplus3,
$$

where the labels denote total spin and coefficients denote multiplicities. The dimensions are respectively $1$, $3\cdot3$, $2\cdot5$, and $7$, summing to $27$.

##### Symmetric three-spin-one subspace

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

#### Spin-one Cartesian basis

↑ **Parent:** [Total-spin sector](#total-spin-sector)

The spin-one Cartesian basis $|x\rangle,|y\rangle,|z\rangle$ transforms as a three-dimensional vector under rotations. In its two-site tensor square, the scalar, antisymmetric, and symmetric traceless subspaces are respectively the total-spin $0$, $1$, and $2$ sectors.

##### Spin-one reversal under quadratic anisotropy

↑ **Parent:** [Spin-one Cartesian basis](#spin-one-cartesian-basis)

For a spin-one [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) $H=AS_z^2+B(S_x^2-S_y^2)$, Cartesian basis energies are $\hbar^2(A-B)$, $\hbar^2(A+B)$ and zero along the $x,y,z$ basis labels. The $S_x=\hbar$ state combines the latter two basis vectors equally. Their relative phase produces the displayed spin-reversal probability. Complete reversal occurs at odd multiples of $\pi/(|A+B|\hbar)$ if $A+B\ne0$; when it vanishes those two components remain degenerate. Individual matrix signs depend on basis conventions, while the [commutators](lie-algebra.md#commutator) and physical probability must remain consistent.

#### Spin-dot-product eigenvalue

↑ **Parent:** [Total-spin sector](#total-spin-sector)

For two spins of magnitude $s$, $\mathbf S_1\mathbin\cdot\mathbf S_2=\tfrac12(\mathbf J^2-\mathbf S_1^2-\mathbf S_2^2)$. For two spin-one particles its eigenvalues in total-spin sectors $J=0,1,2$ are $-2,-1,1$ in units of $\hbar^2$.

##### Spin-three-halves pair spectrum

↑ **Parent:** [Spin-dot-product eigenvalue](#spin-dot-product-eigenvalue)

For $s_1=s_2=3/2$, [angular momentum addition](momentum.md#angular-momentum-addition) gives one copy of $j=0,1,2,3$. The identity $2\mathbf S_1\cdot\mathbf S_2=\mathbf J^2-\mathbf S_1^2-\mathbf S_2^2$ gives the four [eigenvalues](linear-operator-theory.md#eigenvalue) in the title, with [state degeneracy](statistical-physics.md#state-degeneracy) $1,3,5,7$. These exhaust the $4\times4$ spin space. If the particles are identical [fermions](tensor-product-of-quantum-systems.md#fermion), an appropriate spatial exchange parity accommodates each sector; only a specified spatial restriction can remove sectors.

### Clebsch-Gordan decomposition

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

The tensor product of spin-$j_1$ and spin-$j_2$ irreducible representations decomposes into one copy of each spin

$$
j=|j_1-j_2|,|j_1-j_2|+1,\ldots,j_1+j_2.
$$

The change-of-basis entries between uncoupled and coupled states are Clebsch--Gordan coefficients.

#### Lowest-weight coupling of two angular momenta

↑ **Parent:** [Clebsch-Gordan decomposition](#clebsch-gordan-decomposition)

Put $s=j_1+j_2$, with both $j_i>0$. At magnetic quantum number $-s+1$, let $|a\rangle$ raise only the first factor of the lowest product state and $|b\rangle$ raise only the second. Applying total $J_+$ to the lowest product gives the normalized $J=s$ combination $\sqrt{j_1/s}|a\rangle+\sqrt{j_2/s}|b\rangle$. Its orthogonal combination is annihilated by total $J_-$ and therefore has $J=s-1$. This obtains a useful [Clebsch-Gordan coefficients](representation-theory.md#clebsch-gordan-coefficients) without a table.

### Highest-weight states in angular momentum addition

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)

With $J=j_1+j_2$, the maximal state is the product $|J,J\rangle=|j_1,j_1\rangle|j_2,j_2\rangle$. Lowering it once gives

$$
|J,J-1\rangle=
\sqrt{\frac{j_1}{J}}|j_1,j_1-1\rangle|j_2,j_2\rangle
+\sqrt{\frac{j_2}{J}}|j_1,j_1\rangle|j_2,j_2-1\rangle.
$$

The orthogonal combination is the highest-weight state $|J-1,J-1\rangle$.

### Singlet state

↑ **Parent:** [Addition of angular momentum](#addition-of-angular-momentum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singlet_state)

Two equal spins $j$ have the unique total-spin-zero state

$$
|0,0\rangle=\frac1{\sqrt{2j+1}}
\sum_{m=-j}^j(-1)^{j-m}|j,m\rangle|j,-m\rangle.
$$

It is invariant under joint rotations.

A [singlet state](#singlet-state) is the one-dimensional rotation representation; this construction supplies the angular-momentum-zero case for two equal spins.

#### Spin-one singlet state

↑ **Parent:** [Singlet state](#singlet-state)

In the product basis $|m_1,m_2\rangle$ for two spin-one particles, total magnetic quantum number zero allows only $|1,-1\rangle$, $|0,0\rangle$ and $|-1,1\rangle$. Applying the total [ladder operators](semisimple-lie-algebra.md#ladder-operator) to $\alpha|1,-1\rangle+\beta|0,0\rangle+\gamma|-1,1\rangle$ gives

$$
S_+|\psi\rangle=\sqrt2\hbar[(\alpha+\beta)|1,0\rangle+(\beta+\gamma)|0,1\rangle].
$$

A [singlet state](#singlet-state) is annihilated by $S_+$ and $S_-$, so $\alpha=\gamma=-\beta$. [Wavefunction normalization](wave-function.md#wavefunction-normalization) gives the displayed state, up to an overall phase. Here the ket on the left of the title formula has total-spin labels, while its right-hand kets have individual magnetic labels. The state is symmetric under exchanging the particles, although no exchange constraint is needed for distinguishable particles.

#### Spin-one-half singlet state

↑ **Parent:** [Singlet state](#singlet-state)

For two spin-one-half particles, the singlet is

$$
|0,0\rangle=\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2}.
$$

Every component of the total spin annihilates it, and $\mathbf S^2$ has eigenvalue zero.

### Spin-one-half triplet state

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

## Spin

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_(physics))

Spin operators satisfy $[S_i,S_j]=i\hbar\varepsilon_{ijk}S_k$ and are Hermitian traceless generators of rotations in finite-dimensional irreducible representations.

### Total spin

↑ **Parent:** [Spin](#spin)

The [total spin](#total-spin) is the [vector](vector-space.md#vector) sum of subsystem [spin operators](#spin-operator) and generates their simultaneous [rotation](riemannian-geometry.md#rotation-mathematics). For a rotationally invariant [Heisenberg model](#heisenberg-model), both its squared magnitude and any chosen component commute with the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). An anisotropic exchange or field can preserve only a component.

### Spin rotation

↑ **Parent:** [Spin](#spin)

A [spin rotation](#spin-rotation) acts on a [quantum state](quantum-system.md#quantum-state) through the [unitary representation](representation-theory.md#unitary-representation) generated by its [angular momentum operators](angular-momentum-operator.md). With $\hbar=1$, [rotation](riemannian-geometry.md#rotation-mathematics) by angle $\theta$ about axis $\hat{\mathbf n}$ is $e^{-i\theta\hat{\mathbf n}\cdot\mathbf S}$. Simultaneously rotating every site is a global [symmetry](physics.md#symmetry-physics) of an isotropic [Heisenberg model](#heisenberg-model).

### Spin operator

↑ **Parent:** [Spin](#spin)

A [spin operator](#spin-operator) describes intrinsic [angular momentum](momentum.md#angular-momentum). Its components obey angular-momentum [commutators](lie-algebra.md#commutator); for spin one half, $\hat S_j=\hbar\sigma_j/2$ in terms of the [Pauli matrices](algebra.md#pauli-matrices).

#### Uniform-field spin precession

↑ **Parent:** [Spin operator](#spin-operator)

For a spin-half particle with $H=\alpha\mathbf B\cdot\mathbf S$ and $\mathbf S=\hbar\boldsymbol\sigma/2$, exponentiating the [Pauli matrices](algebra.md#pauli-matrices) gives a rotation about the field axis. A field along $y$ evolves initial $z$-up [spin](#spin) to $(\cos(\alpha Bt/2),\sin(\alpha Bt/2))^T$. The sign of $\alpha$ sets the precession direction. [spin](#spin) parallel to the field is conserved even while transverse components vary.

##### Spin measurement in the yz plane

↑ **Parent:** [Uniform-field spin precession](#uniform-field-spin-precession)

For a state initially $z$-up and precessing about $y$, measurement along $\mathbf n=(0,\sin\theta,\cos\theta)$ has the displayed [probabilities](probability-theory.md#probability). [eigenvectors](linear-operator-theory.md#eigenvector) can be chosen as $(\cos(\theta/2),i\sin(\theta/2))^T$ and $(i\sin(\theta/2),\cos(\theta/2))^T$. Their [phases](wave.md#phase-waves) must be retained when taking [inner products](inner-product.md). Full $2\pi$ rotation changes their signs but leaves isolated-state [probabilities](probability-theory.md#probability) unchanged.

#### Spin-one-half quadratic anisotropy is constant

↑ **Parent:** [Spin operator](#spin-operator)

For [spin](#spin) one-half, the Pauli representation makes every diagonal quadratic component a multiple of the identity. Thus $AS_z^2+B(S_x^2-S_y^2)=A\hbar^2I/4$ cannot split the doublet or cause [spin](#spin) reversal. This conclusion is special to this quadratic [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) and does not exclude linear Zeeman dynamics.

### Spin contamination

↑ **Parent:** [Spin](#spin)

A [wavefunction](wave-function.md) intended for a specified total-spin state contains components of other total spins. For an unrestricted [determinant](multilinear-algebra.md#determinant) with one alpha and one beta orbital, $\langle S^2\rangle=1-|\langle\phi_\alpha|\phi_\beta\rangle|^2$ in units of $\hbar^2$.

### Spin multiplicity

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_multiplicity)

A state with total [spin angular momentum](#spin) quantum number $S$ has $2S+1$ magnetic projections. A [singlet state](#singlet-state) has $S=0$, a [triplet state](#spin-one-half-triplet-state) has $S=1$, and the $S=3$ [chromium](chemical-substance.md#chromium) ground term is a septet.

### Two-spin XY Hamiltonian

↑ **Parent:** [Spin](#spin)

The two-site quantum version of an [XY model](statistical-physics.md#xy-model) couples the transverse components of two [spin one-half](#spin-one-half) degrees of freedom. In the ordered basis $|\uparrow\uparrow\rangle,|\uparrow\downarrow\rangle,|\downarrow\uparrow\rangle,|\downarrow\downarrow\rangle$, its only off-diagonal entries are $H_{23}=H_{32}=-2J$. The parallel states have [energies](energy.md) $-2h$ and $2h$; the symmetric and antisymmetric opposite-spin combinations have [energies](energy.md) $-2J$ and $2J$ respectively. The latter is the [singlet state](#singlet-state). The formulas remain valid at accidental degeneracies.

### Spin eigenstate

↑ **Parent:** [Spin](#spin)

A spin eigenstate along a specified axis is a simultaneous [eigenstate](energy-eigenvalue.md#eigenstate) of the squared [spin](#spin) operator $S^2$ and its component $S_{\hat n}$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $\hbar^2s(s+1)$ and $\hbar m$, where $m=-s,-s+1,\ldots,s$. The axis must be specified because components along different axes generally do not commute. For [spin one-half](#spin-one-half), the two field-axis eigenstates have projections $\pm\hbar/2$ and form the branches of a [Stern-Gerlach experiment](#stern-gerlach-experiment).

### Spin-spin interaction

↑ **Parent:** [Spin](#spin)

A [spin-spin interaction](#spin-spin-interaction) couples two [spin angular momenta](#spin). In an isotropic model it is proportional to their [dot product](inner-product.md#dot-product), whose expectation in a total-pair-spin state follows from $2\mathbf S_i\cdot\mathbf S_j=S_{ij}^2-S_i^2-S_j^2$. Magnetic interactions generate examples in atoms and effective colour-magnetic interactions in [hadron](physics.md#hadron) models.

### Spin polarization

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_polarization)

For a spin-one-half ensemble, [spin polarization](#spin-polarization) measures unequal occupation or coherent alignment of [spin](#spin) states. A spin-dependent energy splitting does not alone determine the ensemble's response: occupation, [temperature](temperature.md) and [spin relaxation](#spin-relaxation) matter. A [spin polarization](#spin-polarization) is distinct from a net change of [charge density](electric-charge.md#charge-density) and from the optical [polarization of waves](wave.md#polarization-waves).

#### Beam spin polarization

↑ **Parent:** [Spin polarization](#spin-polarization)

A beam's unequal population of [spin](#spin) projections along a specified axis. For spin-one-half particles the displayed [longitudinal polarization](wave-equation.md#longitudinal-polarization) uses populations parallel and antiparallel to the [momentum](momentum.md). An unpolarized beam has equal populations and requires an initial-spin average in a [cross section](physics.md#cross-section-physics); a polarized beam weights the corresponding [helicity](special-relativity.md#helicity) amplitudes differently. This differs from [photon](quantum-mechanics.md#photon) linear polarization.

#### Spin texture

↑ **Parent:** [Spin polarization](#spin-polarization)

A spin texture describes how a [spin expectation value](quantum-system.md#spin-expectation-value) or [spin polarization](#spin-polarization) varies with [position](classical-mechanics.md#position) or [wavevector](elasticity-physics.md#wavevector). It specifies a [vector field](multivariable-calculus.md#vector-field), including its magnitude when that matters; a direction field alone is undefined wherever that magnitude vanishes. A [Rashba spin texture](atomic-physics.md#rashba-spin-texture) is an example in which [spin expectation values](quantum-system.md#spin-expectation-value) wind around circles in the plane of [wavevectors](elasticity-physics.md#wavevector).

### Spin-rotation coupling

↑ **Parent:** [Spin](#spin)

The [spin-rotation coupling](#spin-rotation-coupling) contribution to a rotating-frame [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) couples [angular velocity](rigid-body-dynamics.md#angular-velocity) to [angular momentum](momentum.md#angular-momentum). When discussing [spin](#spin) alone, identify which part of the total [angular momentum](momentum.md#angular-momentum) enters the effective model.

### Spin relaxation

↑ **Parent:** [Spin](#spin)

#### Hanle spin-precession measurement

↑ **Parent:** [Spin relaxation](#spin-relaxation)

A transverse magnetic field rotates a nonequilibrium [spin polarization](#spin-polarization) while diffusion and [spin relaxation](#spin-relaxation) redistribute it. The field dependence of a detector signal can constrain spin lifetime and transport parameters. A distribution of diffusion times and rotation of the injecting/detecting electrodes must be included when relevant.

#### Spin-memory loss

↑ **Parent:** [Spin relaxation](#spin-relaxation)

Loss of transported spin polarization at an interface, distinct from bulk spin relaxation in an adjacent layer.

#### Spin diffusion length

↑ **Parent:** [Spin relaxation](#spin-relaxation)

The distance over which a nonequilibrium spin imbalance decays appreciably in a diffusive conductor. In a simple diffusion-relaxation model it is $\ell_s=\sqrt{D\tau_s}$; interfaces can contribute additional spin-memory loss.

#### Spin-lattice relaxation

↑ **Parent:** [Spin relaxation](#spin-relaxation)

Exchange of [energy](energy.md) between magnetic [spin](#spin) degrees of freedom and the surrounding lattice, allowing their [temperatures](temperature.md) to approach [thermal equilibrium](thermal-equilibrium.md). It permits [adiabatic demagnetization](temperature.md#adiabatic-demagnetization) to cool a solid and its attached load.

##### Bloembergen-Purcell-Pound relaxation model

↑ **Parent:** [Spin-lattice relaxation](#spin-lattice-relaxation)

A model using exponentially correlated magnetic fluctuations. For homonuclear dipolar relaxation, $T_1^{-1}=C[\tau_c/(1+\omega_0^2\tau_c^2)+4\tau_c/(1+4\omega_0^2\tau_c^2)]$. Its rate maximum occurs near $\omega_0\tau_c=0.616$; a single-frequency Lorentzian instead peaks at one.

#### Spin-flip scattering

↑ **Parent:** [Spin relaxation](#spin-relaxation)

<h3 id="jordan-wigner-transformation">Jordan–Wigner transformation</h3>

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan–Wigner_transformation)

The Jordan–Wigner transformation represents a one-dimensional [spin one-half](#spin-one-half) chain by fermions with a parity string preceding each site. With $P_n=\prod_{m<n}(1-2n_m)$, one has $S_n^+=P_nc_n$ and $S_n^z=1/2-n_n$. The string converts the off-site [canonical anticommutation relations](supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations) into commuting spin operators. Adjacent exchange terms become quadratic fermion expressions, while a periodic end bond depends on global [fermion parity](topological-quantum-matter.md#fermion-parity).

#### Bondwise cancellation of a Jordan-Wigner string

↑ **Parent:** [Jordan–Wigner transformation](#jordan-wigner-transformation)

For $S_n^+=P_nc_n$ with $P_n=\prod_{m<n}(1-2c_m^\dagger c_m)$, neighbouring [Jordan–Wigner transformation](#jordan-wigner-transformation) strings differ by only the local parity factor. The [canonical anticommutation relations](supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations) give $(c_n+c_n^\dagger)(1-2c_n^\dagger c_n)=c_n^\dagger-c_n$, proving the displayed local [spin](#spin) identity. The closing bond of a periodic chain instead retains total [fermion parity](topological-quantum-matter.md#fermion-parity); cancellation on bulk bonds does not justify discarding that global sector.

#### Parity-dependent boundary condition of the Jordan-Wigner chain

↑ **Parent:** [Jordan–Wigner transformation](#jordan-wigner-transformation)

For $S_n^+=\prod_{m<n}(1-2n_m)c_n$ and periodic [spins](#spin), the end exchange term carries the global [fermion parity](topological-quantum-matter.md#fermion-parity) $P=(-1)^{N_f}$. Replacing the end bond by a uniform hopping expression requires $c_{N+1}=-Pc_1$: even parity gives antiperiodic [fermions](tensor-product-of-quantum-systems.md#fermion), odd parity periodic [fermions](tensor-product-of-quantum-systems.md#fermion). Each resulting quadratic spectrum must be restricted to states of the parity used in its [boundary condition](differential-equation.md#boundary-condition).

#### Two-site Jordan-Wigner normalization and signs

↑ **Parent:** [Jordan–Wigner transformation](#jordan-wigner-transformation)

With occupied fermion sites representing up-spins, use $s_1^-=f_1$, $s_2^-=P_1f_2$ and $P_1=(-1)^{n_1}=1-2n_1$. The [canonical anticommutation relations](supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations) imply $P_1^2=I$, $P_1f_1=-f_1P_1$ and $[P_1,f_2]=0$. Consequently the two sites commute as spin operators, while $[s_j^-,s_j^+]=1-2n_j=-\sigma_j^z$. This normalization is essential: the unscaled combinations $\sigma_j^x\pm i\sigma_j^y$ are twice $s_j^\pm$.

The [two-spin XY Hamiltonian](#two-spin-xy-hamiltonian) becomes

$$
H=2h-2h(n_1+n_2)-2J(f_1^\dagger f_2+f_2^\dagger f_1).
$$

In particular, $f_1^\dagger P_1=f_1^\dagger$ and $f_1P_1=-f_1$ fix the hopping signs. The modes $b=(f_1+f_2)/\sqrt2$ and $c=(f_1-f_2)/\sqrt2$ preserve the [canonical anticommutation relations](supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations) and give $H=2h+(-2h-2J)b^\dagger b+(-2h+2J)c^\dagger c$.

### Spin one-half

↑ **Parent:** [Spin](#spin)

In units $\hbar=1$, spin one-half is the two-dimensional irreducible [spin angular momentum](#spin) representation with components $S_i=\sigma_i/2$. The [Pauli matrices](algebra.md#pauli-matrices) give [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm1/2$ along every unit axis. The normalized $x$-axis states are $(|\uparrow_z\rangle\pm|\downarrow_z\rangle)/\sqrt2$.

#### Electron spin

↑ **Parent:** [Spin one-half](#spin-one-half)

An [electron](physics.md#electron) has [spin one-half](#spin-one-half). Its intrinsic [spin angular momentum](#spin) has two possible components, $\pm\hbar/2$, along a specified [unit vector](vector-space.md#unit-vector) $\mathbf n$. These are the two [eigenvalues](linear-operator-theory.md#eigenvalue) of the corresponding [spin measurement](#spin-measurement); the [spin](#spin) is distinct from the electron's [orbital angular momentum](quantum-mechanics.md#orbital-angular-momentum).

#### Spin measurement

↑ **Parent:** [Spin one-half](#spin-one-half)

For a [spin one-half](#spin-one-half) system, an ideal [projective measurement](quantum-measurement.md#projective-measurement) along a [unit vector](vector-space.md#unit-vector) $\mathbf n$ measures $\sigma_{\mathbf n}=\mathbf n\cdot\boldsymbol\sigma$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $\pm1$, corresponding to physical [spin angular momentum](#spin) components $\pm\hbar/2$, and its [orthogonal projections](hilbert-space.md#orthogonal-projection) are $\Pi_\pm=(I\pm\sigma_{\mathbf n})/2$. For [density matrix](density-matrix.md) $\rho=(I+\mathbf r\cdot\boldsymbol\sigma)/2$, the [Born rule](wave-function.md#born-rule) and the [Pauli matrix multiplication law](algebra.md#pauli-matrix-multiplication-law) give the displayed [probabilities](probability-theory.md#probability). Thus a [spin measurement](#spin-measurement) along one direction tests only that component of the [Bloch vector](density-matrix.md#bloch-vector); measurements along three independent directions determine the entire [density matrix](density-matrix.md).

#### Spin one-half along an axis

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

### Stern-Gerlach experiment

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stern–Gerlach_experiment)

A [Stern-Gerlach experiment](#stern-gerlach-experiment) separates atomic beams according to a component of their [magnetic moment](electromagnetism.md#magnetic-dipole-moment) in a nonuniform [magnetic field](magnetic-field.md). For an appropriate two-state [spin](#spin) system, calibrated outputs distinguish the two [spin](#spin) [eigenvalues](linear-operator-theory.md#eigenvalue); [Stern-Gerlach expectation estimation](quantum-system.md#stern-gerlach-expectation-estimation) explains how repeated fresh preparations turn channel counts into an [expectation value](quantum-system.md#expectation-value).

The decisive contrast is between two separated components of an [atomic beam](physics.md#atomic-beam) and the continuous spread predicted for randomly oriented classical [magnetic moments](electromagnetism.md#magnetic-dipole-moment). Neither component need be an infinitely narrow spot: [velocity](classical-mechanics.md#velocity) spread and the resolving power of the [scientific instrument](physics.md#scientific-instrument) affect the spatial image. The apparatus converts an internal [magnetic moment](electromagnetism.md#magnetic-dipole-moment) into a displacement large enough to inspect, connecting [angular momentum eigenstates](#angular-momentum-eigenstate) to macroscopic evidence.

#### Neutron Stern-Gerlach splitting

↑ **Parent:** [Stern-Gerlach experiment](#stern-gerlach-experiment)

An electrically neutral [neutron](neutron.md) still has a [magnetic moment](electromagnetism.md#magnetic-dipole-moment) $\boldsymbol\mu=\gamma_n\mathbf S$. A collimated beam passing through an inhomogeneous [magnetic field](magnetic-field.md) experiences the force derived from $H=-\boldsymbol\mu\cdot\mathbf B$. In a region whose field axis is approximately fixed, a [spin one-half](#spin-one-half) neutron has two field-axis [spin eigenstates](#spin-eigenstate), producing two allowed transverse forces and two separated beam components after a drift. A homogeneous field can cause [Larmor precession](#larmor-precession) but cannot separate positions through this force.

The neutron's negative [gyromagnetic ratio](electromagnetism.md#gyromagnetic-ratio) interchanges which spin projection moves toward increasing field; it does not change the number of branches. An unpolarized beam gives equal ideal populations. A beam prepared in one field-axis eigenstate populates only one branch, so splitting into two observed spots presupposes both components and sufficient spatial resolution.

#### Stern-Gerlach apparatus in 1922

↑ **Parent:** [Stern-Gerlach experiment](#stern-gerlach-experiment)

In 1922, [Otto Stern](physicist.md#otto-stern) and [Walther Gerlach](physicist.md#walther-gerlach) used an electrically heated oven to emit neutral [silver](chemical-substance.md#silver) [chemical atoms](physics.md#atom-physics). Two platinum apertures, a pinhole and a slit $0.03$–$0.04\,\mathrm{mm}$ wide, supplied [collimation](optical-instrument.md#collimation). The beam passed along a $3.5\,\mathrm{cm}$ knife-edge pole in a nonuniform [magnetic field](magnetic-field.md). At its end, a glass plate collected the condensed [silver](chemical-substance.md#silver). Continuous pumping maintained [vacuum](physics.md#vacuum); the thin deposit required development even after eight hours.[Experimental setup, paragraphs 1–5; original 1922 paper in Martin Bauer's translation, PDF pp. 2–3](physics-bibliography.md#der-experimentelle-nachweis-der-richtungsquantelung-im-magnetfeld-by-walther-gerlach-and-otto-stern)

The field-off image established the undeflected slit width. A comparison put field-on and field-off deposits on the same plate. Microscopy revealed two deflected bands, no detectable central component, and broadening attributed to the [velocity](classical-mechanics.md#velocity) distribution. Alignment and distance from the knife-edge affected the pattern; precise [magnetic field](magnetic-field.md) [gradient](multivariable-calculus.md#gradient) measurements were still pending.[Results, Figs. 2–5 and observations b–e; closing paragraph, PDF pp. 3–5](physics-bibliography.md#der-experimentelle-nachweis-der-richtungsquantelung-im-magnetfeld-by-walther-gerlach-and-otto-stern)

The apertures act as a [collimator](optical-instrument.md#collimator): they constrain the initial transverse [positions](classical-mechanics.md#position) and [velocities](classical-mechanics.md#velocity), so a magnetic displacement can be distinguished from an initially broad beam. [Vacuum](physics.md#vacuum) reduces collisions that would destroy this preparation. Deposition integrates arrivals over the exposure; a darkened band is not a time-resolved record of individual [chemical atoms](physics.md#atom-physics). The field-off comparison tests whether the magnet changes the spatial distribution, while alignment checks address a geometric source of apparent asymmetry. Finite sensitivity qualifies the absence of a central deposit: it is an experimental upper limit, not a proof that exactly zero atoms landed there.

<a id="image-from-an-oven-to-a-silver-deposit-and-a-separate-ideal-flight-model"></a>
![](stern-gerlach-oven-to-deposit.png)

**[Figure 1](#image-from-an-oven-to-a-silver-deposit-and-a-separate-ideal-flight-model). From an oven to a silver deposit, and a separate ideal flight model**. The upper schematic shows the historical sequence without reproducing the original image. The lower diagram introduces the hypothetical constant-gradient magnet length $\ell$ and additional drift distance $D$ used below. The historical plate was at the magnet exit; the extra drift is a modeling choice.

#### Stern-Gerlach force and flight model

↑ **Parent:** [Stern-Gerlach experiment](#stern-gerlach-experiment)

Let the [atomic beam](physics.md#atomic-beam) travel along $x$, with [velocity](classical-mechanics.md#velocity) $v>0$, and let $z$ measure displacement along the dominant [magnetic field](magnetic-field.md) [gradient](multivariable-calculus.md#gradient). For a fixed effective [magnetic moment](electromagnetism.md#magnetic-dipole-moment) component $\mu_z$, the [magnetic dipole potential energy](electromagnetism.md#magnetic-dipole-potential-energy) is $U\simeq-\mu_zB_z$. Taking its negative [partial derivative](multivariable-calculus.md#partial-derivative) gives

$$
F_z=-\frac{\partial U}{\partial z}\simeq\mu_z\frac{\partial B_z}{\partial z}=\mu_zG.
$$

A spatially uniform [magnetic field](magnetic-field.md) can produce [torque](momentum.md#torque) and [Larmor precession](#larmor-precession), but cannot produce this translational separation. In a [quantum state](quantum-system.md#quantum-state) following a local internal [energy eigenvalue](energy-eigenvalue.md) $E_n(B)$, the more general expression is $F_z=-\partial_zE_n$, with effective [magnetic moment](electromagnetism.md#magnetic-dipole-moment) $-\partial E_n/\partial B$. Treating that moment as constant is an approximation with a physical regime, not an extra measured fact. Assume the local [magnetic field](magnetic-field.md) direction stays nearly fixed across the sampled beam, and that internal states follow it without transitions, as in the [adiabatic theorem](quantum-theory.md#adiabatic-theorem). The scalar [gradient](multivariable-calculus.md#gradient) model describes the beam's neighborhood; it omits the full [magnetic field](magnetic-field.md)'s transverse components and fringe regions.

Assume a constant $G$ over magnet length $\ell$, followed by a field-free drift $D$. Neglect transverse motion at entry and changes in longitudinal [velocity](classical-mechanics.md#velocity). [Newton's second law](force.md#newton-s-second-law) gives transverse [acceleration](classical-mechanics.md#acceleration) $a_z=\mu_zG/M$ for whole-atom [mass](classical-mechanics.md#mass) $M$. The magnet transit time is $t_m=\ell/v$, and the drift time is $t_d=D/v$. The magnet supplies both a displacement and an exit transverse [velocity](classical-mechanics.md#velocity):

$$
z_m-z_0=\frac{a_zt_m^2}{2},\qquad
v_{z,m}=a_zt_m,\qquad
z_s-z_0=\frac{\mu_zG}{Mv^2}\left(\frac{\ell^2}{2}+\ell D\right).
$$

The $\ell D$ contribution is motion with the acquired transverse [velocity](classical-mechanics.md#velocity), not continued [acceleration](classical-mechanics.md#acceleration) outside the magnet. For the plate-at-exit geometry, set $D=0$. For a nonzero entrance transverse [velocity](classical-mechanics.md#velocity) $w$, add $w(\ell+D)/v$. These terms show why initial [collimation](optical-instrument.md#collimation) and flight geometry matter when inferring a [magnetic moment](electromagnetism.md#magnetic-dipole-moment) from a deposit.

Choose hypothetical parameters $M=1.79\times10^{-25}\,\mathrm{kg}$, $G=300\,\mathrm{T\,m^{-1}}$, $\ell=0.035\,\mathrm m$, $D=0.100\,\mathrm m$, and $v=500\,\mathrm{m\,s^{-1}}$. Approximate the two effective [magnetic moments](electromagnetism.md#magnetic-dipole-moment) by $\mu_z=\pm\mu_B$, where the [Bohr magneton](electromagnetism.md#bohr-magneton) is $\mu_B\simeq9.274\times10^{-24}\,\mathrm{J\,T^{-1}}$. Then $|a_z|\simeq1.55\times10^4\,\mathrm{m\,s^{-2}}$, $t_m=70\,\mu\mathrm s$ and $t_d=200\,\mu\mathrm s$. The positive displacement is about $0.0381\,\mathrm{mm}$ inside the magnet plus $0.2176\,\mathrm{mm}$ during drift: $d=0.2557\,\mathrm{mm}$, with full separation $2d=0.5114\,\mathrm{mm}$. These chosen values illustrate the model and are not reconstructed 1922 measurements.

The exit transverse [velocity](classical-mechanics.md#velocity) is only about $1.09\,\mathrm{m\,s^{-1}}$, small compared with the chosen forward [velocity](classical-mechanics.md#velocity); this checks the small-deflection assumption. Halving $G$ halves $d$, doubling $v$ divides $d$ by four, and setting $D=0$ removes most of this example's separation. A real pole has fringe [magnetic fields](magnetic-field.md) and a position-dependent [gradient](multivariable-calculus.md#gradient); these require a more complete trajectory calculation.

#### Stern-Gerlach discrete and classical profiles

↑ **Parent:** [Stern-Gerlach experiment](#stern-gerlach-experiment)

For an equally populated ideal pair of [angular momentum eigenstates](#angular-momentum-eigenstate), the [magnetic moment](electromagnetism.md#magnetic-dipole-moment) component takes two values, $\pm\mu_B$, and the displacements at fixed [velocity](classical-mechanics.md#velocity) are $\pm d(v)$. Compare a specified classical alternative: every [chemical atom](physics.md#atom-physics) carries a permanent [magnetic moment](electromagnetism.md#magnetic-dipole-moment) of fixed magnitude $\mu_B$, with independently isotropic initial orientations and no dissipative alignment. If $u=\cos\theta$, the sphere's area element is $2\pi\,du$, so $u$ has a [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $[-1,1]$. With precession preserving this component in the ideal geometry, the displacement $d(v)u$ fills the interval $[-d(v),d(v)]$ continuously. A pair of bands therefore tests allowed components rather than merely proving that [silver](chemical-substance.md#silver) is magnetic. Other classical preparation assumptions would be different models and must be stated.

To include finite instrumental width, choose a normalized [Gaussian distribution](probability-distribution.md#normal-distribution)

$$
\phi_\sigma(z)=\frac{1}{\sqrt{2\pi}\sigma}\exp\left(-\frac{z^2}{2\sigma^2}\right)
$$

with [standard deviation](variance.md#standard-deviation) $\sigma=0.035\,\mathrm{mm}$, representing a combined field-off spatial width. At fixed [velocity](classical-mechanics.md#velocity) the model [probability density functions](continuous-probability-distribution.md#probability-density-function) are

$$
p_{\rm two}(z\mid v)=\frac{\phi_\sigma(z-d(v))+\phi_\sigma(z+d(v))}{2},\qquad
p_{\rm classical}(z\mid v)=\frac12\int_{-1}^1\phi_\sigma(z-d(v)u)\,du.
$$

Each has unit [integral](integral.md) and zero [mean](expected-value.md); the different shapes, rather than a different average displacement, distinguish them. The discrete model has [variance](variance.md) $\sigma^2+d(v)^2$, whereas the classical model has [variance](variance.md) $\sigma^2+d(v)^2/3$. Their common mean also explains why the raw average landing position is insufficient to identify the internal [quantum state](quantum-system.md#quantum-state).

Now choose a [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) of forward [velocities](classical-mechanics.md#velocity) from $400$ to $600\,\mathrm{m\,s^{-1}}$, explicitly as an example rather than the oven's actual distribution. Average either conditional [probability density function](continuous-probability-distribution.md#probability-density-function) over that interval. The positive-channel displacement ranges from $0.1776$ to $0.3995\,\mathrm{mm}$, since slower [chemical atoms](physics.md#atom-physics) spend longer accelerating and drifting. The two components broaden into bands even though their internal [magnetic moment](electromagnetism.md#magnetic-dipole-moment) values remain discrete. The corresponding classical profile continues to populate the center. The displayed strip darkness is proportional to predicted deposited number density, with equal total arrivals; it is not a photograph or a calibrated optical response of a developed film.

<a id="image-discrete-magnetic-components-and-continuous-classical-deflections"></a>
![](stern-gerlach-discrete-and-continuous-profiles.png)

**[Figure 2](#image-discrete-magnetic-components-and-continuous-classical-deflections). Discrete magnetic components and continuous classical deflections**. Original model predictions with the chosen flight parameters, comparing one forward speed with a finite speed interval. Both alternatives include the same Gaussian spatial width. Synthetic deposition strips use a common density scale; none of the curves or strips is measured data.

Increasing the spatial width until it is comparable with $d$ can hide the two maxima. At fixed [velocity](classical-mechanics.md#velocity), differentiating the two-state [probability density function](continuous-probability-distribution.md#probability-density-function) twice gives $p_{\rm two}''(0)=\phi_\sigma(d)(d^2-\sigma^2)/\sigma^4$: the central minimum becomes a central maximum when $\sigma>d$. Conversely, a broad distribution of [velocities](classical-mechanics.md#velocity) need not create a new internal component: it spreads each existing component through the $v^{-2}$ dependence. Further instrumental limits include collisions, aperture clipping of strongly deflected trajectories, asymmetric pole geometry, and nonlinear film development. Field-off widths and a mapped [magnetic field](magnetic-field.md) [gradient](multivariable-calculus.md#gradient) are needed to separate such effects. For a modern counting experiment, channel calibration and efficiency corrections belong to [Stern-Gerlach expectation estimation](quantum-system.md#stern-gerlach-expectation-estimation); spatial separation alone does not supply those statistics.

#### Stern-Gerlach historical and modern interpretations

↑ **Parent:** [Stern-Gerlach experiment](#stern-gerlach-experiment)

The 1922 interpretation concerned [space quantization](#space-quantization) of atomic [magnetic moments](electromagnetism.md#magnetic-dipole-moment) in the old [quantum theory](quantum-theory.md). The modern electron [spin](#spin) proposal came in 1925; the original observers did not identify intrinsic electron [spin](#spin) as the cause of their splitting. An orbital interpretation then seemed plausible, but the later [spin](#spin) explanation gives a different account of the same two-component evidence.[Pakvasa, pp. 1–3: original orbital interpretation, 1925 spin proposals and later reinterpretation](physics-bibliography.md#the-stern-gerlach-experiment-and-the-electron-spin-by-sandip-pakvasa)

Modern atomic data assign neutral [silver](chemical-substance.md#silver) the [ground state](quantum-mechanics.md#ground-state) [electron configuration](chemistry.md#electron-configuration) $[\mathrm{Kr}]4d^{10}5s$ and electronic term ${}^2S_{1/2}$. The filled [electron shells](chemistry.md#electron-shell) contribute zero net electronic [angular momentum](momentum.md#angular-momentum); the outer [unpaired electron](chemistry.md#unpaired-electron) has [orbital angular momentum](quantum-mechanics.md#orbital-angular-momentum) $L=0$, [spin](#spin) $S=1/2$, and electronic total [angular momentum](momentum.md#angular-momentum) $J=1/2$. The [magnetic quantum number](quantum-mechanics.md#magnetic-quantum-number) has two values $m_J=\pm1/2$.[Handbook of Basic Atomic Spectroscopic Data by Jean E. Sansonetti and William C. Martin; Ag I ground-state configuration and term; electronic J, distinct from isotope nuclear-spin rows](physics-bibliography.md#handbook-of-basic-atomic-spectroscopic-data-by-jean-e-sansonetti-and-william-c-martin/atomic-data-for-silver-ag)

In the effective electronic description,

$$
\mu_z=-g_J\mu_B\frac{J_z}{\hbar},\qquad
J_z|J,m_J\rangle=\hbar m_J|J,m_J\rangle,\qquad
\mu_z\simeq\mp\mu_B\quad(g_J\simeq2).
$$

The minus sign matters: for positive $G$, the component with $m_J=+1/2$ has negative electronic [magnetic moment](electromagnetism.md#magnetic-dipole-moment) and deflects toward negative $z$ in our coordinates. Calling the upper spot “spin up” without specifying the [magnetic field](magnetic-field.md) and channel calibration can therefore reverse the assignment. The [total angular momentum operator](#total-angular-momentum-operator) here sums electronic [orbital angular momentum](quantum-mechanics.md#orbital-angular-momentum) and electronic [spin](#spin); $J$ is not a claim that the [atomic nucleus](atomic-nucleus.md) has no [spin](#spin). [Hyperfine structure](quantum-mechanics.md#hyperfine-structure) and nuclear [magnetic moments](electromagnetism.md#magnetic-dipole-moment) can require additional internal levels, so a two-channel electronic approximation must be justified for the field and resolution being used.

This is a neutral [atomic beam](physics.md#atomic-beam), not a beam of free [electrons](physics.md#electron). The deflected [mass](classical-mechanics.md#mass) in the flight equations is the entire [silver](chemical-substance.md#silver) [chemical atom](physics.md#atom-physics); its dominant electronic [magnetic moment](electromagnetism.md#magnetic-dipole-moment) supplies the state-dependent [force](force.md). Replacing that atom by a free [electron](physics.md#electron) would also introduce the charged particle's [Lorentz force](relativistic-electromagnetism.md#lorentz-force) and a different preparation problem. The ideal two-state model is useful because it isolates the connection between discrete internal components and spatially resolved outputs; it does not retroactively turn the 1922 deposit into a direct contemporary identification of intrinsic electron [spin](#spin).

<h3 id="holstein-primakoff-transformation">Holstein–Primakoff transformation</h3>

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holstein–Primakoff_transformation)

The Holstein–Primakoff transformation represents a spin-$S$ [operator algebra](functional-analysis.md#operator-algebra) with a bosonic [creation operator](quantum-harmonic-oscillator.md#creation-operator) and [annihilation operator](quantum-harmonic-oscillator.md#annihilation-operator):

$$
S^+=\sqrt{2S}\sqrt{1-\frac{a^\dagger a}{2S}}\,a,\qquad S^-=\sqrt{2S}\,a^\dagger\sqrt{1-\frac{a^\dagger a}{2S}},\qquad S^z=S-a^\dagger a.
$$

The order of the square root and oscillator operator matters. On the physical [Fock states](quantum-field-theory.md#fock-state) $|n\rangle$, $0\le n\le2S$, the raising and lowering matrix elements are $\sqrt{n(2S-n+1)}$ and $\sqrt{(n+1)(2S-n)}$. Their squared difference gives $[S^+,S^-]|n\rangle=2(S-n)|n\rangle$, proving the [spin commutation relations](#spin-commutation-relations). Expanding the square root yields the [linear spin-wave approximation](critical-phenomenon.md#linear-spin-wave-approximation) and its interaction corrections.

#### Holstein-Primakoff matrix-element proof

↑ **Parent:** [Holstein–Primakoff transformation](#holstein-primakoff-transformation)

On $0\le n\le2S$, the raising/lowering amplitudes are $\sqrt{n(2S-n+1)}$ and $\sqrt{(n+1)(2S-n)}$. Their squared difference gives $[S^+,S^-]=2(S-n)$. The order of the number-dependent square root is essential.

<h4 id="holstein-primakoff-occupation-constraint">Holstein–Primakoff occupation constraint</h4>

↑ **Parent:** [Holstein–Primakoff transformation](#holstein-primakoff-transformation)

A spin-$S$ [Hilbert space](hilbert-space.md) has dimension $2S+1$. Its [Holstein–Primakoff transformation](#holstein-primakoff-transformation) therefore uses only bosonic [occupation numbers](quantum-field-theory.md#occupation-number) $0,1,\ldots,2S$. The square root annihilates the upper endpoint. A truncated [linear spin-wave approximation](critical-phenomenon.md#linear-spin-wave-approximation) formally enlarges this space; it is self-consistent only when boson depletion is small compared with $S$.

### Spin commutation relations

↑ **Parent:** [Spin](#spin)

The components of [spin angular momentum](#spin) satisfy $[S_i,S_j]=i\hbar\epsilon_{ijk}S_k$. In units $\hbar=1$, the [spin ladder operators](#spin-ladder-operator) obey $[S^+,S^-]=2S^z$ and $[S^z,S^\pm]=\pm S^\pm$.

### Irreducible spin representation

↑ **Parent:** [Spin](#spin)

The spin-$s$ irreducible representation has dimension $2s+1$, with basis $|s,m\rangle$ for $m=-s,-s+1,\ldots,s$ and Casimir eigenvalue $\hbar^2s(s+1)$.

#### Wigner D-matrix

↑ **Parent:** [Irreducible spin representation](#irreducible-spin-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wigner_D-matrix)

For active rotations with $U=e^{-i\phi J_3}e^{-i\theta J_2}e^{-i\psi J_3}$, the [irreducible spin representation](#irreducible-spin-representation) [matrix](vector-space.md#matrix) is $D^{(j)}_{mm'}=e^{-im\phi}d^{(j)}_{mm'}(\theta)e^{-im'\psi}$, where $d^{(j)}_{mm'}=\langle j,m|e^{-i\theta J_2}|j,m'\rangle$. Its spin-one-half middle [matrix](vector-space.md#matrix) is $\begin{pmatrix}\cos(\theta/2)&-\sin(\theta/2)\\\sin(\theta/2)&\cos(\theta/2)\end{pmatrix}$. A $2\pi$ rotation acts by $(-1)^{2j}$; only integer-spin representations descend to the [special orthogonal group](linear-algebra.md#special-orthogonal-group) in three [dimensions](vector-space.md#dimension-vector-space).

#### Unitary highest-weight termination

↑ **Parent:** [Irreducible spin representation](#irreducible-spin-representation)

For Hermitian $J_3$ and adjoint [angular momentum ladder operators](quantum-mechanics.md#angular-momentum-ladder-operator) $J_+^\dagger=J_-$ on a positive-definite inner-product space, a [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) of weight $j$ obeys $J_+|j,j\rangle=0$. The commutation relations give $J_+(J_-)^\ell|j,j\rangle=\ell(2j-\ell+1)(J_-)^{\ell-1}|j,j\rangle$. Taking [inner products](inner-product.md) forces $2j$ to be a nonnegative integer: otherwise the first negative factor would give a negative squared norm. The norm first vanishes at $\ell=2j+1$, so the generated [unitary representation](representation-theory.md#unitary-representation) has [dimension](vector-space.md#dimension-vector-space) $2j+1$. Without positivity an abstract highest-weight module can remain infinite-dimensional even at an integral [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation).

#### Spin-one half-turn matrix

↑ **Parent:** [Irreducible spin representation](#irreducible-spin-representation)

In the ordered spin-one basis $(m=1,0,-1)$, the second [angular momentum operator](angular-momentum-operator.md) satisfies $J_2^3=J_2$. Therefore its [matrix exponential](linear-operator-theory.md#matrix-exponential) reduces to $I-i\sin\theta J_2+(\cos\theta-1)J_2^2$. A half-turn exchanges the two outer weights and negates the middle weight. Applied to the [pion](standard-model.md#pion) [isospin](standard-model.md#isospin) triplet, this fixes the rotation factor in [G parity](standard-model.md#g-parity).

### Spin ladder operator

↑ **Parent:** [Spin](#spin)

The operators $S_\pm=S_x\pm iS_y$ satisfy

$$
S_\pm|s,m\rangle
=\hbar\sqrt{s(s+1)-m(m\pm1)}|s,m\pm1\rangle.
$$

#### Spin raising operator

↑ **Parent:** [Spin ladder operator](#spin-ladder-operator)

The spin raising operator $S_+=S_x+iS_y$ increases the [magnetic quantum number](quantum-mechanics.md#magnetic-quantum-number) by one and annihilates the maximal-weight state.

#### Spin lowering operator

↑ **Parent:** [Spin ladder operator](#spin-ladder-operator)

The spin lowering operator $S_-=S_x-iS_y$ decreases the [magnetic quantum number](quantum-mechanics.md#magnetic-quantum-number) by one and annihilates the minimal-weight state.

### Spin-three-halves matrices

↑ **Parent:** [Spin](#spin)

In descending $S_z$ order, the spin-$3/2$ raising operator has superdiagonal entries $\hbar\sqrt3,2\hbar,\hbar\sqrt3$; $S_x$ and $S_y$ are its Hermitian real and imaginary combinations.

### Spin coherent state

↑ **Parent:** [Spin](#spin)

A spin coherent state is obtained by rotating the maximal-weight state $|s,s\rangle$ so that it is an eigenstate of spin along a chosen direction with eigenvalue $s\hbar$.

#### Spin-one maximum-projection eigenvector

↑ **Parent:** [Spin coherent state](#spin-coherent-state)

In the ordered z-projection basis $|1,1\rangle,|1,0\rangle,|1,-1\rangle$, the normalized [eigenvector](linear-operator-theory.md#eigenvector) of $J_x\sin\theta+J_z\cos\theta$ with [eigenvalue](linear-operator-theory.md#eigenvalue) $+\hbar$ is the displayed vector. It follows by a y-axis [rotation](riemannian-geometry.md#rotation-mathematics) of the maximum-weight state, or direct solution of the tridiagonal [eigenvalue](linear-operator-theory.md#eigenvalue) equation. Squaring its entries gives the three z-projection measurement [probabilities](probability-theory.md#probability).

#### Spin coherent-state path integral

↑ **Parent:** [Spin coherent state](#spin-coherent-state)

A spin coherent-state path integral inserts group-averaged resolutions of the identity between short time steps. Its kinetic term is the [Spin coherent-state Berry phase](statistical-physics.md#spin-coherent-state-berry-phase), equal to $S$ times the oriented solid angle swept on the sphere.

#### Equatorial spin-three-halves coherent state

↑ **Parent:** [Spin coherent state](#spin-coherent-state)

At azimuth $\varphi$, the normalized spin-$3/2$ coherent-state components are proportional to $1,\sqrt3e^{i\varphi},\sqrt3e^{2i\varphi},e^{3i\varphi}$.

### Larmor precession

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Larmor_precession)

[Larmor precession](#larmor-precession) is the precession of a magnetic moment about an applied magnetic field. For a spin with gyromagnetic ratio $\gamma$ and Hamiltonian $H=-\gamma\mathbf B\cdot\mathbf S$, its expectation obeys $d\langle\mathbf S
angle/dt=\gamma\langle\mathbf S
angle	imes\mathbf B$. A spin coherent state retains its coherent form during this rotation.

#### Larmor frequency

↑ **Parent:** [Larmor precession](#larmor-precession)

The [angular frequency](lagrangian-mechanics.md#angular-frequency) of free [Larmor precession](#larmor-precession) in a uniform [magnetic field](magnetic-field.md) of magnitude $B$, with [gyromagnetic ratio](electromagnetism.md#gyromagnetic-ratio) $\gamma$. Interactions can shift a collective resonance away from this free-spin scale.

#### Larmor precession of a spin coherent state

↑ **Parent:** [Larmor precession](#larmor-precession)

Under $H=-\gamma BS_z$, a coherent spin direction precesses around the $z$-axis with angular velocity $-\gamma B$.

##### Time evolution under a spin-Z Hamiltonian

↑ **Parent:** [Larmor precession of a spin coherent state](#larmor-precession-of-a-spin-coherent-state)

The propagator $e^{i\gamma BtS_z/\hbar}$ multiplies each magnetic component $|s,m\rangle$ by $e^{im\gamma Bt}$.

### Heisenberg model

↑ **Parent:** [Spin](#spin)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heisenberg_model)

The Heisenberg model couples neighboring or more general pairs of spins through $\boldsymbol\sigma_i\mathbin{\cdot}\boldsymbol\sigma_j$. For all-to-all equal coupling, the Hamiltonian can be written in terms of the square of the total spin.

#### Two-spin exchange spectrum with unequal signed magnetic moments

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For $H=(\Delta/4)\boldsymbol\sigma_1\cdot\boldsymbol\sigma_2-(\mu_0B/2)(g_1\sigma_{1z}+g_2\sigma_{2z})$, the parallel-spin energies are $\Delta/4\mp\mu_0B(g_1+g_2)/2$. The zero-projection block has energies $-\Delta/4\pm\sqrt{\Delta^2+[\mu_0B(g_1-g_2)]^2}/2$. Signed moment conventions must be fixed before assigning a physical opposite-charge case.

##### Spin-projection-protected crossings in an exchange spectrum

↑ **Parent:** [Two-spin exchange spectrum with unequal signed magnetic moments](#two-spin-exchange-spectrum-with-unequal-signed-magnetic-moments)

##### Parallel-spin degeneracy for equal-and-opposite moments

↑ **Parent:** [Two-spin exchange spectrum with unequal signed magnetic moments](#two-spin-exchange-spectrum-with-unequal-signed-magnetic-moments)

If $g_2=-g_1$ in a shared magneton convention, the Zeeman [energy](energy.md) of both parallel-spin states cancels. Their [energy](energy.md) stays $\Delta/4$, with exact degeneracy two for every field. Opposite charges alone do not enforce this equality because the masses and magnetic factors may differ.

##### Strong-field limit of a two-spin exchange spectrum

↑ **Parent:** [Two-spin exchange spectrum with unequal signed magnetic moments](#two-spin-exchange-spectrum-with-unequal-signed-magnetic-moments)

If the differential Zeeman [energy](energy.md) $|w|=|\mu_0B(g_1-g_2)|$ greatly exceeds $|\Delta|$, the two mixed levels are $-\Delta/4\pm|w|/2+O(\Delta^2/|w|)$ and approach opposite-spin product states. Four energies are generically distinct. Equal signed moments have $w=0$, so that block remains singlet/triplet rather than being unmixed by a stronger field.

#### XXZ spin chain

↑ **Parent:** [Heisenberg model](#heisenberg-model)

The [XXZ spin chain](#xxz-spin-chain) has equal transverse [exchange interactions](electromagnetism.md#exchange-interaction) and a possibly different longitudinal coupling. For $J>0$ the transverse coupling is antiferromagnetic, while the sign and size of $\Delta$ determine the longitudinal preference. A periodic even chain is bipartite. Its [continuous symmetry](physics.md#continuous-symmetry) is rotation about $z$ for generic $\Delta$, enhanced to full [spin](#spin) rotation at $\Delta=1$.

##### Classical ground states of an XXZ spin chain

↑ **Parent:** [XXZ spin chain](#xxz-spin-chain)

For an even periodic classical chain with [spin](#spin) length $S$ and $J>0$, each bond attains the negative largest [singular value](linear-algebra.md#singular-value) of $\operatorname{diag}(1,1,\Delta)$. For $\Delta>1$ the two minimizing configurations are alternating $z$ [spins](#spin). For $|\Delta|<1$ they are planar [Néel states](statistical-physics.md#neel-state) with arbitrary in-plane angle. For $\Delta<-1$ the two configurations have uniform $z$ [spins](#spin). At $\Delta=1$ the Néel direction is arbitrary on a sphere; at $\Delta=-1$ a staggered transverse component and uniform longitudinal component parameterize another spherical degeneracy. These are classical configuration manifolds, not a claim about finite quantum-chain degeneracy.

#### Classical Heisenberg model

↑ **Parent:** [Heisenberg model](#heisenberg-model)

The [classical Heisenberg model](#classical-heisenberg-model) assigns a three-component unit [vector](vector-space.md#vector) to each site and couples pairs by their [dot product](inner-product.md#dot-product). Positive $J$ favors parallel alignment. With no applied [magnetic field](magnetic-field.md) or anisotropy, simultaneous rotations of all vectors preserve the [energy](energy.md), so an ordered state chooses a direction and exhibits [spontaneous symmetry breaking](quantum-field-theory.md#spontaneous-symmetry-breaking). The [vector order parameter](critical-phenomenon.md#vector-order-parameter) is the spatially averaged orientation. A quartic [Landau free energy](critical-phenomenon.md#landau-free-energy) describes its mean-field onset near a continuous transition; fluctuations can change the critical exponents.[§4.2, $O(3)$ Heisenberg model](physics-bibliography.md#statistical-field-theory-by-david-tong)

##### Classical Heisenberg mean-field partition function

↑ **Parent:** [Classical Heisenberg model](#classical-heisenberg-model)

For unit three-component classical [spins](#spin) and energy $-J\sum_{\langle ij\rangle}\mathbf S_i\cdot\mathbf S_j$ on a lattice of coordination $z_c$, mean-field decoupling gives $E_{\rm MF}=-z_cJS\sum_iS_{iz}+Nz_cJS^2/2$. Integrating each [spin](#spin) over [solid angle](euclidean-geometry.md#solid-angle) yields

$$
Z_{\rm MF}(S)=e^{-\beta Nz_cJS^2/2}
[4\pi\sinh(\beta z_cJS)/(\beta z_cJS)]^N.
$$

The constant term corrects double counting. A normalized angular measure removes $(4\pi)^N$ but does not change the [self-consistency equation](critical-phenomenon.md#self-consistency-equation). The lattice dimension and spin-space dimension are different data.

###### Classical Heisenberg Langevin self-consistency

↑ **Parent:** [Classical Heisenberg mean-field partition function](#classical-heisenberg-mean-field-partition-function)

The single-site average in molecular field $z_cJS$ is $S=\coth x-1/x$, where $x=\beta z_cJS$. Thus $\tau x=\coth x-1/x$ with $\tau=k_BT/(z_cJ)$. The small-$x$ slope $1/3$ gives $k_BT_c^{\rm MF}=z_cJ/3$. On a [square lattice](graph.md#square-lattice) $z_c=4$. This finite mean-field transition does not imply actual positive-temperature [magnetization](electromagnetism.md#magnetization) for the ideal two-dimensional short-range isotropic model, where the [Mermin-Wagner theorem](critical-phenomenon.md#mermin-wagner-theorem) applies.

#### Magnetization sectors of a spin chain

↑ **Parent:** [Heisenberg model](#heisenberg-model)

With $S=\sum_{n=1}^NZ_n$, a computational basis vector containing $k$ excitations has eigenvalue $N-2k$. There are $N+1$ distinct eigenspaces, of dimensions $\binom Nk$. Any Hamiltonian commuting with $S$ preserves each sector and their population weights. In particular, a state supported in one sector cannot be transferred to a different sector by such controls.

#### Excitation-number conservation in XXZ spin chains

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For $H=\sum_{m<n}c_{mn}(X_mX_n+Y_mY_n)+\gamma_{mn}Z_mZ_n$, Pauli [commutators](lie-algebra.md#commutator) give cancellation between the $XX$ and $YY$ terms in $[H,Z_m+Z_n]$, while each $ZZ$ term commutes individually. Hence total spin magnetization is conserved. Local $Z_k$ controls preserve the same law, so dynamics split into fixed-excitation sectors even when a particular sector is controllable.

#### Single-excitation subspace

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For a network of $N$ spin-one-half sites with $Z|0\rangle=|0\rangle$ and $Z|1\rangle=-|1\rangle$, the single-excitation subspace has exactly one spin in state $|1\rangle$ and dimension $N$. Excitation-conserving exchange interactions preserve it. Its restricted Hamiltonian is a hopping matrix whose entries connect the corresponding sites. Controllability within this subspace need not imply controllability on the full $2^N$-dimensional space.

##### XY exchange interaction

↑ **Parent:** [Single-excitation subspace](#single-excitation-subspace)

The isotropic XY exchange interaction between two [qubits](quantum-system.md#qubit) is $E=(X\otimes X+Y\otimes Y)/2$. Its action is

$$
E|00\rangle=E|11\rangle=0,\qquad E|01\rangle=|10\rangle,\qquad E|10\rangle=|01\rangle.
$$

Indeed, $X|0\rangle=|1\rangle$, $X|1\rangle=|0\rangle$, $Y|0\rangle=i|1\rangle$, and $Y|1\rangle=-i|0\rangle$. The two terms cancel on equal bits and add on unequal bits. Thus a network [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) $H=\sum_{a,b}K_{ab}E_{ab}$ preserves excitation number; in the [single-excitation subspace](#single-excitation-subspace), it is the weighted adjacency [matrix](vector-space.md#matrix), moving an excitation from $a$ to $b$ with hopping coefficient $K_{ab}$.

###### Symmetric-arm reduction of an exchange Hamiltonian

↑ **Parent:** [XY exchange interaction](#xy-exchange-interaction)

Consider $q$ identical length-$n$ arms joined to one hub, with [XY exchange interactions](#xy-exchange-interaction) of strength $J_0/\sqrt q$ from the hub to each first site and strength $J_k$ between sites $k,k+1$ on each arm. Let $|s_0\rangle$ be the hub excitation and $|s_k\rangle=q^{-1/2}\sum_{a=1}^q|a,k\rangle$. This [orthonormal](inner-product.md#orthonormal-set) symmetric [single-excitation subspace](#single-excitation-subspace) is invariant, and its restricted [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) is

$$
H|s_0\rangle=J_0|s_1\rangle,\qquad H|s_k\rangle=J_{k-1}|s_{k-1}\rangle+J_k|s_{k+1}\rangle,
$$

with endpoint terms omitted. At the first link the $q$ hub contributions add to $J_0$; all other links act identically on the arms. Thus the [linear isometry](hilbert-space.md#linear-isometry-of-hilbert-spaces) $F|k\rangle=|s_k\rangle$ intertwines $H$ with the path [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) $H_T=\sum_{k=0}^{n-1}J_k(|k\rangle\langle k+1|+|k+1\rangle\langle k|)$: $HF=FH_T$. Expanding the [matrix exponential](linear-operator-theory.md#matrix-exponential) gives $e^{-iHt}F=Fe^{-iH_Tt}$. [Perfect quantum state transfer](quantum-system.md#perfect-quantum-state-transfer) from zero to $n$ on the path therefore produces an equal excitation superposition at the $q$ arm tips. Since all other [qubits](quantum-system.md#qubit) are zero, the tip state is a pure [W state](quantum-system.md#w-state), up to the transfer's common phase.

##### Endpoint control of an XX spin chain

↑ **Parent:** [Single-excitation subspace](#single-excitation-subspace)

In the [single-excitation subspace](#single-excitation-subspace), take a connected real nearest-neighbor hopping matrix $A$ with every coupling nonzero and endpoint control $B=\operatorname{diag}(-1,1,\ldots,1)$. Endpoint commutators isolate the first transition, then propagate along the chain to generate both off-diagonal skew-Hermitian directions and adjacent diagonal differences. These generate $\mathfrak{su}(N)$. For $N\ge3$, $\operatorname{Tr}B=N-2\ne0$ supplies the central direction, giving $\mathfrak u(N)$. For $N=2$ the algebra is $\mathfrak{su}(2)$, which still gives full state controllability but omits an arbitrary global phase. A broken coupling separates an unreachable chain component.

#### Heisenberg antiferromagnet

↑ **Parent:** [Heisenberg model](#heisenberg-model)

A Heisenberg antiferromagnet has positive exchange coupling in $H=J\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j$, so neighboring spins energetically prefer antiparallel alignment.

##### Bipartite spin rotation

↑ **Parent:** [Heisenberg antiferromagnet](#heisenberg-antiferromagnet)

A [bipartite spin rotation](#bipartite-spin-rotation) rotates the [spin](#spin) on one sublattice by $\pi$, converting an alternating classical [Néel state](statistical-physics.md#neel-state) to an all-up reference state. Rotation about $x$ sends $S^z\mapsto-S^z$ and $S^\pm\mapsto S^\mp$ on that sublattice. For an isotropic nearest-neighbor [Heisenberg antiferromagnet](#heisenberg-antiferromagnet), a bond becomes $-S_i^zS_j^z+(S_i^+S_j^++S_i^-S_j^-)/2$. The transformation is unitary and preserves the [spin commutation relations](#spin-commutation-relations); it changes the reference frame, not the model's spectrum.

#### Heisenberg ferromagnet

↑ **Parent:** [Heisenberg model](#heisenberg-model)

A Heisenberg ferromagnet has negative exchange coupling in $H=J\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j$, so neighboring spins energetically prefer parallel alignment.

##### Ferromagnetic ground-state multiplet

↑ **Parent:** [Heisenberg ferromagnet](#heisenberg-ferromagnet)

A connected isotropic spin-$S$ ferromagnet with positive exchanges has a fully polarized [ground state](quantum-mechanics.md#ground-state) and a maximal-total-spin multiplet. For $N$ sites the total spin is $NS$, with $2NS+1$ magnetic states generated by total-spin lowering. Global rotations span the same degenerate space. Slowly varying reorientations produce gapless [ferromagnetic magnons](statistical-physics.md#ferromagnetic-magnon); finite-volume degeneracy must be distinguished from a thermodynamic statement about spontaneous order.

#### Two-spin Heisenberg Hamiltonian in an opposing longitudinal field

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

#### All-to-all Heisenberg model

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For $N$ spin-one-half systems and one term per unordered pair,

$$
\sum_{i<j}\boldsymbol\sigma_i\mathbin{\cdot}\boldsymbol\sigma_j
=2\mathbf S^2-\frac{3N}{2},
\qquad
\mathbf S=\frac12\sum_i\boldsymbol\sigma_i.
$$

Its minimum lies in the smallest available total-spin sector.

#### Infinite-coordination Heisenberg antiferromagnet

↑ **Parent:** [Heisenberg model](#heisenberg-model)

For a bipartite spin-one-half Heisenberg antiferromagnet with coordination $z\to\infty$, the two-sublattice mean-field state becomes exact. Antiparallel pure Bloch vectors give bond energy $-J/4$ for the convention $J\mathbf S_i\cdot\mathbf S_j$.

## Space quantization

↑ **Parent:** [Angular momentum operator](angular-momentum-operator.md)

The restriction of a component of the [angular momentum operator](angular-momentum-operator.md) to discrete [eigenvalues](linear-operator-theory.md#eigenvalue); the [Stern-Gerlach experiment](#stern-gerlach-experiment) tested its magnetic manifestation.

## ↑ Ancestors (4)

1. [Quantum mechanics](quantum-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (28)

- [Angular momentum of a radial function times a linear polynomial](quantum-mechanics.md#angular-momentum-of-a-radial-function-times-a-linear-polynomial)
- [Angular momentum quantum number](quantum-system.md#angular-momentum-quantum-number)
- [Atomic orientation](#atomic-orientation)
- [Barnett equivalent magnetic field](electromagnetism.md#barnett-equivalent-magnetic-field)
- [Nuclear rotational band](atomic-nucleus.md#nuclear-rotational-band)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017.md#1/b/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1.md#a1/a/iii/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1.md#a1/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4.md#6g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#32a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-76.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4.md#6b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#6b/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#6b/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#16b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#16b/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2.md#17b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#34c/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#33b/a/i/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1.md#section-a/2/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1.md#section-b/b6/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1.md#section-b/b7/a/solution)
- [Rigid rotor](molecule.md#rigid-rotor)
- [Space quantization](#space-quantization)
- [Spherical tensor operator](#spherical-tensor-operator)
- [Spin-one half-turn matrix](#spin-one-half-turn-matrix)
- [Spin rotation](#spin-rotation)
- [Weak-field Zeeman splitting](atomic-physics.md#weak-field-zeeman-splitting)
