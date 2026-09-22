# Paper 60

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper60.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper60.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
  - [f](#5/f)
    - [Solution](#5/f/solution)

## 1

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the real [vector space](../../../vector-space.md) of [Hermitian matrices](../../../hilbert-space.md#hermitian-operator) and its [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) $\langle A,B\rangle=\operatorname{Tr}(AB)$. A Hermitian $N$-by-$N$ [matrix](../../../vector-space.md#matrix) has $N$ real diagonal entries and two real parameters for each off-diagonal pair, hence real dimension $N+2\binom N2=N^2$. Imposing zero [trace](../../../linear-algebra.md#matrix-trace) removes one real dimension. Each supplied [generalized Pauli matrix](../../../algebra.md#generalized-pauli-matrix) is Hermitian and traceless, and there are $N(N-1)$ off-diagonal matrices and $N-1$ diagonal matrices, totaling $N^2-1$.

Their assumed [orthonormality](../../../linear-algebra.md#orthonormal-set) makes them linearly independent. Since this equals the dimension of the traceless space, **they are an orthonormal basis of the traceless Hermitian matrices**. To extend the family, the required additional generator is $\sigma_0=I/\sqrt N$, which is implicit in the indexing of the question. It has unit [Hilbert-Schmidt norm](../../../compact-operator.md#hilbert-schmidt-norm) and is orthogonal to every traceless generator, so the extended family is an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of all Hermitian matrices.

For a [density operator](../../../quantum-theory.md#density-matrix) $\rho$, cyclicity of the [trace](../../../linear-algebra.md#matrix-trace) gives

$$
s_k^*=\operatorname{Tr}((\rho\sigma_k)^\dagger)=\operatorname{Tr}(\sigma_k\rho)=\operatorname{Tr}(\rho\sigma_k)=s_k.
$$

Thus **$s\in\mathbb R^{N^2-1}$**. Since $\operatorname{Tr}\rho=1$, the resulting [Generalized Bloch representation](../../../quantum-theory.md#generalized-bloch-representation) is

$$
\rho=\frac IN+\sum_{k=1}^{N^2-1}s_k\sigma_k.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

By [orthonormality](../../../linear-algebra.md#orthonormal-set) in the [Generalized Bloch representation](../../../quantum-theory.md#generalized-bloch-representation),

$$
\operatorname{Tr}(\rho^2)=\frac1N+\sum_{k=1}^{N^2-1}s_k^2.
$$

A [pure state](../../../quantum-theory.md#pure-state) has [density operator](../../../quantum-theory.md#density-matrix) $\rho=|\psi\rangle\langle\psi|$ with $\langle\psi|\psi\rangle=1$, so $\rho^2=\rho$ and its [purity of a density operator](../../../quantum-theory.md#purity-of-a-density-operator) is one. Consequently

$$
\boxed{\|s\|^2=1-\frac1N.}
$$

Every [pure state](../../../quantum-theory.md#pure-state) therefore maps to the specified radius-$\sqrt{1-1/N}$ [sphere](../../../geometry-and-topology.md#sphere) in $\mathbb R^{N^2-1}$, of dimension $N^2-2$. The expansion is unique, so it distinguishes pure-state [density operators](../../../quantum-theory.md#density-matrix), while vectors differing only by [global phase](../../../quantum-mechanics.md#global-phase) describe the same point. This proves that pure states lie on the sphere, without asserting that they fill it.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Take any rank-one [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) $P$ and its generalized [Bloch vector](../../../quantum-theory.md#bloch-vector) $s$. The antipodal vector $-s$ is on the same [sphere](../../../geometry-and-topology.md#sphere), but its corresponding trace-one [Hermitian matrix](../../../hilbert-space.md#hermitian-operator) is

$$
\rho_- =\frac IN-\left(P-\frac IN\right)=\frac2N I-P.
$$

On the range of $P$, this [matrix](../../../vector-space.md#matrix) has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $2/N-1$, which is negative for $N>2$. It is therefore not a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) and cannot be a [density operator](../../../quantum-theory.md#density-matrix). Hence **the pure states do not cover the sphere when $N>2$**. This also shows directly why the [purity bound for generalized Bloch vectors](../../../quantum-theory.md#purity-bound-for-generalized-bloch-vectors) does not by itself guarantee a physical [quantum state](../../../quantum-mechanics.md#quantum-state).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $p_j$ of a [density operator](../../../quantum-theory.md#density-matrix) are nonnegative and sum to one. Therefore

$$
1-\operatorname{Tr}(\rho^2)=\left(\sum_jp_j\right)^2-\sum_jp_j^2=2\sum_{j<k}p_jp_k.
$$

For a non-pure state at least two [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are positive, so the last expression is strictly positive. Combining this with the [Generalized Bloch representation](../../../quantum-theory.md#generalized-bloch-representation) gives

$$
\boxed{\|s\|^2=\operatorname{Tr}(\rho^2)-\frac1N<1-\frac1N.}
$$

Thus every non-pure [quantum state](../../../quantum-mechanics.md#quantum-state) lies strictly inside the radius sphere for $N\geq2$. It need not be an interior point of the entire physical state body: for $N>2$, a rank-deficient mixed [density operator](../../../quantum-theory.md#density-matrix) can lie on that body's boundary while still lying inside the Euclidean sphere.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Write the [unitary conjugation](../../../vector-space.md#unitary-conjugation) as $\rho(t)=U(t)\rho(0)U(t)^\dagger$. The identity component is unchanged, and the generalized [Bloch vector](../../../quantum-theory.md#bloch-vector) transforms by

$$
s_k(t)=\sum_\ell O_{k\ell}(U(t))s_\ell(0),\qquad O_{k\ell}(U)=\operatorname{Tr}(\sigma_kU\sigma_\ell U^\dagger).
$$

These coefficients are real, by the same trace argument as in part (a). [Unitary conjugation](../../../vector-space.md#unitary-conjugation) preserves the [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product), so the conjugated traceless generators form another [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). It follows that $O(U)^TO(U)=I$. The [unitary group](../../../topological-group.md#unitary-group) is connected, $O(I)=I$, and the [determinant](../../../linear-algebra.md#determinant) of an orthogonal [matrix](../../../vector-space.md#matrix) is $\pm1$; hence $\det O(U)=1$. Thus **Hamiltonian evolution rotates the generalized Bloch vector by an element of $SO(N^2-1)$**.

Equivalently, in units $\hbar=1$, the [Von Neumann equation](../../../quantum-theory.md#von-neumann-equation) gives

$$
\dot s_k=\sum_\ell A_{k\ell}s_\ell,\qquad A_{k\ell}=-i\operatorname{Tr}(\sigma_k[H,\sigma_\ell]).
$$

Cyclicity of the [trace](../../../linear-algebra.md#matrix-trace) shows $A_{k\ell}=-A_{\ell k}$, so $A$ is a real [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix). This is the generator form of [Hamiltonian rotations of Bloch vectors](../../../quantum-theory.md#hamiltonian-rotations-of-bloch-vectors), valid also for a time-dependent [Quantum Hamiltonian](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics). For $N>2$, Hamiltonians generally realize only a proper subgroup of all rotations of this real space; they preserve the whole density-operator [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis), not merely its [purity of a density operator](../../../quantum-theory.md#purity-of-a-density-operator).

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The individual rates describe [population relaxation](../../../quantum-theory.md#population-relaxation): $\gamma_{12}$ transfers population from level one to level two, and $\gamma_{21}$ transfers it back. With $p_1+p_2=1$ and the conventional qubit coordinate $r_z=p_1-p_2$,

$$
\dot p_1=-\gamma_{12}p_1+\gamma_{21}p_2,\qquad \dot r_z=-(\gamma_{12}+\gamma_{21})r_z+(\gamma_{21}-\gamma_{12}).
$$

Thus $T_1^{-1}=\gamma_{12}+\gamma_{21}$ is the longitudinal relaxation rate. The parameter $\Gamma=T_2^{-1}$ is the [transverse relaxation](../../../quantum-theory.md#transverse-relaxation) rate: it damps the off-diagonal coherence, or the $x,y$ components of the [Bloch vector](../../../quantum-theory.md#bloch-vector). In the usual completely positive two-level model,

$$
\Gamma=\frac12(\gamma_{12}+\gamma_{21})+\gamma_\phi,\qquad\gamma_\phi\geq0,
$$

so $\Gamma$ includes both the coherence loss caused by [population relaxation](../../../quantum-theory.md#population-relaxation) and additional pure [dephasing](../../../quantum-information-theory.md#dephasing-channel).

There is a normalization switch in the displayed qubit [Affine Bloch equation](../../../quantum-theory.md#affine-bloch-equation). Its constant term is appropriate to the conventional [Pauli matrices](../../../algebra.md#pauli-matrices) and unit-radius coordinate $r_k=\operatorname{Tr}(\rho\sigma_k^{\mathrm{Pauli}})$. With the orthonormal generators used earlier, $s=r/\sqrt2$, the same physical rates would instead give a constant term $(\gamma_{21}-\gamma_{12})/\sqrt2$. The drift matrix is unchanged. We interpret the supplied qubit equation in its conventional $r$ coordinates.

With zero controls and $g=\gamma_{12}+\gamma_{21}>0$, $\Gamma>0$, the [steady state](../../../dynamical-systems.md#steady-state) is unique:

$$
\boxed{r_*=(0,0,(\gamma_{21}-\gamma_{12})/g),\qquad \rho_* =\operatorname{diag}(\gamma_{21}/g,\gamma_{12}/g).}
$$

The earlier normalized vector is $s_*=r_*/\sqrt2$. Indeed $r_x,r_y$ decay as $e^{-\Gamma t}$ and $r_z-r_{*,z}$ as $e^{-gt}$.

For vanishing rates, the full equilibrium conditions of the [Affine Bloch equation](../../../quantum-theory.md#affine-bloch-equation) are $\Gamma r_x=\Gamma r_y=0$ and $g r_z=\gamma_{21}-\gamma_{12}$, together with $\|r\|\leq1$. In particular, for nonnegative rates, $g=0$ means both population rates vanish. If then $\Gamma>0$, all diagonal [density operators](../../../quantum-theory.md#density-matrix) are stationary; if also $\Gamma=0$, every [density operator](../../../quantum-theory.md#density-matrix) is stationary. The formal case $g>0$, $\Gamma=0$ permits extra transverse equilibrium coordinates, but is excluded by the completely positive rate bound above.

## 2

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In units $\hbar=1$, a [bilinear Hamiltonian control system](../../../control-theory.md#bilinear-hamiltonian-control-system) has

$$
\dot U(t)=-i\left(H_0+\sum_{k=1}^m u_k(t)H_k\right)U(t),\qquad U(0)=I,
$$

where the [Hermitian matrices](../../../hilbert-space.md#hermitian-operator) $H_0,H_k$ are fixed, and the real functions $u_k$ are admissible [control inputs](../../../control-theory.md#control-input). The corresponding vector or [density operator](../../../quantum-theory.md#density-matrix) dynamics are $\dot\psi=-iH(u)\psi$ or $\dot\rho=-i[H(u),\rho]$. The dynamics are linear in the state at fixed input and affine in the inputs at fixed state; this is the bilinear terminology.

The [reachable set](../../../control-theory.md#reachable-set) from an initial state $x_0$ at time $T$ is $\mathcal R_T(x_0)=\{x(T;x_0,u):u\text{ admissible}\}$. With freely chosen duration, take $\mathcal R(x_0)=\bigcup_{T\geq0}\mathcal R_T(x_0)$. **Controllability means every allowed target is reachable from every allowed initial state**. The allowed space and phase convention must be specified. For closed [quantum control](../../../control-theory.md#quantum-control), [density operators](../../../quantum-theory.md#density-matrix) remain on their initial [unitary orbit of a density operator](../../../quantum-theory.md#unitary-orbit-of-a-density-operator), rather than becoming arbitrary density operators with different [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A real [Lie algebra](../../../lie-algebra.md) is a real [vector space](../../../vector-space.md) with a bilinear antisymmetric bracket satisfying the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). For [matrices](../../../vector-space.md#matrix), the bracket is the [commutator](../../../lie-algebra.md#commutator) $[X,Y]=XY-YX$. The [Dynamical Lie algebra](../../../control-theory.md#dynamical-lie-algebra) is

$$
\mathfrak g=\operatorname{Lie}_{\mathbb R}\{iH_0,iH_1,\ldots,iH_m\}\subseteq\mathfrak u(N).
$$

It is found by repeatedly adjoining [commutators](../../../lie-algebra.md#commutator) and taking real linear spans until no new independent generators appear. Let $G$ be its connected dynamical [Lie group](../../../lie-theory.md#lie-group). Under the standard assumptions of freely timed controls with unrestricted real amplitudes, the following are the relevant Lie criteria.

For [pure-state controllability](../../../control-theory.md#pure-state-controllability), $G$ must act transitively on normalized state vectors, or on their rays when [global phase](../../../quantum-mechanics.md#global-phase) is disregarded. The standard finite-dimensional classification is, up to a unitary change of basis,

$$
\mathfrak g=\mathfrak u(N),\quad\mathfrak{su}(N),\quad\text{or, for }N=2n,\quad\mathfrak{sp}(n),\quad\mathfrak{sp}(n)\oplus\mathbb R iI.
$$

Here $\mathfrak{sp}(n)$ is the [compact symplectic Lie algebra](../../../semisimple-lie-algebra.md#compact-symplectic-lie-algebra) in its defining complex $2n$-dimensional representation. Equivalently, the infinitesimal action spans the tangent directions to the whole pure-state orbit. The symplectic cases are important because pure-state reachability alone need not give complete mixed-state reachability.

For [density operator controllability](../../../control-theory.md#density-operator-controllability), the action must be transitive on every [unitary orbit of a density operator](../../../quantum-theory.md#unitary-orbit-of-a-density-operator), meaning on every fixed-spectrum class. The criterion is **$\mathfrak g=\mathfrak{su}(N)$ or $\mathfrak u(N)$**. This concerns all [density operators](../../../quantum-theory.md#density-matrix), not merely one unusually degenerate spectrum.

For exact [unitary operator controllability](../../../control-theory.md#unitary-operator-controllability), the criterion is **$\mathfrak g=\mathfrak u(N)$**. If only the physical gate up to [global phase](../../../quantum-mechanics.md#global-phase) matters, it is enough that the image after removing the scalar direction is $\mathfrak{su}(N)$, equivalently that $\mathfrak g+\mathbb R iI=\mathfrak u(N)$. A traceless system can implement all special-unitary gates while lacking independent control of the overall phase.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Set $X_j=iH_j$. The symplectic Lie condition is $X_j^TJ+JX_j=0$, equivalently $H_j^TJ+JH_j=0$. For the supplied diagonal $H_0$, the nonzero entries of $J$ pair levels $1,4$ and $2,3$; the corresponding energy sums are $-\alpha+\alpha=0$ and $-\beta+\beta=0$. Thus $H_0J+JH_0=0$ for all real $\alpha,\beta$.

For the supplied real symmetric control [matrix](../../../vector-space.md#matrix), direct multiplication gives

$$
H_1J=\begin{pmatrix}0&0&1&0\\0&-1&0&1\\1&0&1&0\\0&1&0&0\end{pmatrix}=-JH_1.
$$

Both generators therefore satisfy the same alternating-form condition. That condition is closed under real linear combinations, and for two such generators

$$
[X,Y]^TJ=-J[X,Y],
$$

as follows by substituting $X^TJ=-JX$ and $Y^TJ=-JY$ into $(XY)^TJ-(YX)^TJ$. Hence the whole [Dynamical Lie algebra](../../../control-theory.md#dynamical-lie-algebra) obeys it.

If $\dot U=X(t)U$ and $U(0)=I$, differentiating gives

$$
\frac d{dt}(U^TJU)=U^T(X^TJ+JX)U=0.
$$

Thus **every reachable propagator satisfies $U^TJU=J$**. Also $J^T=-J$, $J^\dagger J=I$, so this is a [symplectic dynamical symmetry in quantum control](../../../control-theory.md#symplectic-dynamical-symmetry-in-quantum-control): the generated group lies in the corresponding [compact symplectic group](../../../topological-group.md#compact-symplectic-group), unitarily equivalent to $Sp(2)$. It is not necessary to claim equality with $Sp(2)$, and special choices of $\alpha,\beta$ can give a smaller group.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The two [density operators](../../../quantum-theory.md#density-matrix) have the same [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $a,a,b,b$, so a permutation of basis vectors makes them [unitarily equivalent](../../../vector-space.md#unitary-equivalence). A dynamical equivalence must additionally respect the [symplectic dynamical symmetry in quantum control](../../../control-theory.md#symplectic-dynamical-symmetry-in-quantum-control).

Define the symplectic dual $\widetilde\rho=J\rho^TJ^\dagger$. For a unitary $U$ preserving $J$, both $U^TJU=J$ and $UJU^T=J$ hold. In particular $JU^*=UJ$, and therefore

$$
\widetilde{U\rho U^\dagger}=J U^*\rho^T U^T J^\dagger=U\widetilde\rho U^\dagger.
$$

It follows by cyclicity of the [trace](../../../linear-algebra.md#matrix-trace) that the [symplectic invariant of a density operator](../../../control-theory.md#symplectic-invariant-of-a-density-operator)

$$
I_J(\rho)=\operatorname{Tr}(\rho\widetilde\rho)
$$

is unchanged by every reachable [unitary conjugation](../../../vector-space.md#unitary-conjugation). The given $J$ reverses the diagonal order, so

$$
\widetilde\rho_0=\operatorname{diag}(b,b,a,a),\qquad\widetilde\rho_1=\operatorname{diag}(a,b,b,a)=\rho_1.
$$

Consequently

$$
I_J(\rho_0)=4ab,\qquad I_J(\rho_1)=2(a^2+b^2),\qquad I_J(\rho_1)-I_J(\rho_0)=2(a-b)^2>0.
$$

Hence **the states are not dynamically equivalent**, despite their identical ordinary spectra. This works for all the allowed values, including $a=0$, and for any subgroup satisfying the symmetry in part (c).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Let $P_0,P_1$ be any two rank-one [orthogonal projections](../../../hilbert-space.md#orthogonal-projection). Choose $0<q<1/N$ and $p=1-(N-1)q$, so $p>q$, and form the mixed [density operators](../../../quantum-theory.md#density-matrix)

$$
\rho_j=qI+(p-q)P_j.
$$

They have the same [spectrum](../../../linear-operator-theory.md#spectrum-functional-analysis). If [density operator controllability](../../../control-theory.md#density-operator-controllability) holds, a reachable $U$ obeys $U\rho_0U^\dagger=\rho_1$, and subtraction of $qI$ gives $UP_0U^\dagger=P_1$. Thus **density operator controllability implies pure-state controllability**, even if its definition is phrased using only mixed density operators.

The converse is false in general. For $N=4$, the full [compact symplectic group](../../../topological-group.md#compact-symplectic-group) $Sp(2)$ is transitive on the complex unit sphere: identify $\mathbb C^4$ with $\mathbb H^2$, extend any quaternionic unit vector to an orthonormal quaternionic basis, and map one such basis to another. This gives [pure-state controllability](../../../control-theory.md#pure-state-controllability). Yet the invariant in part (d) prevents it from connecting the indicated isospectral mixed [density operators](../../../quantum-theory.md#density-matrix), so it fails [density operator controllability](../../../control-theory.md#density-operator-controllability). This counterexample uses the full symplectic group, not an assertion that every parameter choice in part (c) generates it.

For $N=2$, the converse is true. Every [density operator](../../../quantum-theory.md#density-matrix) has the form $\rho=qI+(p-q)P$ for a rank-one $P$, with $p+q=1$. If $p\ne q$, pure-state control of $P$ controls its entire fixed-spectrum [unitary orbit of a density operator](../../../quantum-theory.md#unitary-orbit-of-a-density-operator). If $p=q=1/2$, the orbit contains only $I/2$. Therefore **the two controllability notions coincide for a qubit**. The Lie classification gives the same conclusion, since $Sp(1)=SU(2)$.

## 3

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Since $A$ is a [bounded operator](../../../topological-vector-space.md#continuous-linear-operator), its exponential [power series](../../../real-analysis.md#power-series) converges in [operator norm](../../../continuous-dual-space.md#operator-norm). The identity $A^2=I$ gives $A^{2k}=I$ and $A^{2k+1}=A$. Separating the even and odd powers therefore gives

$$
e^{-i\theta A}=\sum_{k=0}^\infty\frac{(-1)^k\theta^{2k}}{(2k)!}I-i\sum_{k=0}^\infty\frac{(-1)^k\theta^{2k+1}}{(2k+1)!}A=\boxed{\cos\theta\,I-i\sin\theta\,A.}
$$

The algebraic identity does not require $A$ to be Hermitian. Hermiticity is additionally needed for this exponential to be a [unitary operator](../../../vector-space.md#unitary-operator) for real $\theta$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A general single-[qubit](../../../quantum-mechanics.md#qubit) [quantum gate](../../../quantum-circuit.md#quantum-logic-gate) belongs to $U(2)$. Remove its [global phase](../../../quantum-mechanics.md#global-phase) to obtain $V\in SU(2)$; the displayed expression in the question is literally a special-unitary gate and represents a general physical gate up to that phase. Every $V\in SU(2)$ can be written

$$
V=\begin{pmatrix}u&v\\-v^*&u^*\end{pmatrix},\qquad |u|^2+|v|^2=1,
$$

and consequently

$$
V=q_0 I-i(q_x\sigma_x+q_y\sigma_y+q_z\sigma_z),\qquad q_0,q_x,q_y,q_z\in\mathbb R,\quad q_0^2+q_x^2+q_y^2+q_z^2=1.
$$

Choose $\theta$ with $q_0=\cos(\theta/2)$ and $\|q\|=\sin(\theta/2)$, and set $n=q/\|q\|$ when $q\ne0$. The [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) shows $(n\cdot\sigma)^2=\|n\|^2I=I$. Applying part (a) proves

$$
\boxed{U=e^{i\chi}e^{-i\theta(n\cdot\sigma)/2},\qquad \|n\|=1.}
$$

For $q=0$, $V=\pm I$ and any axis can be used with angle zero or $2\pi$. Thus the phase-free gate is a [rotation gate](../../../quantum-circuit.md#rotation-gate) by angle $\theta$ about the unit axis $n$. An arbitrary exact $U(2)$ operator also needs the scalar phase $e^{i\chi}$, which cannot in general be produced by a traceless [Quantum Hamiltonian](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

With $B_y=0$, a pulse of the $x$ field realizes $R_x(\theta)=e^{-i\theta\sigma_x/2}$ when $\int B_x(t)dt=\theta/2$. Similarly the $y$ field realizes $R_y(\theta)$ with area $\theta/2$. These are instances of the [quantum pulse area](../../../control-theory.md#quantum-pulse-area) rule. A [rotation about the z-axis](../../../quantum-circuit.md#rotation-about-the-z-axis) can be synthesized from the two available axes:

$$
R_z(\theta)=R_x(\pi/2)R_y(\theta)R_x(-\pi/2),
$$

because $R_x(\pi/2)\sigma_yR_x(-\pi/2)=\sigma_z$.

For a target $V=\begin{pmatrix}u&v\\-v^*&u^*\end{pmatrix}$, one convenient construction is

$$
V=R_z(\alpha)R_y(\beta)R_z(\gamma),\qquad
u=e^{-i(\alpha+\gamma)/2}\cos(\beta/2),\quad v=-e^{-i(\alpha-\gamma)/2}\sin(\beta/2).
$$

Take $\beta=2\operatorname{atan2}(|v|,|u|)$ and choose $\alpha+\gamma=-2\arg u$, $\alpha-\gamma=-2\arg(-v)$ when both entries are nonzero; if an entry vanishes its phase constraint can be omitted. Substitute the three-pulse construction for each $z$ rotation. Apply the factors from right to left in time. **Pulses along the available $x,y$ axes therefore implement every single-qubit gate up to global phase**. Negative angles use negative field area, or an equivalent full-period rotation.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write $X=\sigma_x$, $Y=\sigma_y$, $Z=\sigma_z$. The specified diagonal [two-qubit gate](../../../quantum-circuit.md#two-qubit-gate) has the exact factorization

$$
C_{\mathrm{phase}}=-Z\otimes Z=R_z(\pi)\otimes R_z(\pi).
$$

Thus one exact implementation is to set the controllable [Ising coupling](../../../control-theory.md#ising-coupling-of-two-qubits) to zero and perform the two local [rotations about the z-axis](../../../quantum-circuit.md#rotation-about-the-z-axis), synthesized from the available $x,y$ pulses as in part (c). Alternatively, turn off the local fields and choose the interaction area $\int J_{12}(t)dt=\pi/2$. Then

$$
U_I=e^{-i\pi Z\otimes Z/2}=-iZ\otimes Z=iC_{\mathrm{phase}},
$$

which implements the same physical gate up to [global phase](../../../quantum-mechanics.md#global-phase). **The printed gate is local, not entangling**; the pulse construction does not change that fact.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The claimed universality is false for the particular gate specified in part (d). Every allowed single-[qubit](../../../quantum-mechanics.md#qubit) gate is local, and $C_{\mathrm{phase}}=-Z\otimes Z$ is local too. Products of these gates remain of the form $e^{i\chi}A\otimes B$. They preserve all [product states](../../../bell-state.md#product-state) and cannot, for example, implement the [CNOT gate](../../../quantum-theory.md#controlled-not-gate) that sends $|+\rangle\otimes|0\rangle$ to $(|00\rangle+|11\rangle)/\sqrt2$. Equivalently, its [diagonal two-qubit phase entanglement criterion](../../../quantum-circuit.md#diagonal-two-qubit-phase-entanglement-criterion) gives the alternating phase $\pi-0-0+\pi=0$ modulo $2\pi$. **No construction with only the printed phase gate and local rotations implements arbitrary two-qubit gates**.

The intended universality argument works after replacing that local gate by an entangling controlled phase. The same tunable [Ising coupling](../../../control-theory.md#ising-coupling-of-two-qubits) supplies

$$
V=e^{-i\pi Z\otimes Z/4},\qquad
\mathrm{CZ}=e^{-i\pi/4}\{R_z(-\pi/2)\otimes R_z(-\pi/2)\}V=\operatorname{diag}(1,1,1,-1).
$$

Thus this quarter-area Ising pulse, with local corrections, realizes the [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate). Conjugating it by the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) on the second qubit gives $\mathrm{CNOT}=(I\otimes H)\mathrm{CZ}(I\otimes H)$, with harmless scalar phases if the Hadamards are implemented using traceless control Hamiltonians.

The [Cartan decomposition of a two-qubit gate](../../../quantum-circuit.md#cartan-decomposition-of-a-two-qubit-gate) writes a target as

$$
U=e^{i\chi}(A_1\otimes A_2)e^{-i(c_xX\otimes X+c_yY\otimes Y+c_zZ\otimes Z)}(B_1\otimes B_2),
$$

with local $SU(2)$ factors. The three central Pauli-product operators commute, so their exponential is a product of three variable interaction gates. From two fixed [CNOT gates](../../../quantum-theory.md#controlled-not-gate) and a variable local [rotation about the z-axis](../../../quantum-circuit.md#rotation-about-the-z-axis),

$$
\mathrm{CNOT}\{I\otimes R_z(2c)\}\mathrm{CNOT}=e^{-icZ\otimes Z},
$$

because $\mathrm{CNOT}(I\otimes Z)\mathrm{CNOT}=Z\otimes Z$. Conjugating this interaction by $R_y(\pi/2)$ on both qubits yields $e^{-icX\otimes X}$; conjugating by $R_x(-\pi/2)$ on both yields $e^{-icY\otimes Y}$. Part (c) implements all outer local factors. This gives the full requested Cartan construction with an entangling phase gate, and pinpoints the defect in the printed version. Exact arbitrary scalar phase requires an identity Hamiltonian term; the physical gate construction is up to [global phase](../../../quantum-mechanics.md#global-phase).

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

An always-on [Ising coupling](../../../control-theory.md#ising-coupling-of-two-qubits) produces evolution during every nominally local pulse, and generally does not commute with the applied $x,y$ [Quantum Hamiltonians](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics). A naive product of single-[qubit](../../../quantum-mechanics.md#qubit) rotations therefore accumulates unwanted conditional phases and can entangle the qubits. Idling is also no longer an identity operation.

For a pulse of duration $\tau$, neglecting the coupling requires **$|J_{12}|\tau\ll1$** in units $\hbar=1$, or $|J_{12}|\tau/\hbar\ll1$ in ordinary units. For order-one rotation angles, this is the strong-local-drive regime $|B|\gg|J_{12}|$. Large drive amplitude alone does not justify neglect over a long total sequence: the accumulated interaction time or an appropriate error bound must also be small.

If it cannot be neglected, include it in the [quantum optimal control](../../../control-theory.md#quantum-optimal-control) model, or refocus it. A $\pi$ pulse $P=R_x^{(1)}(\pi)$ obeys $P(Z\otimes Z)P^\dagger=-Z\otimes Z$, giving the ideal [Ising spin echo](../../../control-theory.md#ising-spin-echo)

$$
e^{-iH_I\tau/2}P e^{-iH_I\tau/2}P^\dagger=I.
$$

This cancellation assumes the refocusing pulses are instantaneous relative to $1/|J_{12}|$, or that the coupling during finite pulses is compensated. It explains how fast local controls can suppress the fixed coupling without mistaking it for a controllable zero interaction.

## 4

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

An [open-loop control](../../../control-theory.md#open-loop-control) is computed from a dynamical model and the initial preparation, then applied without changing it in response to measurements during that run. [Controllability](../../../control-theory.md#controllability) determines which transformations are possible in principle; field design must also account for duration, available control generators, amplitude and bandwidth limits, and calibration errors.

Three useful model-based strategies are the following. [Resonant quantum control](../../../control-theory.md#resonant-quantum-control) chooses carrier frequencies and phases to select transitions, and uses [quantum pulse area](../../../control-theory.md#quantum-pulse-area) or elementary [rotation gates](../../../quantum-circuit.md#rotation-gate) to compile the desired transformation. [Adiabatic quantum control](../../../control-theory.md#adiabatic-quantum-control) chooses a slowly varying path of [Quantum Hamiltonians](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) whose relevant eigenstate connects the initial and target states, maintaining a sufficiently large [spectral gap](../../../linear-operator-theory.md#spectral-gap). [Quantum optimal control](../../../control-theory.md#quantum-optimal-control) parametrizes or varies the fields and maximizes a fidelity or observable objective, while penalizing resources and enforcing the dynamical equations. These can all produce predetermined laboratory waveforms; experimental feedback is a separate design choice.

For a detailed variational construction, let

$$
H(u,t)=H_0+\sum_{k=1}^m u_k(t)H_k,\qquad i\hbar\dot\psi=H(u,t)\psi,\qquad\psi(0)=\psi_0.
$$

Choose a positive target observable $O$, for example $O=|\psi_d\rangle\langle\psi_d|$ for pure-state transfer. Maximize

$$
J[u]=\langle\psi(T)|O|\psi(T)\rangle-\frac12\sum_k\lambda_k\int_0^T u_k(t)^2\,dt,\qquad\lambda_k>0.
$$

The terminal term is the target probability or observable [expectation](../../../probability-theory.md#expected-value), and the quadratic integral penalizes field energy. A [costate](../../../control-theory.md#costate) $\chi(t)$ enforces the [Schrödinger equation](../../../physics.md#schrodinger-equation) through the real augmented functional

$$
\mathcal J=J-2\operatorname{Re}\int_0^T\left\langle\chi\middle|\dot\psi+\frac i\hbar H(u,t)\psi\right\rangle dt.
$$

Variation in $\chi$ recovers the state equation. Integrating the variation in $\dot\psi$ by parts gives the terminal boundary term $2\operatorname{Re}\langle O\psi(T)-\chi(T)|\delta\psi(T)\rangle$ and the interior adjoint equation. Thus the Euler-Lagrange conditions are

$$
\boxed{i\hbar\dot\psi=H\psi,\quad\psi(0)=\psi_0;\qquad i\hbar\dot\chi=H\chi,\quad\chi(T)=O\psi(T).}
$$

The [costate](../../../control-theory.md#costate) obeys the same Hamiltonian equation but is propagated backward from its terminal value. The field variation is

$$
\delta\mathcal J=\sum_k\int_0^T\left\{\frac2\hbar\operatorname{Im}\langle\chi(t)|H_k|\psi(t)\rangle-\lambda_k u_k(t)\right\}\delta u_k(t)\,dt.
$$

Hence the [variational costate gradient for Hamiltonian quantum control](../../../control-theory.md#variational-costate-gradient-for-hamiltonian-quantum-control) is

$$
g_k(t)=\frac{\delta J}{\delta u_k(t)}=\frac2\hbar\operatorname{Im}\langle\chi(t)|H_k|\psi(t)\rangle-\lambda_k u_k(t).
$$

At an unconstrained stationary field,

$$
\boxed{u_k(t)=\frac2{\hbar\lambda_k}\operatorname{Im}\langle\chi(t)|H_k|\psi(t)\rangle.}
$$

These equations couple forward and backward boundary data, so this is not a single initial-value integration, nor a direct feedback law for an unknown experimental state.

A practical [direct-adjoint looping](../../../control-theory.md#direct-adjoint-looping) algorithm starts from an admissible trial field. Propagate $\psi$ forward and store its trajectory; set $\chi(T)=O\psi(T)$ and propagate $\chi$ backward; compute $g_k$ along the two trajectories; then update $u_k^{\mathrm{new}}=u_k+\eta g_k$ for a positive step size $\eta$. A line search evaluates the actual objective and decreases $\eta$ until the ascent condition is met. Project into the admissible amplitude range or optimize a finite Fourier or pulse basis to enforce bandwidth constraints. Repeat until the projected gradient and change in objective are small. Repeated initializations help explore different local optima; the stationarity equations alone do not guarantee a global optimum.

For a piecewise constant discretization, define $H_j=H_0+\sum_k u_{k,j}H_k$ and $U_j=e^{-i\Delta tH_j/\hbar}$. Forward multiplication gives the state trajectory; backward multiplication gives the [costate](../../../control-theory.md#costate). The exact matrix-exponential derivative is

$$
\frac{\partial U_j}{\partial u_{k,j}}=-\frac i\hbar\int_0^{\Delta t}e^{-i(\Delta t-s)H_j/\hbar}H_k e^{-isH_j/\hbar}\,ds.
$$

This supplies accurate discrete gradients even when $H_j$ and $H_k$ do not commute. The small-step expression $\partial U_j/\partial u_{k,j}\simeq-i\Delta tH_kU_j/\hbar$ is only an approximation. Forward/backward factorization is the basis of [gradient ascent pulse engineering](../../../control-theory.md#gradient-ascent-pulse-engineering). For a full-gate objective, propagate all basis columns or $U(t)$ itself and use a terminal objective such as the [phase-insensitive unitary gate error](../../../control-theory.md#phase-insensitive-unitary-gate-error); optimizing one state alone does not implement a prescribed operation on every input.

To implement the result, convert the optimized envelope and quadratures into the calibrated electric or magnetic drive fields. An arbitrary-waveform source can set time-domain quadratures; optical [spectral pulse shaping](../../../optics.md#spectral-pulse-shaping) applies a complex mask to the available pulse spectrum,

$$
\widetilde E_{\mathrm{out}}(\omega)=M(\omega)\widetilde E_{\mathrm{in}}(\omega),
$$

using, for example, a [4f pulse shaper](../../../optics.md#4f-pulse-shaper) and [spatial light modulator](../../../optics.md#spatial-light-modulator). Finite spectral support, mask resolution and actuator limits must be included in the optimization: smoothing an unconstrained optimum afterward may spoil it. Simulating the calibrated final pulse, optionally over an ensemble of detunings or calibration errors, checks its predicted fidelity and robustness. The computed fields are then executed as [open-loop control](../../../control-theory.md#open-loop-control), with all measurements used for later calibration rather than an assumed instantaneous state readout.

## 5

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use units $\hbar=1$. A Hermitian quadrature coupling of a cavity mode to a continuum of external modes can be written

$$
H_{\mathrm{couple}}=i\int d\omega\,\kappa(\omega)(a+a^\dagger)\otimes(b_\omega^\dagger-b_\omega),
$$

with real coupling amplitude $\kappa$. The free [Quantum Hamiltonian](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) is $H_0=\omega_ca^\dagger a+\int\omega b_\omega^\dagger b_\omega\,d\omega$. In the [interaction picture](../../../quantum-mechanics.md#interaction-picture), the two photon-exchange products $ab_\omega^\dagger$ and $a^\dagger b_\omega$ acquire phases with frequency $\omega-\omega_c$, whereas $a^\dagger b_\omega^\dagger$ and $ab_\omega$ oscillate at $\omega+\omega_c$.

For weak coupling near resonance, the [rotating-wave approximation](../../../quantum-mechanics.md#rotating-wave-approximation) drops those rapidly oscillating pair-creation and pair-annihilation terms and retains

$$
H_I(t)=i\int d\omega\,\kappa(\omega)\{a\otimes b_\omega^\dagger e^{i(\omega-\omega_c)t}-a^\dagger\otimes b_\omega e^{-i(\omega-\omega_c)t}\}.
$$

For a broadband flat coupling $\kappa=\sqrt{\gamma/(2\pi)}$, define the envelope [annihilation operator](../../../quantum-mechanics.md#annihilation-operator) $b(t)=(2\pi)^{-1/2}\int b_\omega e^{-i(\omega-\omega_c)t}d\omega$. The [Markov approximation](../../../stochastic-process.md#markov-approximation-for-a-random-medium) extends the detuning integral over the full real line and gives $[b(t),b^\dagger(s)]=\delta(t-s)$. Then the [cavity-reservoir interaction](../../../control-theory.md#cavity-reservoir-interaction) is

$$
\boxed{H_I(t)=i\sqrt\gamma\{a(t)\otimes b^\dagger(t)-a^\dagger(t)\otimes b(t)\}.}
$$

The phases and normalization of the external field fix the sign convention. The [creation operators](../../../quantum-mechanics.md#creation-operator) and [annihilation operators](../../../quantum-mechanics.md#annihilation-operator) exchange one excitation between cavity and field, rather than creating or destroying a pair.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Under the [Markov approximation](../../../stochastic-process.md#markov-approximation-for-a-random-medium), a short incoming time bin is independent of the earlier input and commutes with adapted cavity operators. Write its [quantum noise increment](../../../control-theory.md#quantum-noise-increment) as $dB_{\mathrm{in}}(t)=\int_t^{t+dt}b(\tau)d\tau$; this is the increment denoted $B_{\mathrm{in}}(t)$ in the short-time definition, not an accumulated integral from zero.

During this bin, use the cavity operator at its left endpoint. Integrating the [cavity-reservoir interaction](../../../control-theory.md#cavity-reservoir-interaction) and applying $U=e^{-i\int H_I d\tau}$ yields the bin propagator

$$
\boxed{U_I(t+dt,t)=\exp\!\left[\sqrt\gamma\{a(t)\otimes dB_{\mathrm{in}}^\dagger(t)-a^\dagger(t)\otimes dB_{\mathrm{in}}(t)\}\right].}
$$

The exponent is anti-Hermitian, so the bin evolution is [unitary](../../../fiber-bundle.md#unitary-connection). This is the short-time stochastic form: the time-bin limit, or equivalently the time-ordered product of these adapted propagators, gives continuous evolution. The [quantum noise increments](../../../control-theory.md#quantum-noise-increment) scale as $\sqrt{dt}$; therefore one must retain the square of this exponent, rather than treating its integral as an ordinary order-$dt$ bounded Hamiltonian.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Put $K=\sqrt\gamma(a\otimes dB^\dagger-a^\dagger\otimes dB)$, with the time argument suppressed. Since the incoming field commutes with the adapted cavity operators,

$$
K^2=\gamma\{a^2\otimes(dB^\dagger)^2-aa^\dagger\otimes dB^\dagger dB-a^\dagger a\otimes dB\,dB^\dagger+(a^\dagger)^2\otimes(dB)^2\}.
$$

Applying the [Gaussian quantum noise Ito table](../../../control-theory.md#gaussian-quantum-noise-ito-table) gives

$$
K^2=-\gamma\,dt\,Q\otimes I_B,\qquad Q=Naa^\dagger+(N+1)a^\dagger a-M(a^\dagger)^2-M^*a^2.
$$

The [power series](../../../real-analysis.md#power-series) expansion $e^K=I+K+K^2/2+\cdots$ consequently becomes, through Ito order $dt$,

$$
\boxed{U_I=I+\sqrt\gamma(a\otimes dB^\dagger-a^\dagger\otimes dB)-\frac\gamma2Q\otimes I_B\,dt.}
$$

This has precisely the required quadratic drift correction. The short-time ordering is essential: the linear noise term is order $\sqrt{\gamma dt}$ and the drift is order $\gamma dt$; higher stochastic orders are discarded in the differential limit. A remainder written merely as a power of $\gamma$ is a formal coupling expansion, not a dimensionally complete statement of the short-time error.

As a sign check, $K^\dagger=-K$ and $Q^\dagger=Q$. Thus $U_I^\dagger U_I=I-\gamma Qdt-K^2=I$ through this order. The cross term is needed for stochastic [unitarity](../../../vector-space.md#unitary-operator).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

The Heisenberg update is $ds=U^\dagger sU-s$; the left side of the printed first update relation must be this increment, rather than $s(t)$ itself. For $s=a$, the linear noise term in the supplied stochastic equation is

$$
\sqrt\gamma[a^\dagger\otimes dB-a\otimes dB^\dagger,a]=-\sqrt\gamma\,dB,
$$

by the bosonic [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) $[a,a^\dagger]=I$.

The two thermal drift expressions simplify separately to

$$
2a^\dagger a a-aa^\dagger a-a^\dagger a a=-a,\qquad
2aaa^\dagger-aaa^\dagger-aa^\dagger a=a.
$$

The anomalous terms vanish because $[a^\dagger,[a^\dagger,a]]=0$ and $[a,[a,a]]=0$. Hence the factor inside the drift braces is $-(N+1)a+Na=-a$, independent of $N$ and $M$. Therefore

$$
\boxed{da=-\frac\gamma2a\,dt-\sqrt\gamma\,dB_{\mathrm{in}}.}
$$

Equivalently, in the formal white-noise notation of the [cavity-reservoir interaction](../../../control-theory.md#cavity-reservoir-interaction),

$$
\dot a(t)=-\frac\gamma2a(t)-\sqrt\gamma\,b_{\mathrm{in}}(t).
$$

The dot is a derivative notation for this stochastic differential equation, not a claim that the white-noise field is an ordinary differentiable function.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Take unilateral [Laplace transforms](../../../analysis.md#laplace-transform) of the cavity equation, keeping the initial operator:

$$
(s+\gamma/2)\widetilde a(s)=a(0)-\sqrt\gamma\,\widetilde b_{\mathrm{in}}(s).
$$

The input-output relation gives

$$
\widetilde b_{\mathrm{out}}(s)=\widetilde b_{\mathrm{in}}(s)+\sqrt\gamma\,\widetilde a(s)
=\frac{s-\gamma/2}{s+\gamma/2}\widetilde b_{\mathrm{in}}(s)+\frac{\sqrt\gamma\,a(0)}{s+\gamma/2}.
$$

A [transfer function](../../../control-theory.md#transfer-function) describes the forced zero-state part of the response. Thus the [passive cavity input-output transfer function](../../../control-theory.md#passive-cavity-input-output-transfer-function) is

$$
\boxed{G(s)=\frac{s-\gamma/2}{s+\gamma/2}.}
$$

The omitted initial-state term is a decaying transient $\sqrt\gamma e^{-\gamma t/2}a(0)$, and is present for a general initial cavity state. This distinction avoids silently setting a physical annihilation operator equal to zero.

<h3 id="5/f">f</h3>

↑ **Parent:** [5](#5)

<h4 id="5/f/solution">Solution</h4>

↑ **Parent:** [F](#5/f)

For a specified negative-feedback loop with return ratio $L(s)$, let $P$ be its number of open-right-half-plane poles. Let $N_{\mathrm{cw}}$ be the signed clockwise encirclement count of $-1$ by the standard [Nyquist stability criterion](../../../control-theory.md#nyquist-stability-criterion) contour. Provided the contour does not hit a singularity or the critical point, the number of right-half-plane closed-loop poles is $Z=P+N_{\mathrm{cw}}$. Thus **closed-loop stability requires $N_{\mathrm{cw}}=-P$ and no closed-loop pole on the imaginary axis**, with the usual well-posedness and absence of hidden unstable cancellations. For an already stable return ratio, there must be no encirclement of $-1$ and no passage through it.

The open cavity itself, for $\gamma>0$, has state eigenvalue and transfer-function pole $-\gamma/2$. Its initial transient decays and its impulse response is a direct-feedthrough term plus a decaying exponential. Hence **the open-loop cavity is asymptotically stable and its transfer function is BIBO stable**. The right-half-plane zero at $+\gamma/2$ does not make the open cavity unstable. On the frequency axis,

$$
G(i\omega)=\frac{\omega^2-(\gamma/2)^2+i\gamma\omega}{\omega^2+(\gamma/2)^2},\qquad |G(i\omega)|=1.
$$

Its unit-circle plot passes through $-1$ at $\omega=0$. A [Nyquist stability criterion](../../../control-theory.md#nyquist-stability-criterion) is a feedback criterion; this passage is not by itself a test of open-plant stability.

If the intended interpretation is a unit negative-feedback loop with $L=G$, then

$$
1+G(s)=\frac{2s}{s+\gamma/2},\qquad \frac{G(s)}{1+G(s)}=\frac{s-\gamma/2}{2s}.
$$

That loop has a pole at zero, so **unit negative feedback is marginal rather than asymptotically stable**, and the critical-point passage correctly prevents a strict Nyquist stability conclusion. Without a specified feedback interconnection, the unambiguous conclusion is the stable open cavity, not that particular closed loop.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
