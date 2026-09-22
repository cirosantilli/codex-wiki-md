<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an $n$-qubit [quantum code](../../../../../quantum-error-correcting-code.md) with projector $P$, the [quantum code distance](../../../../../distance-of-a-quantum-error-correcting-code.md) is

$$
\boxed{d=\min\{\operatorname{wt}(F):F\text{ is a Pauli operator and }PFP\notin\mathbb CP\}.}
$$

Here the weight counts nonidentity tensor factors. Thus every error supported on fewer than $d$ qubits is detectable, by the [Pauli expansion of a quantum error](../../../../../pauli-expansion-of-a-quantum-error.md). A scalar action on the code, including a nonidentity [stabilizer](../../../../../stabilizer-subgroup.md), is harmless and does not reduce this distance. For a [stabilizer code](../../../../../stabilizer-code.md), the equivalent definition minimizes weight among [Pauli operators](../../../../../pauli-operator.md) which commute with every [stabilizer generator](../../../../../stabilizer-generator.md) but act nontrivially on the logical information. The [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md) then guarantees correction of all errors of weight at most $t=\lfloor(d-1)/2\rfloor$, since each pairwise product has weight at most $2t<d$.

Suppose the code encodes $k$ logical [qubits](../../../../../qubit.md) and is nondegenerate for all errors through weight $t$. There are

$$
N_t=\sum_{j=0}^t3^j\binom nj
$$

distinct [Pauli errors](../../../../../pauli-operator.md) modulo phase: choose the $j$ affected positions and choose $X,Y$ or $Z$ at each. Each error is unitary, so its image of the code has dimension $2^k$. Nondegeneracy makes these images mutually orthogonal, equivalently the combined vectors $E_a|i_L\rangle$ are orthonormal. They all lie in the physical [Hilbert space](../../../../../hilbert-space-split.md) of dimension $2^n$. Counting dimensions proves the [quantum Hamming bound](../../../../../quantum-hamming-bound.md)

$$
\boxed{2^k\sum_{j=0}^t3^j\binom nj\leq2^n.}
$$

This dimension argument requires nondegeneracy. For a degenerate code, different errors can share an image, as in the [Shor code](../../../../../shor-code.md), and this counting proof cannot be applied unchanged.

For a binary classical code of $M$ words, the [Hamming bound](../../../../../hamming-bound.md) is $M\sum_{j=0}^t\binom nj\leq2^n$: disjoint [Hamming balls](../../../../../hamming-ball.md) around the words must fit into all binary strings. The quantum factor $3^j$ is needed because at each erroneous [qubit](../../../../../qubit.md) there are three linearly independent nonidentity [Pauli operators](../../../../../pauli-operator.md), not just a classical bit flip. A [phase flip](../../../../../pauli-z-gate.md) is invisible to a computational-basis classical record but changes a quantum superposition. A $Y$ error combines bit and phase effects, and the identity with $X,Y,Z$ spans every one-qubit operator. Quantum correction must protect amplitudes and coherences, and consequently count whole orthogonal logical subspaces rather than just classical words.

For parameters $[[5,1,3]]$, $t=1$, and

$$
2^1\left(1+3\binom51\right)=2\cdot16=32=2^5.
$$

Thus a nondegenerate such code saturates the bound: the sixteen two-dimensional error images exhaust the physical space. **It is a perfect quantum error-correcting code for single-qubit errors.** It also has the smallest possible length for nondegenerate single-error protection of one logical qubit: for $1\leq n\leq4$, the required inequality $1+3n\leq2^{n-1}$ fails.

Here is an explicit realization and its [five-qubit stabilizer syndrome table](../../../../../five-qubit-stabilizer-syndrome-table.md). Write tensor products without multiplication symbols and use

$$
g_1=XZZXI,\qquad g_2=IXZZX,\qquad g_3=XIXZZ,\qquad g_4=ZXIXZ.
$$

Each pair has an even number of anticommuting single-site factors, so the four [stabilizer generators](../../../../../stabilizer-generator.md) commute. Their binary Pauli labels are independent: no nonempty product has identity label. For example, the $X$-support at site three fixes the exponent of $g_3$ in such a product to zero, site five then fixes that of $g_2$, site one fixes that of $g_1$, and site two fixes that of $g_4$. Thus their group has sixteen elements and excludes $-I$. The common $+1$ eigenspace has projector $P=\prod_{a=1}^4(I+g_a)/16$ and dimension $\operatorname{Tr}P=32/16=2$, since all nonidentity Pauli strings have zero trace.

Record a syndrome bit as one when an error anticommutes with the corresponding generator, in order $g_1,g_2,g_3,g_4$. Direct local commutation gives

$$
\begin{array}{c|c|c|c}
\text{site}&X&Y&Z\\\hline
1&0001&1011&1010\\
2&1000&1101&0101\\
3&1100&1110&0010\\
4&0110&1111&1001\\
5&0011&0111&0100
\end{array}
$$

These are all fifteen nonzero four-bit [error syndromes](../../../../../error-syndrome.md); the identity has $0000$. Distinct errors in this list have a product with nonzero syndrome, so it anticommutes with some $g_a$. Inserting $g_aP=P$ on both sides gives $PE_b^\dagger E_cP=-PE_b^\dagger E_cP=0$. The diagonal product is the identity. Hence the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md) is exactly $C_{bc}=\delta_{bc}$, proving nondegenerate correction. Measure the four commuting checks, apply the unique indicated [Pauli error](../../../../../pauli-operator.md) again, and every logical state is recovered. The [Pauli expansion of a quantum error](../../../../../pauli-expansion-of-a-quantum-error.md) extends this recovery to an arbitrary one-qubit noise channel, not just the fifteen discrete errors.

The table also proves that every Pauli operator of weight one or two has nonzero syndrome: a weight-two operator is the product of distinct single-site errors, whose syndromes differ. Therefore the distance is at least three. The operators $\overline X=X^{\otimes5}$ and $\overline Z=Z^{\otimes5}$ commute with all four generators and anticommute with each other. They are nontrivial logical [Pauli operators](../../../../../pauli-operator.md). Multiplication of $\overline X$ by $g_1$ gives $-IYYIX$, a weight-three operator with the same logical action; it cannot be scalar on the code because it anticommutes with the invertible logical operator $\overline Z$. This proves $d=3$ exactly.

The code consequently detects every two-qubit error and corrects two known-location erasures by the [quantum erasure correction](../../../../../quantum-erasure-correction.md) criterion, but it cannot correct all two-qubit errors of unknown location. A nontrivial weight-three logical operator can be split into a weight-one and a weight-two error, whose pairwise product violates the correction condition. It also saturates the [quantum Singleton bound](../../../../../quantum-singleton-bound.md), since $n-k=4=2(d-1)$. These properties distinguish single-error perfectness from unrestricted protection against larger errors.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
