# Supersymmetric quantum mechanics

↑ **Parent:** [Quantum mechanics](quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersymmetric_quantum_mechanics)

Supersymmetric quantum mechanics factors partner Hamiltonians through first-order operators. Its odd supercharges anticommute to the Hamiltonian; on a Riemannian manifold, the Hilbert space can be realized by square-integrable differential forms with supercharges given by a differential and its adjoint.

**Table of contents**

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

## Supersymmetric factorization and zero-mode normalizability

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)

The candidate zero modes are $e^{-\int^xw}$ in the minus sector and $e^{+\int^xw}$ in the plus sector; this follows from the positive squared-norm expressions for their energy. Their membership in the [Hilbert space](hilbert-space.md) determines whether [supersymmetry](supersymmetry.md) is unbroken. For $w=x$ only the first is normalizable. For $w=x^2+a$, $a>0$, neither is normalizable, while both partner potentials grow quartically and have discrete spectra. Thus their strictly positive lowest energy is paired and [supersymmetry](supersymmetry.md) is broken, with zero [Witten index](#witten-index).

## Witten index

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)

With a well-defined regulated supertrace, positive-energy states of [supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md) are paired by an odd invertible charge. Their opposite [fermion parities](topological-quantum-matter.md#fermion-parity) cancel, leaving $I=n_B^0-n_F^0$, independent of $\beta$. A nonzero index proves the existence of a [supersymmetric vacuum](supersymmetry.md#supersymmetric-vacuum); zero does not prove its absence. Discrete-spectrum or suitable infrared conditions matter, because continuum thresholds and states escaping to infinity can invalidate naive trace manipulations or deformation invariance.

## Gradient superpotential Hamiltonian in supersymmetric quantum mechanics

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)

For a real smooth function $\chi$ on [Euclidean space](normed-vector-space.md#euclidean-norm), put $A_a=\partial_a-\partial_a\chi$ and $q=\sum_a\psi_a^\dagger A_a$. The [adjoint operator](hilbert-space.md#adjoint-operator) for the usual $L^2$ [inner product](inner-product.md) is $A_a^\dagger=-\partial_a-\partial_a\chi$. Since $[A_a,A_b]=0$, the [canonical anticommutation relations](#canonical-anticommutation-relations) give $q^2=0$. Expanding $H=\{q,q^\dagger\}$ and using $[A_a,A_b^\dagger]=-2\partial_a\partial_b\chi$ gives

$$
H=(-\Delta+|\nabla\chi|^2+\Delta\chi)I-2\sum_{a,b}(\partial_a\partial_b\chi)\psi_a^\dagger\psi_b.
$$

In the empty [fermionic Fock space](#fermionic-fock-space) sector the last term vanishes; in the filled sector $\psi_a^\dagger\psi_b=\delta_{ab}$. Consequently the two scalar [Hamiltonian operators](quantum-system.md#hamiltonian-quantum-mechanics) are $H_0=-\Delta+|\nabla\chi|^2+\Delta\chi$ and $H_d=-\Delta+|\nabla\chi|^2-\Delta\chi$. On the compatible [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) domain the [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) is nonnegative because $\langle v,Hv\rangle=\|qv\|^2+\|q^\dagger v\|^2$.

### Zero mode in the fermion-vacuum sector

↑ **Parent:** [Gradient superpotential Hamiltonian in supersymmetric quantum mechanics](#gradient-superpotential-hamiltonian-in-supersymmetric-quantum-mechanics)

For the [gradient superpotential Hamiltonian in supersymmetric quantum mechanics](#gradient-superpotential-hamiltonian-in-supersymmetric-quantum-mechanics), $H_0=\sum_aA_a^\dagger A_a$. A zero-energy [normalizable wavefunction](wave-function.md#normalizable-wavefunction) therefore satisfies $A_af=0$ for every $a$, because its energy is $\sum_a\|A_af\|^2$. Equivalently $\partial_a(e^{-\chi}f)=0$, so on a connected configuration space $f=Ce^\chi$. It exists in the [Hilbert space](hilbert-space.md) precisely when $e^\chi$ is [square-integrable](measure-theory.md#square-integrable-function). In three dimensions with radial $\chi$, this requires $4\pi\int_0^\infty r^2e^{2\chi(r)}\,dr<\infty$. The sign depends on the convention $A=\partial-\partial\chi$; the filled sector instead has the possible zero mode $e^{-\chi}$.

## Fermion-number sectors in supersymmetric quantum mechanics

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)

For $d$ [fermionic creation operators](relativistic-quantum-field.md#fermionic-creation-operator) with the [canonical anticommutation relations](#canonical-anticommutation-relations), the [Hilbert space](hilbert-space.md) $L^2(\mathbb R^d)\otimes\Lambda^\bullet\mathbb C^d$ splits into $\mathcal H_n=L^2(\mathbb R^d)\otimes\Lambda^n\mathbb C^d$, $0\leq n\leq d$. The [fermion number operator](#fermion-number-operator) $N=\sum_a\psi_a^\dagger\psi_a$ has value $n$ on $\mathcal H_n$; its internal multiplicity is $\binom dn$. An odd [supercharge](supersymmetry.md#supersymmetry-generator) $Q=q+q^\dagger$, with $q$ raising $n$ and $q^2=0$, gives $H=\{q,q^\dagger\}$ and preserves these sectors.

On an [eigenspace](linear-operator-theory.md#eigenspace) with $E>0$, $Q/\sqrt E$ is an [odd involution pairing bosonic and fermionic states](supersymmetry.md#odd-involution-pairing-bosonic-and-fermionic-states). More precisely,

$$
v=E^{-1}(qq^\dagger+q^\dagger q)v
$$

gives an [orthogonal decomposition](hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) of each state into the images of $q$ and $q^\dagger$: their [inner product](inner-product.md) vanishes because $(q^\dagger)^2=0$. If $u\in\operatorname{im}q^\dagger$, then $q^\dagger u=0$, $q^\dagger qu=Eu$ and $\|qu\|^2=E\|u\|^2$. Thus $q/\sqrt E$ pairs such a state in degree $n$ with one in degree $n+1$, and $q^\dagger/\sqrt E$ is the inverse. States with zero energy are killed by both operators and may remain unpaired. The pairing applies to positive spectral subspaces as well; discreteness is not implied.

### Radial superpartner in three-dimensional supersymmetric quantum mechanics

↑ **Parent:** [Fermion-number sectors in supersymmetric quantum mechanics](#fermion-number-sectors-in-supersymmetric-quantum-mechanics)

Let $\chi=\chi(r)$, $r=|x|$, and let $f(r)|0\rangle$ be a normalized [eigenstate](energy-eigenvalue.md#eigenstate) of $H_0$ with $E>0$, where $|0\rangle$ is the [Clifford vacuum](#clifford-vacuum). Acting with the [supercharge](supersymmetry.md#supersymmetry-generator) differentiates only its [wavefunction](wave-function.md):

$$
Qf(r)|0\rangle=(f'-\chi'f)\psi_r^\dagger|0\rangle,
\qquad \psi_r^\dagger=\sum_a\frac{x_a}{r}\psi_a^\dagger.
$$

The normalized partner is $E^{-1/2}(f'-\chi'f)\psi_r^\dagger|0\rangle$. Indeed $[H,Q]=0$, and $\|Qf|0\rangle\|^2=E\|f|0\rangle\|^2$; acting with $Q$ again returns $\sqrt E$ times the original state. The expression at $r=0$ is interpreted by the regular extension of the original state. Although its coefficient depends only on $r$, its degree-one components contain the radial unit vector.

## Fermionic Fock space

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)

The fermionic Fock space of $n$ modes is the exterior algebra $\Lambda^\bullet\mathbb C^n$. Creation acts by exterior multiplication and annihilation by contraction.

### Polarized fermionic Fock space

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

An orthogonal projection $P$ splits a one-particle [Hilbert space](hilbert-space.md) into empty and filled modes. Take completed exterior Fock spaces of empty particles and of holes in the filled modes, with the graded tensor product enforcing the [canonical anticommutation relations](#canonical-anticommutation-relations) between both factors. The vacuum is killed by particle annihilation in $PH$ and by particle creation in $(I-P)H$. Only finite particle-hole excitations are needed for a dense basis. Normal ordering subtracts the filled-vacuum expectation from bilinear observables.

#### Fermion-boson correspondence on the circle

↑ **Parent:** [Polarized fermionic Fock space](#polarized-fermionic-fock-space)

In charge $q$, let $\Omega_q$ fill all integer modes below $q$. Its rotation energy is $q(q-1)/2$. The negative [Heisenberg current algebra of a fermion on the circle](#heisenberg-current-algebra-of-a-fermion-on-the-circle) modes create mutually commuting oscillators $b_n^*=J_{-n}/\sqrt n$ with $[b_n,b_m^*]=\delta_{nm}$. Their normalized occupation monomials applied to $\Omega_q$ are orthonormal. The [Jacobi triple product](modular-function.md#jacobi-triple-product) identifies the fermionic charge-energy generating function with $\sum_q u^q t^{q(q-1)/2}\prod_{n>0}(1-t^n)^{-1}$, proving completeness in each finite-dimensional energy space. Thus the rotation Hamiltonian is $Q(Q-1)/2+\sum_{n>0}n b_n^*b_n$.

#### Heisenberg current algebra of a fermion on the circle

↑ **Parent:** [Polarized fermionic Fock space](#polarized-fermionic-fock-space)

For integer modes filled at indices below zero, set $E_{rs}=c_r^\dagger c_s-\delta_{rs}\mathbf1_{r<0}$ and $J_n=\sum_r E_{r,r+n}$ on the finite-energy domain. The [canonical anticommutation relations](#canonical-anticommutation-relations) give a central term $\delta_{st}\delta_{ur}(\mathbf1_{r<0}-\mathbf1_{s<0})$ in $[E_{rs},E_{tu}]$. Summing across the filled-empty boundary gives $[J_n,J_m]=n\delta_{n+m,0}I$, with $J_n^*=J_{-n}$. The current's level is the coefficient of this central term.

##### Fermionic current on the circle

↑ **Parent:** [Heisenberg current algebra of a fermion on the circle](#heisenberg-current-algebra-of-a-fermion-on-the-circle)

A Fourier mode of the normal-ordered fermion density is a fermionic current. On the finite-energy domain its defining sum has finitely many nonzero actions on each occupation vector. The modes satisfy $J_n^*=J_{-n}$ and $[J_n,J_m]=n\delta_{n+m,0}I$. The zero mode is charge; positive modes annihilate charge ground states and negative modes create the oscillators in the [fermion-boson correspondence on the circle](#fermion-boson-correspondence-on-the-circle).

#### Segal quantization criterion for fermions

↑ **Parent:** [Polarized fermionic Fock space](#polarized-fermionic-fock-space)

For the irreducible representation of the [canonical anticommutation relations](#canonical-anticommutation-relations) determined by $P$, a unitary one-particle map $u$ is unitarily implementable precisely when $P-uPu^*$ is [Hilbert-Schmidt](compact-operator.md#hilbert-schmidt-operator), equivalently when $[P,u]$ is Hilbert-Schmidt. The implementer is unique up to a scalar phase. The equivalent representation criterion for two polarizations is that their projections differ by a Hilbert-Schmidt operator. This yields a continuous [projective unitary representation](wave-function.md#projective-unitary-representation) of the [restricted unitary group](topological-group.md#restricted-unitary-group).

### Fermionic operator

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

A [fermionic operator](#fermionic-operator) is odd under [fermion parity](topological-quantum-matter.md#fermion-parity): if $P=(-1)^N$ is the parity operator, then $PAP=-A$. A [fermionic creation operator](relativistic-quantum-field.md#fermionic-creation-operator) or [fermionic annihilation operator](relativistic-quantum-field.md#fermionic-annihilation-operator) is an example. Interchanging odd insertions in a [time-ordered product](perturbative-quantum-field-theory.md#time-ordered-product) contributes the corresponding [fermionic sign](perturbative-quantum-field-theory.md#fermionic-sign). Odd parity alone does not imply that every pair of such operators has zero [anticommutator](vector-space.md#anticommutator).

### Clifford vacuum

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

A Clifford vacuum is a state annihilated by all the chosen fermionic annihilation operators. In a [massless supermultiplet](supersymmetry.md#massless-supermultiplet) it labels the starting [helicity](special-relativity.md#helicity), and applying [fermionic raising and lowering operators](quantum-mechanics.md#fermionic-raising-and-lowering-operator) constructs the remaining states.

### Canonical anticommutation relations

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

Fermionic creation and annihilation operators satisfy $\{a_i,a_j^\dagger\}=\delta_{ij}$ and vanishing equal-type anticommutators. These relations make each mode either empty or singly occupied.

#### Fermionic bilinear charge algebra

↑ **Parent:** [Canonical anticommutation relations](#canonical-anticommutation-relations)

For constant internal matrices acting on [Dirac fields](relativistic-quantum-field.md#dirac-field), the equal-time [canonical anticommutation relations](#canonical-anticommutation-relations) give

$$
[\psi_i^\dagger\psi_j,\psi_k^\dagger\psi_l]=\delta_{jk}\psi_i^\dagger\psi_l-\delta_{il}\psi_k^\dagger\psi_j
$$

with the corresponding spatial delta functions for fields. The quartic terms cancel after fermion reordering. Integrating proves the displayed algebra for well-defined global [Noether charges](classical-field-theory.md#noether-charge), with [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) and a regulator that preserves the nonanomalous internal symmetry. Orthogonal [chiral projectors](relativistic-quantum-field.md#chiral-projector) make the left/right mixed commutators zero. This reduces current-charge closure to a finite matrix calculation.

##### Triplet charged-current closure on electromagnetic charge

↑ **Parent:** [Fermionic bilinear charge algebra](#fermionic-bilinear-charge-algebra)

For normalized triplets $(E^+,n,e)_L$ and $(E^+,N,e)_R$, let the raising matrix have ones in entries $(1,2)$ and $(2,3)$. Its commutator with its adjoint is $\operatorname{diag}(1,0,-1)$. Neutral mixing in $n=c_\alpha\nu+s_\alpha N$ leaves this result unchanged because $c_\alpha^2+s_\alpha^2=1$. With current normalization using $1\mp\gamma^5=2P_{L,R}$, [fermionic bilinear charge algebra](#fermionic-bilinear-charge-algebra) gives the displayed proportionality to the leptonic [electric charge](electric-charge.md) $Q_\ell=e\int:(E^{+\dagger}E^+-e^\dagger e):$. Other current normalizations change the numerical prefactor, not closure. Equal-time algebra does not itself imply conservation of a fermionic weak charge in a symmetry-broken theory.

#### Equal-time canonical anticommutator of a Dirac field

↑ **Parent:** [Canonical anticommutation relations](#canonical-anticommutation-relations)

For mode normalization $1/\sqrt{2E_{\mathbf p}}$, particle and antiparticle operators satisfy $\{a_{\mathbf p}^s,a_{\mathbf q}^{r\dagger}\}=\{b_{\mathbf p}^s,b_{\mathbf q}^{r\dagger}\}=(2\pi)^3\delta^{sr}\delta^3(\mathbf p-\mathbf q)$. The [Dirac spinor](relativistic-quantum-field.md#dirac-spinor) completeness relations imply $\sum_s[u_s(\mathbf p)u_s^\dagger(\mathbf p)+v_s(-\mathbf p)v_s^\dagger(-\mathbf p)]=2E_{\mathbf p}I$. Inserting this into the [mode expansion of a Dirac field](relativistic-quantum-field.md#mode-expansion-of-a-dirac-field) gives the displayed local anticommutator. The reversed momentum in the antiparticle completeness term is essential.

### Fermion number operator

↑ **Parent:** [Fermionic Fock space](#fermionic-fock-space)

The fermion number operator counts occupied fermionic modes. Its parity $(-1)^F$ is positive on even exterior degree and negative on odd exterior degree.

#### Supertrace

↑ **Parent:** [Fermion number operator](#fermion-number-operator)

A supertrace is the trace weighted by fermion parity. Supersymmetry makes paired positive-energy states cancel in a supertrace.

##### Equivariant supertrace

↑ **Parent:** [Supertrace](#supertrace)

An equivariant supertrace inserts a symmetry $f$ as well as fermion parity, $\operatorname{Tr}((-1)^FfA)$. In a path integral, $f$ produces boundary conditions twisted by its action.

## Fermionic path integral

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)

A fermionic path integral integrates Grassmann-valued histories. Its Gaussian integral is a determinant, in contrast with the inverse determinant produced by a bosonic Gaussian integral.

### Berezin integral

↑ **Parent:** [Fermionic path integral](#fermionic-path-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Berezin_integral)

The Berezin integral is differentiation with respect to a Grassmann variable: $\int d\theta\,1=0$ and $\int d\theta\,\theta=1$. A finite-dimensional fermionic Gaussian integral gives a determinant or Pfaffian.

#### Grassmann change-of-variables formula

↑ **Parent:** [Berezin integral](#berezin-integral)

For independent [Grassmann variables](multilinear-algebra.md#grassmann-variable) and an invertible ordinary matrix $S$, the linear change $\eta=S\xi$ transforms the [Berezin integral](#berezin-integral) measure by the inverse [Jacobian determinant](multivariable-calculus.md#jacobian-determinant). Indeed, the highest-degree monomial transforms by $\det S$, and coefficient extraction must undo that factor. For paired variables $\eta=S\xi$ and $\bar\eta=\bar\xi S^{-1}$ the two factors cancel. The order of odd variables and differentials fixes the overall sign and must be kept consistent.

### Short-time limit of a supersymmetric path integral

↑ **Parent:** [Fermionic path integral](#fermionic-path-integral)

The short-time limit rescales a Euclidean time circle toward zero size. Supersymmetry cancels paired nonzero-mode determinants, leaving an integral over constant or symmetry-fixed zero modes.

## Twisted de Rham differential

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)

For a real function $h$, the twisted de Rham differential is $d_h=d+dh\wedge=e^{-h}de^h$. Its adjoint and $d_h$ define a supersymmetric Hamiltonian, and its square-integrable cohomology describes zero-energy states.

## Partner Hamiltonians

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partner_Hamiltonians)

Partner Hamiltonians reverse the order of two first-order factors and share corresponding positive-energy states.

<h2 id="poschl-teller-potential">Pöschl-Teller potential</h2>

↑ **Parent:** [Supersymmetric quantum mechanics](supersymmetric-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pöschl–Teller_potential)

A Pöschl-Teller potential is a solvable one-dimensional potential built from $\operatorname{sech}^2 x$. The attractive member

$$
V(x)=-n(n+1)\alpha^2\operatorname{sech}^2(\alpha x)
$$

is reflectionless when $n$ is a positive integer.

### Supersymmetric factorization of the one-soliton potential

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

## ↑ Ancestors (4)

1. [Quantum mechanics](quantum-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-53.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#1/solution)
- [Witten index](#witten-index)
