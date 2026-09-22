<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in four-dimensional [Minkowski spacetime](../../../../../minkowski-spacetime.md), with $\bar Q_{\dot\alpha A}=(Q_\alpha^A)^\dagger$ in a [unitary representation](../../../../../unitary-representation.md). The usual [Super-Poincaré algebra](../../../../../super-poincare-algebra.md) has the [Poincare algebra](../../../../../poincare-algebra.md) and possible internal [Lorentz scalars](../../../../../lorentz-scalar.md) as its even generators, and only the stated [Weyl spinors](../../../../../weyl-spinor.md) as its odd generators. This closure assumption is essential: [Lorentz covariance](../../../../../lorentz-covariance.md) alone would also permit additional tensor-valued generators. It is the setting selected by the [Haag–Łopuszański–Sohnius theorem](../../../../../haag-lopuszanski-sohnius-theorem.md) for ordinary interacting relativistic theories.

The [Spinor representation of the Lorentz group](../../../../../spinor-representation-of-the-lorentz-group.md) gives

$$
[Q_\alpha^A,M^{\mu\nu}]=(\sigma^{\mu\nu})_\alpha{}^\beta Q_\beta^A.
$$

Here $\sigma^{\mu\nu}$ denotes the [Lorentz algebra](../../../../../lorentz-algebra.md) matrices in the convention of the paper. Moving $M^{\mu\nu}$ to the left changes the sign; definitions using Hermitian [Lorentz algebra](../../../../../lorentz-algebra.md) generators may also put an explicit $i$ into these matrices. The conjugate relation acts on the dotted [Weyl spinor](../../../../../weyl-spinor.md) indices.

The [tensor product of group representations](../../../../../tensor-product-of-group-representations.md)

$$
(\tfrac12,0)\otimes(0,\tfrac12)=(\tfrac12,\tfrac12)
$$

is a [Lorentz four-vector](../../../../../four-vector.md). The only such even generator is $P_\mu$, so the mixed [anticommutator](../../../../../anticommutator.md) must be

$$
\{Q_\alpha^A,\bar Q_{\dot\beta B}\}=H^A{}_B\,\sigma^\mu_{\alpha\dot\beta}P_\mu.
$$

Applying [Hermitian conjugation](../../../../../hermitian-conjugation.md) makes $H$ a [Hermitian matrix](../../../../../hermitian-operator.md). Positivity of $\{S,S^\dagger\}$ for every [linear combination](../../../../../linear-combination.md) $S$ of [supercharges](../../../../../supersymmetry-generator.md) makes $H$ a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md) on a positive-energy physical [superalgebra representation](../../../../../lie-superalgebra-representation.md). Remove any null [supercharges](../../../../../supersymmetry-generator.md), which act trivially, and use a [unitary diagonalization of a normal matrix](../../../../../unitary-diagonalization-of-a-normal-matrix.md) followed by rescaling to obtain $H^A{}_B=2\delta^A{}_B$. Thus $\mathcal N$ counts the independent nontrivial [supercharges](../../../../../supersymmetry-generator.md).

For equal [chirality](../../../../../chirality-physics.md), the [tensor product of group representations](../../../../../tensor-product-of-group-representations.md) is

$$
(\tfrac12,0)\otimes(\tfrac12,0)=(0,0)\oplus(1,0).
$$

Consequently the tentative equal-[chirality](../../../../../chirality-physics.md) [anticommutator](../../../../../anticommutator.md) can contain $\epsilon_{\alpha\beta}Z^{AB}$ and a symmetric spinor tensor $T_{\alpha\beta}^{\mu\nu}M_{\mu\nu}Y^{AB}$, where $T$ is the [intertwining operator](../../../../../intertwining-operator.md) for [Lorentz covariance](../../../../../lorentz-covariance.md) onto $(1,0)$. Symmetry of the [anticommutator](../../../../../anticommutator.md) under $(A,\alpha)\leftrightarrow(B,\beta)$ forces $Z^{AB}=-Z^{BA}$ and $Y^{AB}=Y^{BA}$. At this stage $Z^{AB}$ is an internal [Lorentz scalar](../../../../../lorentz-scalar.md), hence commutes with $P_\mu$; its full centrality will follow below.

To determine the [commutator](../../../../../commutator.md) with translations, [Lorentz covariance](../../../../../lorentz-covariance.md) and the absence of additional odd generators leave only

$$
[P_\mu,Q_\alpha^A]=C^{AB}(\sigma_\mu)_{\alpha\dot\beta}\bar Q_B^{\dot\beta}
$$

and the relation obtained by [Hermitian conjugation](../../../../../hermitian-conjugation.md). The [graded Jacobi identity](../../../../../graded-jacobi-identity.md) for $(P_\mu,P_\nu,Q)$, using $[P_\mu,P_\nu]=0$, gives

$$
C\overline C\,\bigl(\sigma_\mu\bar\sigma_\nu-\sigma_\nu\bar\sigma_\mu\bigr)=0,
\qquad C\overline C=0,
$$

where $\overline C$ means entrywise [complex conjugation](../../../../../complex-conjugation.md). This equation alone would not imply $C=0$. Contract the [graded Jacobi identity](../../../../../graded-jacobi-identity.md)

$$
[P_\mu,\{Q_\alpha^A,Q_\beta^B\}]
=\{[P_\mu,Q_\alpha^A],Q_\beta^B\}+\{Q_\alpha^A,[P_\mu,Q_\beta^B]\}
$$

with $\epsilon^{\alpha\beta}$. The $M$ term drops out because its spinor tensor is symmetric, and $[P_\mu,Z^{AB}]=0$ makes the remaining left side vanish. Substitution of the mixed [anticommutator](../../../../../anticommutator.md) makes the right side a nonzero numerical multiple of $(C^{AB}-C^{BA})P_\mu$. Thus $C=C^T$. It follows that $\overline C=C^\dagger$ and $CC^\dagger=0$, whence $C=0$. Applying [Hermitian conjugation](../../../../../hermitian-conjugation.md) proves the same assertion for $\bar Q$:

$$
\boxed{[P_\mu,Q_\alpha^A]=[P_\mu,\bar Q_{\dot\alpha A}]=0.}
$$

Returning to the uncontracted [graded Jacobi identity](../../../../../graded-jacobi-identity.md) now gives $[P_\mu,\{Q_\alpha^A,Q_\beta^B\}]=0$. Since the [Lorentz algebra](../../../../../lorentz-algebra.md) generators do not commute with translations, the tentative $M$ term must have $Y^{AB}=0$. Hence

$$
\boxed{\{Q_\alpha^A,\bar Q_{\dot\beta B}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu\delta^A{}_B,
\qquad \{Q_\alpha^A,Q_\beta^B\}=\epsilon_{\alpha\beta}Z^{AB},
\qquad Z^{AB}=-Z^{BA}.}
$$

In particular $Z^{11}=0$ for $\mathcal N=1$. The dotted-dotted [anticommutator](../../../../../anticommutator.md) follows by [Hermitian conjugation](../../../../../hermitian-conjugation.md) applied to the second relation.

The [graded Jacobi identity](../../../../../graded-jacobi-identity.md) for $(Q^A,Q^B,\bar Q_C)$, together with $[P,Q]=0$, gives $[Z^{AB},\bar Q_C]=0$. As a [Lorentz scalar](../../../../../lorentz-scalar.md), $Z^{AB}$ commutes with $M_{\mu\nu}$, and it already commutes with $P_\mu$. Closure and [Lorentz covariance](../../../../../lorentz-covariance.md) make $[Z^{AB},Q_\alpha^C]=D^{AB,C}{}_D Q_\alpha^D$ for some coefficients. Apply the [graded Jacobi identity](../../../../../graded-jacobi-identity.md) once more:

$$
0=[Z^{AB},\{Q_\alpha^C,\bar Q_{\dot\beta E}\}]
=\{[Z^{AB},Q_\alpha^C],\bar Q_{\dot\beta E}\}
=2D^{AB,C}{}_E\sigma^\mu_{\alpha\dot\beta}P_\mu.
$$

Thus $D=0$. Since every $Z$ and $Z^\dagger$ is itself an [anticommutator](../../../../../anticommutator.md) of [supercharges](../../../../../supersymmetry-generator.md), the $Z$'s also commute with each other and their conjugates. Therefore **$Z^{AB}$ are [central charges in supersymmetry](../../../../../central-charge-in-supersymmetry.md) of the displayed algebra**. Additional [R-symmetry](../../../../../r-symmetry.md) automorphisms are not among the generators specified here.

For [boson-fermion degeneracy in a supermultiplet](../../../../../boson-fermion-degeneracy-in-a-supermultiplet.md), fix a physical [four-momentum](../../../../../four-momentum.md) $p$ with $p_0=E>0$, and take the finite internal space of states at that [four-momentum](../../../../../four-momentum.md). Let $\Gamma=(-1)^F$ be [fermion parity](../../../../../fermion-parity.md). It anticommutes with each [supercharge](../../../../../supersymmetry-generator.md) and its adjoint. For any fixed $A$, summing the diagonal spinor indices gives

$$
\sum_{\alpha=1}^2\{Q_\alpha^A,(Q_\alpha^A)^\dagger\}=4E\,\mathbf1,
$$

because $\sigma^0=\mathbf1$ and the [Pauli matrices](../../../../../pauli-matrices.md) are traceless. Cyclicity of the [operator trace](../../../../../operator-trace.md) and $\Gamma Q=-Q\Gamma$ imply

$$
\operatorname{Tr}(\Gamma QQ^\dagger)=-\operatorname{Tr}(\Gamma Q^\dagger Q).
$$

The [supertrace](../../../../../supertrace.md) of the preceding summed [anticommutator](../../../../../anticommutator.md) therefore vanishes:

$$
0=4E\operatorname{Tr}\Gamma=4E(n_B-n_F),
\qquad \boxed{n_B=n_F.}
$$

This counts physical [boson](../../../../../boson.md) and [fermion](../../../../../fermion.md) degrees of freedom, including polarizations. The phrase “any representation” needs a qualification: a one-dimensional even [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) with $P=Q=Z=0$ has one [boson](../../../../../boson.md) and no [fermion](../../../../../fermion.md). Thus the equality applies to positive-energy physical [supermultiplets](../../../../../supermultiplet.md) with finite state counts at fixed [four-momentum](../../../../../four-momentum.md), not to arbitrary abstract [superalgebra representations](../../../../../lie-superalgebra-representation.md) or unregulated infinite-dimensional [operator traces](../../../../../operator-trace.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
