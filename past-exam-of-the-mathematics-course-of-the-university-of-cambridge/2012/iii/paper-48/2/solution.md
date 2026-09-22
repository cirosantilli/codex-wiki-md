<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the full definition of the [special unitary group](../../../../../special-unitary-group.md): $A^\dagger A=I$ and $\det A=1$. The [determinant](../../../../../determinant.md) condition is essential for the alternating [tensors](../../../../../tensor.md); unitarity alone would instead define $U(n)$. Assume $n\geq2$ when discussing proper [invariant subspaces](../../../../../invariant-subspace.md).

Let $V=\mathbb C^n$ be the [fundamental representation](../../../../../fundamental-representation.md). A $(j,k)$ [tensor](../../../../../tensor.md) belongs to $V^{\otimes j}\otimes(V^*)^{\otimes k}$. Its [SU(n) tensor transformation](../../../../../su-n-tensor-transformation.md) is

$$
\boxed{T'{}^{\alpha_1\cdots\alpha_j}_{\beta_1\cdots\beta_k}
=A^{\alpha_1}{}_{\gamma_1}\cdots A^{\alpha_j}{}_{\gamma_j}
(A^{-1})^{\delta_1}{}_{\beta_1}\cdots(A^{-1})^{\delta_k}{}_{\beta_k}
T^{\gamma_1\cdots\gamma_j}_{\delta_1\cdots\delta_k}.}
$$

Since $(A^{-1})^\delta{}_{\beta}=\overline{A^\beta{}_{\delta}}$, [complex conjugation](../../../../../complex-conjugation.md) exchanges upper fundamental and lower dual factors. Reordering the two index groups shows that $\overline T$ is a $(k,j)$ [tensor](../../../../../tensor.md).

The [invariant tensors](../../../../../invariant-tensor.md) follow directly. The [Kronecker delta](../../../../../kronecker-delta.md) transforms to $A^\alpha{}_{\gamma}(A^{-1})^\gamma{}_{\beta}=\delta^\alpha{}_{\beta}$. For the alternating [tensors](../../../../../tensor.md), the [determinant](../../../../../determinant.md) expansion gives

$$
A^{\alpha_1}{}_{\gamma_1}\cdots A^{\alpha_n}{}_{\gamma_n}\epsilon^{\gamma_1\cdots\gamma_n}
=(\det A)\epsilon^{\alpha_1\cdots\alpha_n}=\epsilon^{\alpha_1\cdots\alpha_n}.
$$

The lower [tensor](../../../../../tensor.md) is preserved in the same way using $\det A^{-1}=1$. Thus **$\delta$, $\epsilon^{\alpha_1\cdots\alpha_n}$ and $\epsilon_{\beta_1\cdots\beta_n}$ are invariant.**

When $j\geq2$, the permutation of two upper slots commutes with the [tensor product representation](../../../../../tensor-product-of-group-representations.md). Its $+1$ and $-1$ [eigenspaces](../../../../../eigenspace.md) are nonzero proper [invariant subspaces](../../../../../invariant-subspace.md). The same argument uses two lower slots when $k\geq2$. The remaining rank-two case $(j,k)=(1,1)$ splits into scalar multiples of $\delta$ and [traceless second-rank tensors](../../../../../traceless-second-rank-tensor.md), since [tensor contraction](../../../../../tensor-contraction.md) is equivariant. This covers every case except the fundamental, dual fundamental and scalar cases specified in the question. Those three are irreducible: the [special unitary group](../../../../../special-unitary-group.md) acts transitively on unit vectors in its fundamental space, so a nonzero [invariant subspace](../../../../../invariant-subspace.md) must be the full space, and the dual has the same property.

A [symmetric tensor](../../../../../symmetric-tensor.md) of upper rank $j$ has one component for each multiplicity vector $(r_1,\ldots,r_n)$ with nonnegative entries and $\sum r_i=j$. Equivalently it is a homogeneous degree-$j$ polynomial in $n$ variables. Counting these monomials gives

$$
\boxed{\dim\operatorname{Sym}^jV=\binom{n+j-1}{j}=\frac{(n+j-1)!}{j!(n-1)!}.}
$$

For a [totally antisymmetric tensor](../../../../../totally-antisymmetric-tensor.md), any repeated index gives zero and the remaining components are indexed by increasing $j$-element subsets. Hence

$$
\boxed{\dim\bigwedge^jV=\binom nj\quad(0\leq j\leq n),\qquad \dim\bigwedge^jV=0\quad(j>n).}
$$

These are the dimensions of the [symmetric power](../../../../../symmetric-power.md) and [exterior power](../../../../../exterior-power.md), respectively.

For [SU(4)](../../../../../su-4-group.md), the [two-index antisymmetric representation](../../../../../two-index-antisymmetric-representation.md) has complex dimension six. To establish a six-dimensional [real representation](../../../../../real-representation.md), one must exhibit a real structure; simply counting six complex components would give twelve real components. Normalize $\epsilon^{1234}=1$ and define the [antilinear map](../../../../../antilinear-map.md)

$$
(\mathcal JT)^{ab}=\frac12\epsilon^{abcd}\overline{T^{cd}}.
$$

The invariant Hermitian form identifies the conjugate indices with lower indices, and the invariant volume [tensor](../../../../../tensor.md) then returns an upper pair. Thus $\mathcal J$ commutes with [SU(4)](../../../../../su-4-group.md). The identity

$$
\epsilon^{abcd}\epsilon_{cdef}=2(\delta^a_e\delta^b_f-\delta^a_f\delta^b_e)
$$

gives $\mathcal J^2=1$. Its fixed space has

$$
T^{12}=\overline{T^{34}},\qquad T^{13}=-\overline{T^{24}},\qquad T^{14}=\overline{T^{23}}.
$$

Three arbitrary complex entries specify all the others, giving exactly six real degrees of freedom. The [real structure of the SU4 exterior square](../../../../../real-structure-of-the-su4-exterior-square.md) therefore proves

$$
\boxed{\bigwedge^2\mathbb C^4\text{ is the complexification of a real six-dimensional representation}.}
$$

The ordinary Hermitian [norm](../../../../../norm.md) restricts to an invariant positive real [inner product](../../../../../inner-product.md) on this fixed space.

[Irreducible representations](../../../../../irreducible-representation.md) classify states because an exact symmetry commutes with the [Hamiltonian](../../../../../hamiltonian.md), preserving energy [eigenspaces](../../../../../eigenspace.md). Irreducible multiplets are the smallest sets closed under all symmetry transformations; their labels and [Casimir operators](../../../../../casimir-element.md) provide quantum numbers. Approximate [flavour symmetry](../../../../../flavor-symmetry.md) gives approximate multiplets and mass relations, with splittings caused by its breaking. Spin and internal quantum numbers are distinct labels.

For the light-quark [flavour symmetry](../../../../../flavor-symmetry.md) in [Quantum chromodynamics](../../../../../quantum-chromodynamics.md), the quark flavours form $\mathbf3$. Their [Triple tensor decomposition for the defining sl3 representation](../../../../../triple-tensor-decomposition-for-the-defining-sl3-representation.md) is

$$
\mathbf3^{\otimes3}=\mathbf{10}_{\rm sym}\oplus\mathbf8_{\rm mixed}\oplus\mathbf8_{\rm mixed}\oplus\mathbf1_{\rm antisym}.
$$

This algebraic decomposition alone does not determine the allowed ground-state [baryons](../../../../../baryon.md). The [three-quark colour singlet](../../../../../three-quark-colour-singlet.md) is antisymmetric. The no-orbital-excitation ground state has a symmetric spatial wavefunction, so the [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md) requires the combined spin-flavour wavefunction to be symmetric. The three spin-one-half factors have

$$
\mathbf2^{\otimes3}=\mathbf4_{\rm sym}\oplus\mathbf2_{\rm mixed}\oplus\mathbf2_{\rm mixed},\qquad \bigwedge^3\mathbb C^2=0.
$$

Here the four-dimensional spin representation has spin $3/2$, while each doublet has spin $1/2$. Symmetric decuplet flavour pairs with symmetric spin $3/2$. The two flavour-octet copies and two spin-doublet copies carry the two-dimensional standard permutation multiplicity space; its [tensor square](../../../../../tensor-square.md) contains one symmetric singlet. Their invariant pairing therefore supplies one octet with spin $1/2$, not two independent ground-state octets. Antisymmetric flavour would need a completely antisymmetric three-quark spin state, which does not exist.

Equivalently the [symmetric spin-flavour SU6 representation](../../../../../symmetric-spin-flavour-su6-representation.md) has

$$
\operatorname{Sym}^3(\mathbb C^3\otimes\mathbb C^2)
=(\mathbf{10},\mathbf4)\oplus(\mathbf8,\mathbf2),\qquad 56=40+16.
$$

Thus the [Pauli constraint on three-quark flavour multiplets](../../../../../pauli-constraint-on-three-quark-flavour-multiplets.md) gives the concise spectrum classification

$$
\boxed{\mathbf8\text{ with }J^P=\tfrac12^+,\qquad \mathbf{10}\text{ with }J^P=\tfrac32^+.}
$$

These are the [baryon octet](../../../../../baryon-octet.md) and [baryon decuplet](../../../../../baryon-decuplet.md). The [three-quark flavour singlet](../../../../../three-quark-flavour-singlet.md) requires a different spatial permutation symmetry and belongs to excited states, outside the symmetric ground-state approximation used here. If low-lying spatially excited states are also included while their orbital labels are merely suppressed, singlets can occur; the full flavour tensor cube has types $\mathbf1,\mathbf8,\mathbf{10}$. The absence of the singlet from the unexcited ground multiplet is a permutation-symmetry constraint, not a prohibition by $SU(3)$ alone. Light-quark mass differences make the [flavour symmetry](../../../../../flavor-symmetry.md) approximate rather than exact.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
