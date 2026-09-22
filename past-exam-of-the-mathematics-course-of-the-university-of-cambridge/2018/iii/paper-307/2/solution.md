<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use a positive-energy [unitary representation](../../../../../unitary-representation.md) with finite [helicity](../../../../../helicity.md) states, excluding [continuous-spin representations](../../../../../continuous-spin-representation.md). In the specified frame the [Pauli matrices](../../../../../pauli-matrices.md) give

$$
2\sigma^\mu p_\mu=2E(\mathbf1+\sigma^3)
=4E\begin{pmatrix}1&0\\0&0\end{pmatrix}.
$$

For every $A$ and every state $|\chi\rangle$,

$$
0=\langle\chi|\{Q_2^A,(Q_2^A)^\dagger\}|\chi\rangle
=\|Q_2^A|\chi\rangle\|^2+\|(Q_2^A)^\dagger|\chi\rangle\|^2.
$$

Positivity therefore gives $Q_2^A=\bar Q_{\dot2 A}=0$ on this [massless supermultiplet](../../../../../massless-supermultiplet.md). The equal-[chirality](../../../../../chirality-physics.md) [anticommutator](../../../../../anticommutator.md) $\{Q_1^A,Q_2^B\}=\epsilon_{12}Z^{AB}$ then shows that every [central charge in supersymmetry](../../../../../central-charge-in-supersymmetry.md) vanishes on this [superalgebra representation](../../../../../lie-superalgebra-representation.md).

Normalize the remaining [supercharges](../../../../../supersymmetry-generator.md) as [fermionic raising and lowering operators](../../../../../fermionic-raising-and-lowering-operator.md):

$$
a_A=\frac{Q_1^A}{\sqrt{4E}},\qquad a_A^\dagger=\frac{\bar Q_{\dot1 A}}{\sqrt{4E}}.
$$

They obey the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md)

$$
\{a_A,a_B^\dagger\}=\delta_{AB},\qquad
\{a_A,a_B\}=\{a_A^\dagger,a_B^\dagger\}=0.
$$

Choose a [Clifford vacuum](../../../../../clifford-vacuum.md) $|\lambda\rangle$ of [helicity](../../../../../helicity.md) $\lambda\in\tfrac12\mathbb Z$ annihilated by every $a_A$. Such a vector exists because the commuting [fermion number operators](../../../../../fermion-number-operator.md) $a_A^\dagger a_A$ have eigenvalues $0$ and $1$, and lowering every occupied mode produces a nonzero empty state. In an [irreducible representation](../../../../../irreducible-representation.md) this empty space has dimension one; multiple empty states produce a [direct sum](../../../../../direct-sum.md) of copies. The states are

$$
|A_1\cdots A_k;\lambda\rangle
=a_{A_1}^\dagger\cdots a_{A_k}^\dagger|\lambda\rangle,
\qquad 1\leq A_1<\cdots<A_k\leq\mathcal N,
\qquad 0\leq k\leq\mathcal N.
$$

The [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md) make these states orthonormal for a normalized [Clifford vacuum](../../../../../clifford-vacuum.md). In the [helicity](../../../../../helicity.md) convention $[J_3,Q_1^A]=\tfrac12Q_1^A$, its adjoint has $[J_3,a_A^\dagger]=-\tfrac12a_A^\dagger$. Thus the [Clifford vacuum](../../../../../clifford-vacuum.md) is the highest-[helicity](../../../../../helicity.md) state and

$$
\boxed{h_k=\lambda-\frac{k}{2},\qquad d(h_k)=\binom{\mathcal N}{k}.}
$$

Reversing the rotation convention reverses the displayed ordering and leaves all counts unchanged. The level-$k$ states form the [exterior power](../../../../../exterior-power.md) $\Lambda^k\mathbb C^{\mathcal N}$, which explains the [binomial coefficient](../../../../../binomial-coefficient.md). Summing the [binomial coefficients](../../../../../binomial-coefficient.md) gives the [helicity spectrum of a massless supermultiplet](../../../../../helicity-spectrum-of-a-massless-supermultiplet.md):

$$
\boxed{\dim\mathcal H_p=\sum_{k=0}^{\mathcal N}\binom{\mathcal N}{k}=2^{\mathcal N},
\qquad h_{\max}-h_{\min}=\frac{\mathcal N}{2}.}
$$

Each application of a [fermionic raising and lowering operator](../../../../../fermionic-raising-and-lowering-operator.md) reverses [fermion parity](../../../../../fermion-parity.md). The even and odd levels each contain $2^{\mathcal N-1}$ states, so a physical [massless supermultiplet](../../../../../massless-supermultiplet.md) has $2^{\mathcal N-1}$ [boson](../../../../../boson.md) and $2^{\mathcal N-1}$ [fermion](../../../../../fermion.md) states.

These formulas describe one [irreducible representation](../../../../../irreducible-representation.md) of the massless [Super-Poincaré algebra](../../../../../super-poincare-algebra.md) at fixed [four-momentum](../../../../../four-momentum.md). A reducible [superalgebra representation](../../../../../lie-superalgebra-representation.md) can contain several such [supermultiplets](../../../../../supermultiplet.md). Also, the [CPT theorem](../../../../../cpt-theorem.md) sends [helicity](../../../../../helicity.md) $h$ to $-h$ and conjugates internal charges. [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md) may therefore require a second $2^{\mathcal N}$-state [supermultiplet](../../../../../supermultiplet.md), with highest [helicity](../../../../../helicity.md) $\mathcal N/2-\lambda$. A necessary condition for the original [helicity spectrum of a massless supermultiplet](../../../../../helicity-spectrum-of-a-massless-supermultiplet.md) to be self-conjugate is $\lambda=\mathcal N/4$; internal charges must also admit the conjugation in a realization compatible with the [Spin-statistics theorem](../../../../../spin-statistics-theorem.md). Thus this [helicity](../../../../../helicity.md) condition alone is not sufficient for [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md) without doubling. In particular, the original irreducible count is not automatically the count after [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md).

For the conventional bounds on [extended supersymmetry](../../../../../extended-supersymmetry.md), suppose all massless states satisfy $|h|\leq s_{\max}$. The [helicity spectrum of a massless supermultiplet](../../../../../helicity-spectrum-of-a-massless-supermultiplet.md) occupies an interval of width $\mathcal N/2$, whereas the available interval has width $2s_{\max}$. Hence

$$
\boxed{\mathcal N\leq4s_{\max}.}
$$

An ordinary four-dimensional [renormalizable quantum field theory](../../../../../renormalizable-quantum-field-theory.md) without gravity uses interacting massless fields of [spin angular momentum](../../../../../spin.md) at most one. Massless [spin angular momentum](../../../../../spin.md) $3/2$ requires [supergravity](../../../../../supergravity.md), whose gravitational coupling has negative [mass dimension](../../../../../mass-dimension.md) and is a [nonrenormalizable interaction](../../../../../nonrenormalizable-interaction.md) by [power counting in quantum field theory](../../../../../power-counting-in-quantum-field-theory.md). Setting $s_{\max}=1$ gives **$\mathcal N\leq4$ for conventional renormalizable theories**. The bound is attained by [four-dimensional N=4 super Yang-Mills theory](../../../../../four-dimensional-n-4-super-yang-mills-theory.md): choosing $\lambda=1$ gives

$$
\begin{array}{c|ccccc}
h&1&\tfrac12&0&-\tfrac12&-1\\\hline
d(h)&1&4&6&4&1
\end{array}
$$

for its [supersymmetric vector multiplet](../../../../../supersymmetric-vector-multiplet.md).

Allowing gravity permits $s_{\max}=2$, so **$\mathcal N\leq8$ for conventional theories including gravity**. The [four-dimensional N=8 supergravity](../../../../../four-dimensional-n-8-supergravity.md) [supergravity multiplet](../../../../../supergravity-multiplet.md) attains the bound with $\lambda=2$:

$$
\begin{array}{c|ccccccccc}
h&2&\tfrac32&1&\tfrac12&0&-\tfrac12&-1&-\tfrac32&-2\\\hline
d(h)&1&8&28&56&70&56&28&8&1
\end{array}
$$

It has $256$ states, $128$ [boson](../../../../../boson.md) and $128$ [fermion](../../../../../fermion.md) states. The conventional claim about a maximum “in general” assumes local interacting four-dimensional theories in [Minkowski spacetime](../../../../../minkowski-spacetime.md) with a finite spectrum of fields and no massless [spin angular momentum](../../../../../spin.md) above two. It is not a theorem excluding arbitrary free higher-[spin angular momentum](../../../../../spin.md) constructions or all theories in other spacetime settings.

Finally, a [chiral gauge spectrum](../../../../../chiral-gauge-spectrum.md) means that the independent left-handed [Weyl spinors](../../../../../weyl-spinor.md) occur in complex [gauge group representations](../../../../../gauge-group-representation.md) without obligatorily paired conjugate left-handed [Weyl spinors](../../../../../weyl-spinor.md). In [four-dimensional N=1 supersymmetry](../../../../../four-dimensional-n-1-supersymmetry.md), an irreducible matter [supermultiplet](../../../../../supermultiplet.md) with [helicities](../../../../../helicity.md) $(0,-\tfrac12)$ can carry a complex [gauge group representation](../../../../../gauge-group-representation.md) $R$. Its [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md) supplies the right-handed [antiparticle](../../../../../antiparticle.md) in $\bar R$, as every left-handed [Weyl spinor](../../../../../weyl-spinor.md) requires; it does not supply a second independent left-handed [Weyl spinor](../../../../../weyl-spinor.md) in $\bar R$. Consequently a [chiral gauge spectrum](../../../../../chiral-gauge-spectrum.md) is possible.

For $\mathcal N=2$, the matter [hypermultiplet](../../../../../hypermultiplet.md) has [helicities](../../../../../helicity.md) $(\tfrac12,0,0,-\tfrac12)$ before internal [charge conjugation](../../../../../charge-conjugation.md). If it carries a complex [gauge group representation](../../../../../gauge-group-representation.md) $R$, its [CPT completion of a supermultiplet](../../../../../cpt-completion-of-a-supermultiplet.md) adds the conjugate [hypermultiplet](../../../../../hypermultiplet.md). Equivalently, the resulting full [hypermultiplet](../../../../../hypermultiplet.md) contains two $\mathcal N=1$ [chiral superfields](../../../../../chiral-superfield.md), one in $R$ and one in $\bar R$. These give a [vectorlike gauge spectrum](../../../../../vectorlike-gauge-spectrum.md). Half-[hypermultiplets](../../../../../hypermultiplet.md) can occur in [pseudoreal representations](../../../../../pseudoreal-representation.md), which also do not produce genuinely complex [chiral gauge spectra](../../../../../chiral-gauge-spectrum.md). A [supersymmetric vector multiplet](../../../../../supersymmetric-vector-multiplet.md) has [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), hence real gauge [quantum numbers](../../../../../quantum-number.md). Since every $\mathcal N\geq2$ algebra contains an $\mathcal N=2$ subalgebra, the same obstruction applies to greater [extended supersymmetry](../../../../../extended-supersymmetry.md).

Therefore **a conventional chiral gauge spectrum is possible only for $\mathcal N=0$ or $\mathcal N=1$**. Here $\mathcal N=0$ means no [supersymmetry](../../../../../supersymmetry-split.md); among theories with actual [supersymmetry](../../../../../supersymmetry-split.md), only $\mathcal N=1$ qualifies. These are necessary structural conditions, not a guarantee that a chosen [chiral gauge spectrum](../../../../../chiral-gauge-spectrum.md) satisfies [anomaly cancellation](../../../../../anomaly-cancellation.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
