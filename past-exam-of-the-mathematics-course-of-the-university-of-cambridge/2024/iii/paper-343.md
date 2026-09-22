# Paper 343

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_343.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_343.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\Phi:M_d(\mathbb C)\to M_D(\mathbb C)$ be a [linear map](../../../vector-space.md#linear-map). It is [positive](../../../quantum-information-theory.md#positive-linear-map) when $X\geq0$ implies $\Phi(X)\geq0$, and [completely positive](../../../quantum-information-theory.md#completely-positive-map) when

$$
\Phi\otimes\operatorname{id}_r
$$

is positive for every ancillary dimension $r$. In finite dimensions it is enough to check $r=d$.

A finite family of [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $A^\alpha:\mathbb C^d\to\mathbb C^D$ defines the [Kraus representation](../../../quantum-information-theory.md#kraus-representation)

$$
\Phi(X)=\sum_{\alpha=1}^R A^\alpha X(A^\alpha)^\dagger.
$$

This map is completely positive because, for every [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) $Y$ on the enlarged space,

$$
(\Phi\otimes\operatorname{id}_r)(Y)
=\sum_\alpha(A^\alpha\otimes I_r)Y((A^\alpha)^\dagger\otimes I_r)\geq0.
$$

Conversely, use the unnormalized [maximally entangled vector](../../../quantum-theory.md#maximally-entangled-state) $|\Omega\rangle=\sum_{j=1}^d|j\rangle|j\rangle$. Complete positivity makes the [Choi matrix](../../../quantum-information-theory.md#choi-matrix)

$$
C_\Phi=(\Phi\otimes\operatorname{id}_d)(|\Omega\rangle\langle\Omega|)
$$

positive semidefinite. By the [spectral theorem for normal operators](../../../hilbert-space.md#spectral-theorem-for-normal-operators), $C_\Phi=\sum_{\alpha=1}^R|v_\alpha\rangle\langle v_\alpha|$, where $R=\operatorname{rank}C_\Phi\leq dD$. Reshape each $v_\alpha\in\mathbb C^D\otimes\mathbb C^d$ into a matrix $A^\alpha$ by $|v_\alpha\rangle=\sum_{\mu j}A^\alpha_{\mu j}|\mu\rangle|j\rangle$. The [Choi matrix](../../../quantum-information-theory.md#choi-matrix) inversion formula

$$
\Phi(X)=\operatorname{Tr}_{\rm in}\!\left[C_\Phi(I_D\otimes X^T)\right]
$$

then gives $\Phi(X)=\sum_\alpha A^\alpha X(A^\alpha)^\dagger$. Thus finite [Kraus representations](../../../quantum-information-theory.md#kraus-representation) characterize finite-dimensional completely positive maps.

The additional normalization

$$
\sum_\alpha(A^\alpha)^\dagger A^\alpha=I_d
$$

makes $\Phi$ trace preserving and hence a [quantum channel](../../../quantum-information-theory.md#quantum-channel); $\sum_\alpha A^\alpha(A^\alpha)^\dagger=I_D$ instead makes it unital.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

An open-boundary [matrix product state](../../../quantum-theory.md#matrix-product-state) with physical dimension $q$ and bond dimension $\chi$ is

$$
|\Psi_N\rangle
=\sum_{i_1,\ldots,i_N=1}^q
\langle \ell|A^{i_1}A^{i_2}\cdots A^{i_N}|r\rangle
|i_1i_2\cdots i_N\rangle,
$$

where the $A^i$ are $\chi\times\chi$ matrices and $|\ell\rangle,|r\rangle$ are boundary vectors. For periodic boundary conditions, replace the boundary contraction by the [matrix trace](../../../linear-algebra.md#matrix-trace) $\operatorname{Tr}(A^{i_1}\cdots A^{i_N})$.

The same matrices define the [matrix product state transfer map](../../../quantum-theory.md#matrix-product-state-transfer-map)

$$
\mathcal E(X)=\sum_iA^iX(A^i)^\dagger.
$$

When $\sum_i(A^i)^\dagger A^i=I$, the [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation)

$$
V|\psi\rangle=\sum_i|i\rangle\otimes A^i|\psi\rangle
$$

is an [isometry](../../../riemannian-geometry.md#isometry). Repeatedly applying $V$ stores each Kraus label in a fresh physical register:

$$
V_N\cdots V_1|r\rangle
=\sum_{i_1,\ldots,i_N}|i_1\cdots i_N\rangle
\otimes A^{i_N}\cdots A^{i_1}|r\rangle.
$$

Contracting the remaining virtual system with $\langle\ell|$ gives an MPS, while tracing over all recorded labels gives repeated application of the [completely positive map](../../../quantum-information-theory.md#completely-positive-map) $\mathcal E$. The MPS is therefore a coherent [unravelling](../../../quantum-theory.md#matrix-product-state-as-an-unravelling-of-a-completely-positive-map) of the channel. Equivalently, retaining the Kraus-label registers realizes a [purification](../../../quantum-theory.md#purification-of-a-density-operator) of its output. A non-normalized MPS tensor gives the same construction with a general completely positive map; an appropriate canonical gauge normalizes the transfer map on its support.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Normalize the stated [Pauli matrices](../../../algebra.md#pauli-matrices) as

$$
A^x=\frac{\sigma_x}{\sqrt3},
\qquad
A^y=\frac{\sigma_y}{\sqrt3},
\qquad
A^z=\frac{\sigma_z}{\sqrt3}.
$$

The factor $3^{-1/2}$ changes only the overall normalization at fixed $N$. In the [spin-one Cartesian basis](../../../quantum-mechanics.md#spin-one-cartesian-basis), the associated periodic [uniform matrix product state](../../../quantum-theory.md#uniform-matrix-product-state) is

$$
|\Psi_N\rangle
=\sum_{i_1,\ldots,i_N\in\{x,y,z\}}
\operatorname{Tr}(A^{i_1}\cdots A^{i_N})
|i_1\cdots i_N\rangle.
$$

This is the [Pauli-matrix representation of the Affleck--Kennedy--Lieb--Tasaki state](../../../quantum-theory.md#pauli-matrix-representation-of-the-affleck-kennedy-lieb-tasaki-state).

The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law)

$$
\sigma_i\sigma_j=\delta_{ij}I+i\varepsilon_{ijk}\sigma_k
$$

shows that products on two neighboring sites span all of $M_2(\mathbb C)$, so the tensor is an [injective matrix product state](../../../quantum-theory.md#injective-matrix-product-state) after [blocking](../../../quantum-theory.md#blocking-a-matrix-product-state) two sites. More geometrically, its two-site image is the scalar plus antisymmetric subspace of $3\otimes3$, namely the total-spin $J=0$ and $J=1$ sectors. By the [Two-site support of the Pauli-matrix Affleck--Kennedy--Lieb--Tasaki tensor](../../../quantum-theory.md#two-site-support-of-the-pauli-matrix-affleck-kennedy-lieb-tasaki-tensor), the missing subspace is the five-dimensional symmetric traceless $J=2$ sector.

Let $P^{(2)}_{n,n+1}$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto that $J=2$ sector. The [parent Hamiltonian of a matrix product state](../../../quantum-theory.md#parent-hamiltonian-of-a-matrix-product-state) is

$$
H=\sum_nP^{(2)}_{n,n+1}.
$$

Each term annihilates $|\Psi_N\rangle$, so this is a [frustration-free quantum Hamiltonian](../../../quantum-theory.md#frustration-free-quantum-hamiltonian) and the MPS is a ground state. Writing $x=\mathbf S_n\mathbin\cdot\mathbf S_{n+1}$ and using the [eigenvalues](../../../quantum-mechanics.md#spin-dot-product-eigenvalue) $-2,-1,1$ in the three [total-spin sectors](../../../quantum-mechanics.md#total-spin-sector) gives the explicit projector

$$
P^{(2)}_{n,n+1}
=\frac{(x+2)(x+1)}6.
$$

This is the [Affleck--Kennedy--Lieb--Tasaki parent Hamiltonian](../../../quantum-theory.md#affleck-kennedy-lieb-tasaki-parent-hamiltonian). Injectivity implies that its periodic ground state is unique for every sufficiently long chain.

## 2

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write the spin-one-half [Heisenberg antiferromagnet](../../../quantum-mechanics.md#heisenberg-antiferromagnet) as

$$
H_z=J\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j,
\qquad J>0,
$$

on a bipartite lattice of [coordination number](../../../statistical-physics.md#coordination-number-of-a-lattice) $z$. A one-spin [density operator](../../../quantum-theory.md#density-matrix) is $\rho=(I+\mathbf r\mathbin\cdot\boldsymbol\sigma)/2$, where $\mathbf r$ is its [Bloch vector](../../../quantum-theory.md#bloch-vector) and $|\mathbf r|\leq1$. In a two-sublattice [product state](../../../bell-state.md#product-state),

$$
\langle\mathbf S_i\mathbin\cdot\mathbf S_j\rangle
=\frac14\mathbf r_A\mathbin\cdot\mathbf r_B.
$$

The minimum is $-1/4$, attained by pure antiparallel Bloch vectors, so the minimizing product state is a [Néel state](../../../statistical-physics.md#neel-state). In the $z\to\infty$ limit this [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation) becomes exact and the ground-state energy per bond is therefore

$$
e_{\rm bond}=-\frac J4.
$$

The phrase “energy density” requires a coupling convention. For the unscaled Hamiltonian above, every site belongs to $z/2$ bonds and

$$
\frac{E_0}{N}=-\frac{Jz}{8},
$$

which diverges as $z\to\infty$. With the standard [Kac normalization](../../../statistical-physics.md#coordination-number-of-a-lattice)

$$
H_z^{\rm Kac}=\frac Jz\sum_{\langle ij\rangle}\mathbf S_i\mathbin\cdot\mathbf S_j,
$$

the finite energy density is

$$
\lim_{z\to\infty}\frac{E_0}{N}=-\frac J8.
$$

If the convention divides by the spatial dimension $d=z/2$ instead, the answer is $-J/4$ per site. A Hamiltonian written with $\boldsymbol\sigma_i\mathbin\cdot\boldsymbol\sigma_j$ rather than $\mathbf S_i\mathbin\cdot\mathbf S_j$ multiplies all these energies by four.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Quantum de Finetti theorem](../../../quantum-information-theory.md#quantum-de-finetti-theorem) says that the fixed-$k$ [reduced density matrix](../../../bell-state.md#reduced-density-matrix) of an exchangeable $N$-particle state approaches

$$
\rho^{(k)}=\int \sigma^{\otimes k}\,d\mu(\sigma)
$$

as $N\to\infty$. Finite versions bound the [trace norm](../../../functional-analysis.md#trace-norm) error by a constant of order $d_{\rm loc}^2k/N$. On a bipartite lattice, the corresponding two-sublattice form is a mixture

$$
\rho_{AB}=\int \rho_A\otimes\rho_B\,d\mu(\rho_A,\rho_B)+o(1).
$$

This is the [mean-field ansatz from the quantum de Finetti theorem](../../../quantum-information-theory.md#mean-field-ansatz-from-the-quantum-de-finetti-theorem).

The bond energy is a [linear functional](../../../linear-algebra.md#linear-functional) of $\rho_{AB}$. A [convex combination](../../../mathematical-optimization.md#convex-combination) cannot have energy below its lowest product component, so it remains only to minimize

$$
\operatorname{Tr}\!\left[
(\rho_A\otimes\rho_B)\,
J\mathbf S_A\mathbin\cdot\mathbf S_B
\right]
=\frac J4\mathbf r_A\mathbin\cdot\mathbf r_B.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $\mathbf r_A\mathbin\cdot\mathbf r_B\geq-|\mathbf r_A||\mathbf r_B|\geq-1$, with equality for pure antiparallel vectors. This reproduces the [Néel state](../../../statistical-physics.md#neel-state) and $-J/4$ per bond found in part (a).

**Yes.** The limiting state saturates the de Finetti mean-field lower bound: the minimizing product state belongs to the allowed de Finetti mixture, and the finite-de-Finetti error tends to zero as $z\to\infty$. At finite $z$ the theorem gives only an approximation; entanglement and correlated fluctuations can lower the energy below the product-state value by corrections that vanish in the infinite-coordination limit.

## 3

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let

$$
H_\pm=\pm J\sum_jh_{j,j+1},
\qquad
h_{j,j+1}=\mathbf S_j\mathbin\cdot\mathbf S_{j+1},
$$

where the two signs describe the [Heisenberg antiferromagnet](../../../quantum-mechanics.md#heisenberg-antiferromagnet) and [Heisenberg ferromagnet](../../../quantum-mechanics.md#heisenberg-ferromagnet). A standard [Lieb-Robinson bound](../../../quantum-theory.md#lieb-robinson-bound) is obtained by iterating the [Heisenberg picture](../../../quantum-mechanics.md#heisenberg-picture) equation and bounding nested [commutators](../../../lie-algebra.md#commutator) by [operator norms](../../../continuous-dual-space.md#operator-norm). Its constants depend on the interaction only through quantities such as

$$
\sup_x\sum_{X\ni x}|X|\,\|\Phi(X)\|e^{\mu\operatorname{diam}X}.
$$

Changing $J$ to $-J$ changes neither the supports nor the norms $\|\Phi(X)\|$. Every term in the nested-commutator estimate acquires at most an irrelevant sign before its absolute value is taken. Therefore both chains obey exactly the same estimate

$$
\|[A(t),B]\|
\leq C\|A\|\|B\|e^{-\mu(d(A,B)-v_{\rm LR}|t|)}
$$

with the same $C,\mu$, and Lieb-Robinson velocity $v_{\rm LR}$. No unitary equivalence of the two Hamiltonians is required.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Consider a depth-$D$ circuit whose gates have range at most $r$. Under backward Heisenberg evolution, a one-site observable has a [backward light cone of a local quantum circuit](../../../quantum-theory.md#backward-light-cone-of-a-local-quantum-circuit) of radius at most $rD$. Choose sites $i,j$ separated by $L>2rD$. Their two backward light cones are disjoint. Since the input is a [product state](../../../bell-state.md#product-state), expectations factorize, and hence every [connected correlation function](../../../critical-phenomenon.md#connected-correlation-function) between the two output observables vanishes.

For the [GHZ state](../../../quantum-theory.md#greenberger-horne-zeilinger-state)

$$
|\operatorname{GHZ}_N\rangle
=\frac{|0\rangle^{\otimes N}+|1\rangle^{\otimes N}}{\sqrt2},
$$

however,

$$
\langle Z_i\rangle=\langle Z_j\rangle=0,
\qquad
\langle Z_iZ_j\rangle=1,
\qquad
\langle Z_iZ_j\rangle_c=1
$$

at every separation. The light cones must therefore overlap, which forces

$$
D\geq\frac{L}{2r}.
$$

For opposite ends of a one-dimensional chain, $L=\Theta(N)$, so $D=\Omega(N)$ and no constant-depth local circuit can prepare the GHZ state. The continuous-time version follows directly from the [Lieb-Robinson bound](../../../quantum-theory.md#lieb-robinson-bound), with preparation time at least $L/(2v_{\rm LR})$ up to exponentially small tails.

This is the [GHZ-state circuit-depth lower bound](../../../quantum-theory.md#ghz-state-circuit-depth-lower-bound). [Finite-depth local circuits](../../../quantum-theory.md#finite-depth-local-quantum-circuit) define equivalence within a gapped phase, so a state with this [long-range order](../../../statistical-physics.md#long-range-order) cannot lie in the same circuit phase as a product state. The GHZ state is the finite-size cat state associated with spontaneous symmetry breaking; it is not a unique short-range-entangled ground state. The persistent distant correlation is precisely the obstruction.

## 4

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the injective translationally invariant case, the [fundamental theorem of matrix product states](../../../quantum-theory.md#fundamental-theorem-of-matrix-product-states) states that two tensors $A=\{A^i\}$ and $B=\{B^i\}$ of the same minimal bond dimension generate the same periodic MPS for every sufficiently large length if and only if

$$
A^i=e^{i\theta}XB^iX^{-1}
$$

for every physical index $i$, with one invertible matrix $X$. Equality as normalized rays permits the phase $e^{i\theta}$; equality as vectors for all lengths restricts the resulting factor $e^{iN\theta}$ accordingly. The converse is immediate from cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace):

$$
\operatorname{Tr}(A^{i_1}\cdots A^{i_N})
=e^{iN\theta}\operatorname{Tr}(B^{i_1}\cdots B^{i_N}).
$$

For the nontrivial direction, [block](../../../quantum-theory.md#blocking-a-matrix-product-state) enough sites that both tensors are injective and define

$$
\Gamma_A^L(X)
=\sum_{i_1,\ldots,i_L}
\operatorname{Tr}(XA^{i_1}\cdots A^{i_L})
|i_1\cdots i_L\rangle,
$$

with $\Gamma_B^L$ defined similarly. Injectivity means that $\Gamma_A^L$ and $\Gamma_B^L$ have trivial [kernels](../../../linear-algebra.md#kernel-of-a-linear-map). Equality of all sufficiently long periodic states implies equality of the local support spaces $\operatorname{im}\Gamma_A^L=\operatorname{im}\Gamma_B^L$, so there is an invertible linear map $F$ on the virtual matrix algebra satisfying

$$
\Gamma_A^L=\Gamma_B^L\circ F.
$$

Compare two adjacent blocks and contract arbitrary environments on their left and right. Because both block maps are injective, equality of the physical contractions forces

$$
F(XY)=F(X)F(Y),
\qquad
F(I)=I.
$$

Thus $F$ is a unital algebra automorphism of $M_\chi(\mathbb C)$. By [every automorphism of a full matrix algebra is inner](../../../linear-algebra.md#every-automorphism-of-a-full-matrix-algebra-is-inner), $F(X)=X_0XX_0^{-1}$ for an invertible $X_0$. Applying this relation to a block with one physical site exposed gives

$$
A^i=e^{i\theta}X_0B^iX_0^{-1}.
$$

This proves the theorem and identifies the freedom as the [gauge equivalence of injective matrix product state tensors](../../../quantum-theory.md#gauge-equivalence-of-injective-matrix-product-state-tensors). For noninjective tensors, their canonical forms first split into injective blocks; equality then permits a permutation of equivalent blocks together with a similarity transformation and phase on each block.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Affleck--Kennedy--Lieb--Tasaki state](../../../quantum-theory.md#affleck-kennedy-lieb-tasaki-state) places two virtual spin-one-half degrees of freedom at every site, puts neighboring virtual spins into [singlets](../../../quantum-mechanics.md#spin-one-half-singlet-state), and projects the two virtual spins at each site onto their symmetric spin-one triplet. Its local tensor is equivalently proportional to $\sigma_x,\sigma_y,\sigma_z$ in the [spin-one Cartesian basis](../../../quantum-mechanics.md#spin-one-cartesian-basis), and its [Affleck--Kennedy--Lieb--Tasaki parent Hamiltonian](../../../quantum-theory.md#affleck-kennedy-lieb-tasaki-parent-hamiltonian) is

$$
H_{\rm AKLT}=\sum_jP^{(2)}_{j,j+1}.
$$

The one-dimensional [cluster state](../../../topological-quantum-matter.md#cluster-state) is the simultaneous $+1$ eigenstate of the commuting stabilizers

$$
K_j=Z_{j-1}X_jZ_{j+1}.
$$

On a periodic chain it is obtained by applying a controlled-$Z$ gate on every neighboring pair of the product state $|+\rangle^{\otimes N}$.

After suitable blocking, the two states have the same nontrivial [projective virtual symmetry of a matrix product state](../../../topological-quantum-matter.md#projective-virtual-symmetry-of-a-matrix-product-state) for the protecting group $\mathbb Z_2\times\mathbb Z_2$. The two virtual symmetry generators can be represented by anticommuting Pauli matrices, so they realize the nontrivial projective class in [group cohomology](../../../group-theory.md#group-cohomology). Consequently the AKLT and cluster states can be connected by a symmetry-preserving gapped path, or equivalently by a symmetry-preserving finite-depth local circuit: this is the [Symmetry-protected equivalence of the Affleck--Kennedy--Lieb--Tasaki state and cluster state](../../../quantum-theory.md#symmetry-protected-equivalence-of-the-affleck-kennedy-lieb-tasaki-state-and-cluster-state).

Both states therefore exhibit one-dimensional [symmetry-protected topological order](../../../topological-quantum-matter.md#symmetry-protected-topological-phase). On an open chain their nontrivial virtual representation produces [protected edge degrees of freedom](../../../topological-quantum-matter.md#protected-edge-state-of-a-symmetry-protected-topological-phase) and a characteristic degeneracy in the [entanglement spectrum of a matrix product state](../../../quantum-theory.md#entanglement-spectrum-of-a-matrix-product-state). They do not have [intrinsic topological order](../../../topological-quantum-matter.md#intrinsic-topological-order): if the protecting symmetry is discarded, either state can be connected to a product state by a finite-depth local circuit.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
