<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The $n$-qubit [Pauli group](../../../../../pauli-group.md) is

$$
G_n=\{i^rP_1\otimes\cdots\otimes P_n:r\in\{0,1,2,3\},\ P_j\in\{I,X,Y,Z\}\}.
$$

A [stabilizer group](../../../../../stabilizer-group.md) $S$ is an abelian subgroup of $G_n$ excluding $-I$. Its associated [stabilizer code](../../../../../stabilizer-code.md) is the common positive [eigenspace](../../../../../eigenspace.md)

$$
\boxed{\mathcal X_S=\{|\psi\rangle:s|\psi\rangle=|\psi\rangle\text{ for every }s\in S\}.}
$$

The exclusion of $-I$ is necessary for a nonzero code, since no nonzero vector has [eigenvalue](../../../../../eigenvalue.md) $+1$ under $-I$.

Every $s\in S$ is a signed Hermitian [tensor product](../../../../../tensor-product.md) of [Pauli matrices](../../../../../pauli-matrices.md). An imaginary-phase Pauli element would have $s^2=-I$, contradicting closure of $S$ and exclusion of $-I$; hence $s^2=I$ and $s^\dagger=s$. If $s\ne I$, it cannot be a nontrivial scalar Pauli element, and at least one of its local factors is $X,Y$ or $Z$. Each of these has trace zero. Using $\operatorname{Tr}(A\otimes B)=\operatorname{Tr}(A)\operatorname{Tr}(B)$ gives $\operatorname{Tr}s=0$.

The [spectral theorem](../../../../../spectral-theorem.md) for Hermitian operators and $s^2=I$ show that all [eigenvalues](../../../../../eigenvalue.md) are $+1$ or $-1$. If their multiplicities are $m_+$ and $m_-$, then

$$
m_++m_-=2^n,\qquad m_+-m_-=\operatorname{Tr}s=0.
$$

Thus the [balanced spectrum of a nonidentity stabilizer](../../../../../balanced-spectrum-of-a-nonidentity-stabilizer.md) is

$$
\boxed{m_+=m_-=2^{n-1}.}
$$

This concerns a nonidentity stabilizer acting on the entire physical space; on the code every stabilizer acts with [eigenvalue](../../../../../eigenvalue.md) $+1$.

Because all elements commute and square to $I$, $S$ is a [vector space](../../../../../vector-space-split.md) over $\mathbb F_2$ under multiplication. Its independent [stabilizer generators](../../../../../stabilizer-generator.md) $g_1,\ldots,g_r$ satisfy that no nonempty product is $I$; all $2^r$ products are distinct. The [stabilizer-projector formula](../../../../../stabilizer-projector-formula.md) is

$$
P_S=\frac1{|S|}\sum_{s\in S}s=\prod_{j=1}^r\frac{I+g_j}{2}.
$$

To verify it, group multiplication gives $P_S^2=P_S$, Hermiticity gives $P_S^\dagger=P_S$, and $sP_S=P_S$ for every $s\in S$. Conversely every code vector is fixed by this average, so its range is exactly $\mathcal X_S$. All nonidentity stabilizers have trace zero by the preceding proof. Therefore

$$
\dim\mathcal X_S=\operatorname{Tr}P_S=\frac{2^n}{|S|}=2^{n-r}.
$$

For a code of dimension $2^k$, the number of independent generators is consequently $\boxed{r=n-k}$. One can list additional redundant generators, but an independent generating set has exactly this size.

For a correctable Pauli error $E_\alpha$, define the syndrome bit $s_j(\alpha)$ to be zero when $E_\alpha$ commutes with $g_j$ and one when it anticommutes. On an encoded state,

$$
g_jE_\alpha|\psi\rangle=(-1)^{s_j(\alpha)}E_\alpha|\psi\rangle.
$$

Measure the commuting [stabilizer generators](../../../../../stabilizer-generator.md); their [eigenvalues](../../../../../eigenvalue.md) reveal the [error syndrome](../../../../../error-syndrome.md) without revealing logical amplitudes. In a [nondegenerate quantum code](../../../../../nondegenerate-quantum-error-correcting-code.md), the distinct specified correctable errors have orthogonal images of the code and distinct syndromes. A syndrome therefore identifies the error representative, and applying the inverse [Pauli operator](../../../../../pauli-operator.md) $E_\alpha^\dagger$ restores the encoded state.

If an actual error operator is a coherent linear combination of the specified errors, its state is a sum of these orthogonal syndrome components. Syndrome measurement selects one component, followed by the same inverse operation. The [linearity of coherent quantum error correction](../../../../../linearity-of-coherent-quantum-error-correction.md) ensures the logical state is recovered in every outcome. The same procedure handles noise [Kraus operators](../../../../../kraus-operator.md) in that error span; it does not require a probabilistic Pauli-noise assumption.

A Pauli error commuting with every stabilizer has the all-zero syndrome and preserves the code space. If it is a stabilizer up to global phase, this silent action is harmless. If it lies in the [centralizer of a stabilizer group](../../../../../centralizer-of-a-stabilizer-group.md) but is not a stabilizer up to phase, it acts as a nontrivial logical operator, and syndrome measurements cannot detect it. More generally, a non-scalar component $P_SEP_S$ of an error is an undetectable logical action. This distinguishes harmful undetected errors from scalar actions that satisfy [quantum error detection](../../../../../quantum-error-detection.md) algebraically.

The three-qubit [bit-flip repetition code](../../../../../bit-flip-repetition-code.md) has basis $|000\rangle,|111\rangle$ and generators

$$
\boxed{g_1=Z_1Z_2,\qquad g_2=Z_2Z_3.}
$$

A single phase flip $Z_1$ commutes with both and has zero syndrome, but

$$
Z_1(\alpha|000\rangle+\beta|111\rangle)
=\alpha|000\rangle-\beta|111\rangle.
$$

It is a nontrivial logical phase operation. In particular, $P_SZ_1P_S$ is not scalar, so the error set $\{I,Z_1\}$ violates the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md) and cannot be corrected. Thus **the code corrects single bit flips but not single phase flips**; its distance against arbitrary quantum errors is one.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
