<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Kronecker delta](../../../../../kronecker-delta.md) is the identity map on the defining representation. Its transformation is $A^\alpha{}_\gamma\delta^\gamma{}_\delta(A^{-1})^\delta{}_\beta=\delta^\alpha{}_\beta$. For the alternating [Levi-Civita symbol](../../../../../levi-civita-symbol.md), the determinant identity gives

$$
A^\alpha{}_aA^\beta{}_bA^\gamma{}_c\epsilon^{abc}=(\det A)\epsilon^{\alpha\beta\gamma}=\epsilon^{\alpha\beta\gamma}.
$$

The lower-index alternating [tensor](../../../../../tensor.md) transforms with three inverse [matrices](../../../../../matrix.md) and acquires $\det(A^{-1})=1$ instead. Thus **$\delta^\alpha{}_\beta$, $\epsilon^{\alpha\beta\gamma}$ and $\epsilon_{\alpha\beta\gamma}$ are invariant [tensors](../../../../../tensor.md)** of [SU(3)](../../../../../su-3-group.md). These identities use unimodularity; unitarity identifies the dual representation with the complex-conjugate defining representation.

For a [mixed SU(3) tensor representation](../../../../../mixed-su-3-tensor-representation.md) $T^a{}_b$, the [matrix trace](../../../../../matrix-trace.md) is invariant. Hence

$$
T^a{}_b=\frac13\delta^a{}_b\,T^c{}_c+Q^a{}_b,\qquad Q^a{}_a=0,
$$

gives

$$
\boxed{\mathbf3\otimes\overline{\mathbf3}=\mathbf1\oplus\mathbf8.}
$$

The trace is the singlet. The traceless [matrix](../../../../../matrix.md) transforms by conjugation, so it is the [adjoint representation of SU(3)](../../../../../adjoint-representation-of-su-3.md). It is irreducible: an invariant complex subspace is invariant under commutators with the complexified algebra $\mathfrak{sl}_3$, and would be an ideal in that simple [Lie algebra](../../../../../lie-algebra-split.md). Only the zero and full traceless-[matrix](../../../../../matrix.md) spaces are possible.

For the cubic [tensor](../../../../../tensor.md), define its symmetric and antisymmetric first-pair parts by

$$
T_+^{abc}=\frac12(T^{abc}+T^{bac}),\qquad
T_-^{abc}=\frac12(T^{abc}-T^{bac}),
$$

and let $S^{abc}=T^{(abc)}$ be its completely symmetric part. This has $\binom{5}{3}=10$ independent components and transforms as the [symmetric cubic representation of SU(3)](../../../../../symmetric-cubic-representation-of-su-3.md). Its irreducibility can be seen in the homogeneous cubic-polynomial realization: the simultaneous highest-weight conditions $z_1\partial_{z_2}P=0$ and $z_2\partial_{z_3}P=0$ leave only $P\propto z_1^3$. A finite-dimensional unitary representation is completely reducible, and each irreducible summand has a [highest-weight vector](../../../../../highest-weight-vector.md), so this single highest-weight line implies a single irreducible summand. Lowering generates all ten monomials.

Remove this fully symmetric part from $T_+$, putting $M^{abc}=T_+^{abc}-S^{abc}$. Define

$$
O^a{}_d=\epsilon_{dbc}M^{abc}.
$$

Its trace vanishes because $M$ is symmetric in its first two indices. Invariance of $\epsilon$ makes $O$ transform as one upper and one lower index. The inverse map is

$$
M^{abc}=\frac13\left(\epsilon^{bcd}O^a{}_d+\epsilon^{acd}O^b{}_d\right).
$$

Indeed contraction with $\epsilon_{ebc}$ gives $(2O^a{}_e+O^a{}_e-\delta^a{}_e\operatorname{tr}O)/3=O^a{}_e$. The inverse has the required first-pair symmetry and zero completely symmetric part. Thus this eight-dimensional remainder is another [adjoint representation of SU(3)](../../../../../adjoint-representation-of-su-3.md).

For the antisymmetric part, define

$$
N^c{}_d=\frac12\epsilon_{dab}T_-^{abc},\qquad
T_-^{abc}=\epsilon^{abd}N^c{}_d.
$$

Now decompose $N^c{}_d=U^c{}_d+\delta^c{}_d\operatorname{tr}N/3$, with $U$ traceless. The first term supplies a second independent octet; the trace supplies a singlet proportional to $\epsilon^{abc}$. With $q=\epsilon_{abc}T^{abc}/6=\operatorname{tr}N/3$, the [explicit cubic SU3 tensor projections](../../../../../explicit-cubic-su3-tensor-projections.md) reconstruct the entire [tensor](../../../../../tensor.md):

$$
T^{abc}=S^{abc}
+\frac13\left(\epsilon^{bcd}O^a{}_d+\epsilon^{acd}O^b{}_d\right)
+\epsilon^{abd}U^c{}_d+q\epsilon^{abc}.
$$

All projections commute with the [SU(3)](../../../../../su-3-group.md) action because they use permutations and [invariant tensors](../../../../../invariant-tensor.md). Their inverse maps and the dimension count $10+8+8+1=27$ establish

$$
\boxed{\mathbf3\otimes\mathbf3\otimes\mathbf3=\mathbf{10}\oplus\mathbf8\oplus\mathbf8\oplus\mathbf1.}
$$

The two octets are equivalent as group representations but distinct subspaces in this decomposition; one comes from the first-pair symmetric sector and the other from the first-pair antisymmetric sector. General permutations can mix these equivalent copies.

In the [quark model](../../../../../quark-model.md), the [up quark](../../../../../up-quark.md), [down quark](../../../../../down-quark.md) and [strange quark](../../../../../strange-quark.md) form the defining triplet of approximate [flavor symmetry](../../../../../flavor-symmetry.md). Three-quark [baryons](../../../../../baryon.md) therefore have precisely these possible flavor representations. The fully symmetric decuplet corresponds to the observed spin-$3/2$ [baryon decuplet](../../../../../baryon-decuplet.md): the four [Delta baryons](../../../../../delta-baryon.md), three $\Sigma^*$ states, two $\Xi^*$ states and the [Omega baryon](../../../../../omega-baryon.md). Their strangeness rows have [flavor hypercharge](../../../../../flavor-hypercharge.md) and [isospin](../../../../../isospin.md) $(Y,I)=(1,3/2),(0,1),(-1,1/2),(-2,0)$; $uuu$ and $sss$ occupy the extreme $\Delta^{++}$ and $\Omega^-$ weights.

The observed spin-$1/2$ [baryon octet](../../../../../baryon-octet.md) contains the [nucleons](../../../../../nucleon.md), three [Sigma baryons](../../../../../sigma-baryon.md), the [Lambda baryon](../../../../../lambda-baryon.md) and two [Xi baryons](../../../../../xi-baryon.md). In its $Y=0$ row, $\Sigma^0$ and $\Lambda$ share the same third-component/hypercharge weight but have different total [isospin](../../../../../isospin.md). Approximate flavor symmetry explains multiplet organization, not exact equality of all their masses: the strange-quark mass and electromagnetic interactions break it.

The two octet copies in the flavor [tensor](../../../../../tensor.md) do not require two identical ground-state octets. A [three-quark colour singlet](../../../../../three-quark-colour-singlet.md) is antisymmetric in color; for a symmetric ground-state orbital wavefunction, the [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md) requires a symmetric combined spin-flavor state. The mixed flavor octet [tensors](../../../../../tensor.md) combine with the mixed spin-$1/2$ [tensors](../../../../../tensor.md) to supply that symmetry. The symmetric flavor decuplet combines with symmetric spin $3/2$. Together they form the [symmetric spin-flavour SU6 representation](../../../../../symmetric-spin-flavour-su6-representation.md), with $10\times4+8\times2=56$ spin-flavor states. A completely antisymmetric flavor singlet cannot appear in this spatial ground state because three spin-$1/2$ indices have no fully antisymmetric spin state: $\bigwedge^3\mathbb C^2=0$. [Three-quark flavour singlet](../../../../../three-quark-flavour-singlet.md) configurations instead require a suitable excited spatial/spin symmetry. Flavor [SU(3)](../../../../../su-3-group.md) here is distinct from the exact color gauge symmetry; treating them as the same group action would misidentify the physical multiplets.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
