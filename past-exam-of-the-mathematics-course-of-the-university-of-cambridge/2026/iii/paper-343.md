# Paper 343

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20343.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20343.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [quantum channel](../../../quantum-information-theory.md#quantum-channel) is a linear completely positive trace-preserving map. Its [Kraus representation](../../../quantum-information-theory.md#kraus-representation) is

$$
\mathcal E(\rho)=\sum_\alpha K_\alpha\rho K_\alpha^\dagger,
\qquad
\boxed{\sum_\alpha K_\alpha^\dagger K_\alpha=I}.
$$

Kraus operators are not unique: two representations of the same channel are related by an isometry on the Kraus index, and by a unitary when both lists are minimal and equally long. A differentiable Markovian family of infinitesimal channels gives the [Lindblad equation](../../../quantum-information-theory.md#lindblad-equation)

$$
\boxed{\dot\rho=-i[H,\rho]
+\sum_\alpha\left(
L_\alpha\rho L_\alpha^\dagger
-\frac12\{L_\alpha^\dagger L_\alpha,\rho\}
\right).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Strict trace-distance contraction means that for some $\eta<1$,

$$
\|\mathcal E(\rho)-\mathcal E(\sigma)\|_1
\leq\eta\|\rho-\sigma\|_1
$$

for all states. Equivalently, the induced trace norm on nonzero traceless Hermitian operators is strictly below one. This immediately gives a unique fixed state by the contraction mapping theorem.

The standard algebraic condition is that the channel be a [primitive quantum channel](../../../quantum-information-theory.md#primitive-quantum-channel): some finite products

$$
K_{\alpha_m}\cdots K_{\alpha_1}
$$

span the full matrix algebra, equivalently some power of the channel maps every nonzero positive operator to a positive-definite one. Spectrally, eigenvalue $1$ is then simple and every other eigenvalue has modulus less than one. This condition is necessary and sufficient for convergence to a unique full-rank fixed point. Irreducibility alone gives uniqueness but may leave periodic peripheral eigenvalues.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $\rho_*=|\psi^-\rangle\langle\psi^-|$ and choose

$$
\boxed{
\mathcal E(\rho)=\frac12\rho+\frac12\rho_*\operatorname{Tr}\rho}.
$$

For any orthonormal two-qubit basis $\{|\mu\rangle\}_{\mu=1}^4$, a Kraus representation is

$$
K_0=\frac1{\sqrt2}I,
\qquad
K_\mu=\frac1{\sqrt2}|\psi^-\rangle\langle\mu|.
$$

The completeness relation holds and $\mathcal E(\rho_*)=\rho_*$. Differences of states are traceless, so

$$
\mathcal E(\rho)-\mathcal E(\sigma)
=\frac12(\rho-\sigma).
$$

The channel is strictly contractive with coefficient $1/2$. On operator space, $\rho_*$ spans the eigenvalue-one direction and every traceless operator has eigenvalue $1/2$, hence

$$
\boxed{|\lambda_2|=\frac12}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation) isometry is

$$
V=\sum_\alpha K_\alpha\otimes|\alpha\rangle_E.
$$

Applying it successively to fresh environment systems gives

$$
|\Psi_N\rangle
=\sum_{\alpha_1,\ldots,\alpha_N}
K_{\alpha_N}\cdots K_{\alpha_1}|\phi\rangle
\otimes|\alpha_1\cdots\alpha_N\rangle.
$$

Contracting the final system with a boundary vector turns every amplitude into a boundary contraction of the matrices $K_\alpha$. This is a [matrix product state](../../../quantum-theory.md#matrix-product-state) with bond dimension at most the system dimension.

For an injective MPS, the fundamental gauge freedom is

$$
K_\alpha\mapsto XK_\alpha X^{-1},
$$

together with the inverse transformation of boundary vectors; an overall phase is also immaterial. Its channel converges to a unique fixed state exactly when eigenvalue one is simple and there are no other peripheral eigenvalues, equivalently when it is a [primitive quantum channel](../../../quantum-information-theory.md#primitive-quantum-channel). A unique fixed state without convergence only requires the eigenvalue-one eigenspace itself to be one-dimensional.

## 2

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Entanglement monogamy](../../../quantum-information-theory.md#entanglement-monogamy) says that strong entanglement between $A$ and $B$ limits the entanglement of either with an independent $C$. For qubits, the Coffman--Kundu--Wootters inequality is

$$
C_{A:BC}^2\geq C_{AB}^2+C_{AC}^2.
$$

In quantum cryptography, nearly maximal correlations between legitimate partners imply that an eavesdropper cannot hold a purification with equally strong correlations. Measuring an error rate therefore bounds the eavesdropper's information and permits privacy amplification.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Interpret the sum as one term per unordered pair. With

$$
S_\alpha=\frac12\sum_{i=1}^N\sigma_i^\alpha,
$$

the all-to-all XY Hamiltonian is

$$
H=2(S_x^2+S_y^2)-N
=2[S(S+1)-m^2]-N.
$$

For fixed total spin $S$, choose $|m|=S$, giving $E=2S-N$. The smallest allowed total spin is $S=0$ for even $N$ and $S=1/2$ for odd $N$, so

$$
E_0=
\begin{cases}
-N,&N\ \text{even},\\
1-N,&N\ \text{odd}.
\end{cases}
$$

Dividing by $\binom N2$ gives

$$
\boxed{\lim_{N\to\infty}\frac{E_0}{\binom N2}=0^-}.
$$

For three qubits, $E_0=-2$ and there are three pairs:

$$
\boxed{\frac{E_0}{3}=-\frac23<0}.
$$

The finite system therefore has a smaller pair-energy density; monogamy prevents every pair from independently attaining the two-qubit minimum.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

In a local gapped ground state, correlations and the entanglement needed to lower a local interaction energy are concentrated over a finite distance. Degrees of freedom deep inside a region use most of their entanglement with nearby degrees of freedom that are also inside; [entanglement monogamy](../../../quantum-information-theory.md#entanglement-monogamy) limits their simultaneous entanglement with the exterior. Only degrees of freedom within a correlation length of the boundary can contribute extensively across the cut, giving an [entanglement area law](../../../quantum-information-theory.md#entanglement-area-law)

$$
S(A)=O(|\partial A|).
$$

Monogamy supplies the physical mechanism, while locality and suitable ground-state assumptions are essential; monogamy alone is not a general mathematical proof of an area law.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Cutting an open-boundary [matrix product state](../../../quantum-theory.md#matrix-product-state) crosses one virtual bond of dimension $\chi$. Its Schmidt rank is at most $\chi$, so

$$
\boxed{S(A)\leq\log\chi}.
$$

A periodic interval crosses two bonds and obeys $S(A)\leq2\log\chi$. The one-dimensional boundary has a constant number of points, so this is an area law.

For a [projected entangled pair state](../../../quantum-theory.md#projected-entangled-pair-state), cut every virtual bond crossing the boundary of a region $A$. If $n_\partial$ bonds are cut, the Schmidt rank is at most $\chi^{n_\partial}$, and therefore

$$
\boxed{S(A)\leq n_\partial\log\chi}.
$$

Since $n_\partial$ is proportional to the lattice boundary area, every fixed-bond-dimension PEPS satisfies an area law.

## 3

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

There are only two one-site matrices, so they cannot span the four-dimensional virtual matrix algebra. For two sites,

$$
A^iA^j
=\langle s_i|j\rangle\,|i\rangle\langle s_j|,
\qquad
s_0=+,\quad s_1=-.
$$

Every overlap $\langle s_i|j\rangle$ is nonzero, and the four outer products $|i\rangle\langle s_j|$ are linearly independent. Hence

$$
\boxed{\text{the injectivity length is }2}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Physical $\sigma_x$ swaps $A^0$ and $A^1$. Direct multiplication of the four blocked matrices shows

$$
A^{1-i_1}A^{i_2}
=\sigma_x(A^{i_1}A^{i_2})\sigma_x,
$$



$$
A^{i_1}A^{1-i_2}
=\sigma_z(A^{i_1}A^{i_2})\sigma_z.
$$

Thus one may choose

$$
\boxed{V_a=\sigma_x,\qquad V_b=\sigma_z}.
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Apply $\sigma_x$ to every odd site and use the first pulling-through identity on every two-site block. Adjacent $V_a^{-1}V_a$ factors cancel, while periodicity and cyclicity of the trace cancel the final pair. The MPS is unchanged. The identical argument with $V_b$ applies to every even site. Therefore the state has the two commuting physical symmetries

$$
\boxed{\prod_{j\ {\rm odd}}X_j},
\qquad
\boxed{\prod_{j\ {\rm even}}X_j},
$$

which generate $\mathbb Z_2\times\mathbb Z_2$.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Although the physical symmetry generators commute,

$$
V_aV_b=\sigma_x\sigma_z=-\sigma_z\sigma_x=-V_bV_a.
$$

Their virtual commutator is

$$
\boxed{
V_aV_bV_a^{-1}V_b^{-1}=-I}.
$$

This phase cannot be removed by rephasing $V_a$ and $V_b$. The virtual matrices therefore form a nontrivial projective representation, which is the nontrivial [projective virtual symmetry of a matrix product state](../../../topological-quantum-matter.md#projective-virtual-symmetry-of-a-matrix-product-state) and proves that the [cluster state](../../../topological-quantum-matter.md#cluster-state) lies in a nontrivial SPT phase.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/b/iv)

Under symmetry $g$, cyclicity changes the twist matrix by

$$
B\mapsto V_g^{-1}BV_g.
$$

Therefore its charge is the sign in this conjugation. With $V_a=X$ and $V_b=Z$,

$$
\begin{array}{c|cc}
B&\theta_B(a)&\theta_B(b)\\ \hline
I&+1&+1\\
V_a&+1&-1\\
V_b&-1&+1\\
V_aV_b&-1&-1
\end{array}
$$

The four twists realize all four characters of $\mathbb Z_2\times\mathbb Z_2$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Ignoring the common normalization $1/(2\sqrt2)$, direct multiplication gives

$$
|v(e_{00})\rangle
=|000\rangle+|001\rangle+|010\rangle-|011\rangle,
$$



$$
|v(e_{10})\rangle
=|000\rangle-|001\rangle+|010\rangle+|011\rangle,
$$



$$
|v(e_{01})\rangle
=|100\rangle+|101\rangle-|110\rangle+|111\rangle,
$$



$$
|v(e_{11})\rangle
=|100\rangle-|101\rangle-|110\rangle-|111\rangle.
$$

These four states span the positive eigenspace of $Z\otimes X\otimes Z$. The parent term annihilating that local MPS support is therefore the complementary projector

$$
\boxed{h=\frac12(I-Z\otimes X\otimes Z)}.
$$

Translated terms have stabilizers $K_j=Z_{j-1}X_jZ_{j+1}$. Two such Pauli strings either do not overlap nontrivially or have two X--Z anticommutations, so all $K_j$ commute. Their positive eigenspaces have a common state, making the parent Hamiltonian frustration free. Each alternating global X symmetry flips the two Z factors of every $K_j$ or neither, and therefore commutes with every local term.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

In the X eigenbasis, $M$ is $\operatorname{diag}(I,X)$ on its physical indices. A physical X insertion changes the sign of the minus block and can be pulled through as

$$
X_{\rm phys}M=Z_{\rm virt}MZ_{\rm virt}=MX_{\rm phys}.
$$

Conjugating both physical legs by Z swaps the two blocks:

$$
Z_{\rm phys}MZ_{\rm phys}
=M X_{\rm virt}
=X_{\rm virt}M.
$$

Hence

$$
\boxed{S=T=X}.
$$

Likewise $N=\operatorname{diag}(I,Z)$. Its analogous relations are

$$
X_{\rm phys}N=X_{\rm virt}NX_{\rm virt}=NX_{\rm phys},
$$



$$
Z_{\rm phys}NZ_{\rm phys}
=NZ_{\rm virt}
=Z_{\rm virt}N.
$$

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

Pulling the three operators of each cluster stabilizer through the alternating MPO cancels all internal virtual Pauli matrices and gives

$$
\boxed{
O\,(Z_{j-1}X_jZ_{j+1})
=(Z_{j-1}Z_{j+1})\,O}.
$$

Thus, for $H=\sum_j(I-K_j)/2$,

$$
\boxed{
H'=\frac12\sum_j(I-Z_{j-1}Z_{j+1})},
\qquad
OH=H'O.
$$

This is a pair of decoupled ferromagnetic Ising chains, one on each parity sublattice. Its four product ground states independently choose all odd spins up or down and all even spins up or down in the Z basis. In a symmetry-preserving basis they become four cat states.

The dual phase spontaneously breaks the two $\mathbb Z_2$ spin-flip symmetries. It has ordinary symmetry-breaking order and no nontrivial SPT invariant; the nonlocal MPO has converted the cluster SPT order into symmetry breaking.

## 4

↑ **Parent:** [Paper 343](paper-343.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The two-dimensional [Kramers--Wannier duality](../../../topological-quantum-matter.md#kramers-wannier-duality) PEPO has one physical input leg at every original vertex and one physical output leg at every edge. A COPY tensor at each vertex sends its binary value to all incident virtual legs. An XOR tensor on each edge compares the two incident virtual bits and writes their sum modulo two to the edge output. Contracting every vertex--edge virtual leg gives the graphical network

$$
\text{vertex COPY tensors}\;-\;\text{edge XOR tensors},
$$

repeated over the graph. In the X-Fourier basis the same network exchanges the COPY and parity constraints. This local tensor description is a [projected entangled pair operator](../../../quantum-theory.md#projected-entangled-pair-operator).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $Z_e$ denote the dual edge variable. The PEPO implements the domain-wall map

$$
Z_uZ_v\longleftrightarrow Z_{e=(uv)},
\qquad
X_v\longleftrightarrow
A_v=\prod_{e\ni v}X_e.
$$

Because edge domain walls arise from vertex spins, their product around every plaquette is constrained:

$$
B_p=\prod_{e\in\partial p}Z_e=1.
$$

Thus the transverse-field Ising operators map to the $\mathbb Z_2$ lattice-gauge operators, while the image is projected into the positive eigenspace of all $B_p$. At the commuting-projector fixed point, adjoining these automatic projectors gives

$$
\boxed{
H_{\rm TC}
=-\sum_vA_v-\sum_pB_p},
$$

the [toric code](../../../quantum-error-correction.md#toric-code) Hamiltonian. Conversely, solving the zero-flux constraint writes $Z_e=Z_uZ_v$ locally and recovers the Ising variables, establishing the duality on the supported symmetry sectors.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The original Ising symmetry is the global spin flip

$$
\boxed{U=\prod_vX_v}.
$$

The dual system has a [one-form symmetry](../../../topological-quantum-matter.md#one-form-symmetry) generated by products of edge Pauli operators along closed noncontractible loops; equivalently, closed Wilson loops label its electric and magnetic topological sectors.

The PEPO annihilates the nonsymmetric Ising sector because each virtual index is summed with the global parity constraint. On the dual side it has support only on configurations obeying all contractible zero-flux constraints and, for a fixed untwisted PEPO, one choice of noncontractible loop eigenvalues. Therefore the duality is invertible only after restricting both Hilbert spaces to corresponding symmetry sectors.

On a torus the [toric code](../../../quantum-error-correction.md#toric-code) has four ground states distinguished by two independent noncontractible loop eigenvalues. A single untwisted duality operator reaches only one of them; inserting the two possible Ising twists supplies the other three. This explains why the global-symmetry Ising description and topologically degenerate toric-code description do not contradict each other.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Violating a star stabilizer $A_v$ creates an electric $e$ particle; violating a plaquette stabilizer $B_p$ creates a magnetic $m$ particle. Open Z strings create pairs of $e$ endpoints, while open X strings create pairs of $m$ endpoints. Their fusion $\epsilon=e\times m$ is the third nontrivial particle type.

Two equal-type strings can be exchanged without a phase, so $e$ and $m$ have bosonic self-statistics. An X string and a Z string crossing once anticommute, so taking $e$ around $m$ gives phase $-1$: they are [mutual semions](../../../topological-quantum-matter.md#mutual-semion). Combining these two mutual-semion species gives

$$
\boxed{\theta_e=\theta_m=+1,\qquad
M_{em}=-1,\qquad
\theta_\epsilon=-1}.
$$

**Thus $\epsilon$ is a fermion.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
