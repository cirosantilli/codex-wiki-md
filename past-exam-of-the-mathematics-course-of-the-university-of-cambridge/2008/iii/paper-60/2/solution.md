<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The physical space of $n$ [qubits](../../../../../qubit.md) is $\mathcal H_n=(\mathbb C^2)^{\otimes n}$. An error operator is a [linear operator](../../../../../linear-operator.md) on this space, for example one [Kraus operator](../../../../../kraus-operator.md) of a noise [quantum channel](../../../../../quantum-channel.md). The usual channel description assumes initially uncorrelated system and environment, with the environment subsequently ignored; more general initial correlations need not define a channel on arbitrary system inputs. Finite dimension and the tensor decomposition into identifiable qubits allow an exact [Pauli expansion of a quantum error](../../../../../pauli-expansion-of-a-quantum-error.md). No independence between errors on different qubits is assumed by this expansion.

The $4^n$ [tensor products](../../../../../tensor-product.md) of $I,X,Y,Z$ form an orthogonal basis of the operator space under the [Hilbert-Schmidt inner product](../../../../../hilbert-schmidt-inner-product.md). Equivalently, absorbing phases into coefficients, every error has an expansion

$$
E=\sum_{a,b\in\mathbb F_2^n}c_{a,b}X^aZ^b,
\qquad X^a=\bigotimes_{j=1}^nX^{a_j},\quad Z^b=\bigotimes_{j=1}^nZ^{b_j}.
$$

For a [computational basis](../../../../../computational-basis.md) vector $|x\rangle$ labelled by $x\in\mathbb F_2^n$, this gives

$$
\boxed{E|x\rangle=\sum_{a,b}c_{a,b}(-1)^{b\cdot x}|x+a\rangle,}
$$

where addition and the dot product in the exponent are modulo two. Thus $X$ changes a bit, $Z$ changes its phase, and $Y$ performs both up to a scalar phase. A general error is a coherent linear combination of such actions; it need not be a classical random choice of [Pauli operators](../../../../../pauli-operator.md). A restriction to at most $t$ faulty qubits is an additional locality assumption, expressed by the span of [Pauli operators](../../../../../pauli-operator.md) of weight at most $t$.

The [weight of a Pauli operator](../../../../../weight-of-a-pauli-operator.md) is the number of tensor factors different from $I$, ignoring global phase. Let $P$ be the [orthogonal projector](../../../../../orthogonal-projection.md) onto a $2^k$-dimensional code $\mathcal X$. [Quantum error detection](../../../../../quantum-error-detection.md) means

$$
PEP=c_EP.
$$

Indeed, a [projective measurement](../../../../../projective-measurement.md) of $P$ flags departure from the code, while its code-space outcome acts as the scalar $c_E$ on every encoded state and hence does not change logical information. Harmless scalar actions are included in this criterion. The [quantum code distance](../../../../../distance-of-a-quantum-error-correcting-code.md) is

$$
d=\min\{\operatorname{wt}(E):E\text{ is Pauli and }PEP\text{ is not scalar on }\mathcal X\}.
$$

Thus every [Pauli operator](../../../../../pauli-operator.md) of weight at most $d-1$ is detectable. The condition is linear in $E$, so it holds for any error in their span. This proves detection of arbitrary errors affecting at most $d-1$ qubits, including coherent errors.

For correction, put $t=\lfloor(d-1)/2\rfloor$ and take all phase-free [Pauli operators](../../../../../pauli-operator.md) $E_a$ of weight at most $t$. Their pairwise products satisfy

$$
\operatorname{wt}(E_a^\dagger E_b)\leq2t\leq d-1,
\qquad PE_a^\dagger E_bP=C_{ab}P.
$$

These are the [Knill--Laflamme conditions](../../../../../knill-laflamme-condition.md). Here is their recovery construction, rather than merely using the criterion's name. For any normalized code state $|\psi\rangle$, the matrix $C$ is a [Gram matrix](../../../../../gram-matrix.md), since $C_{ab}=\langle\psi|E_a^\dagger E_b|\psi\rangle$, and is therefore positive semidefinite. Choose linear combinations $F_j$ of the errors diagonalizing this matrix, so that

$$
PF_j^\dagger F_lP=c_j\delta_{jl}P,\qquad c_j\geq0.
$$

For $c_j>0$, the operators $V_j=F_jP/\sqrt{c_j}$ are isometries from the code into mutually orthogonal error-image subspaces: $V_j^\dagger V_l=\delta_{jl}P$. Measure the projectors $Q_j=V_jV_j^\dagger$ and, on outcome $j$, apply $V_j^\dagger$. Complete this recovery arbitrarily on the remaining orthogonal subspace to make a trace-preserving [quantum channel](../../../../../quantum-channel.md).

For an error $E=\sum_j\beta_jF_j$ and any encoded [density operator](../../../../../density-matrix.md) $\rho$, the recovered contribution is

$$
\sum_j V_j^\dagger E\rho E^\dagger V_j
=\left(\sum_j|\beta_j|^2c_j\right)\rho.
$$

Terms with $c_j=0$ annihilate the code. For a physical noise channel whose [Kraus operators](../../../../../kraus-operator.md) belong to this span, summing the displayed scalar over those operators gives one by trace preservation. The resulting recovered state is exactly $\rho$. This proves the [constructive recovery from the Knill-Laflamme condition](../../../../../constructive-recovery-from-the-knill-laflamme-condition.md) and the requested guarantee

$$
\boxed{[[n,k,d]]\text{ detects }d-1\text{ qubit errors and corrects }\left\lfloor\frac{d-1}{2}\right\rfloor.}
$$

This argument allows degenerate codes; distinct physical errors may have identical actions on the code.

For the [Shor code](../../../../../shor-code.md), define $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. Its two normalized basis codewords are

$$
\boxed{|0_L\rangle=|G_+\rangle^{\otimes3},\qquad |1_L\rangle=|G_-\rangle^{\otimes3}.}
$$

Six [stabilizer generators](../../../../../stabilizer-generator.md) are $Z_1Z_2,Z_2Z_3,Z_4Z_5,Z_5Z_6,Z_7Z_8,Z_8Z_9$; the two phase checks are

$$
g_7=X_1X_2X_3X_4X_5X_6,\qquad
g_8=X_4X_5X_6X_7X_8X_9.
$$

All eight have [eigenvalue](../../../../../eigenvalue.md) $+1$ on both basis codewords. A phase error $Z_4$ commutes with the six $Z$ checks and anticommutes with both $g_7$ and $g_8$. Their [projective measurements](../../../../../projective-measurement.md) therefore return

$$
\boxed{(+,+,+,+,+,+,-,-).}
$$

The two negative phase checks identify the middle three-qubit block. Apply the [Pauli Z gate](../../../../../pauli-z-gate.md) $Z_4$ to restore the state, since $Z_4^2=I$. This procedure acts identically on every logical superposition, and the checks reveal no logical amplitudes. The syndrome cannot distinguish $Z_4$ from $Z_5$ or $Z_6$, but all three have the same action on the code: their pairwise products lie in the [stabilizer group](../../../../../stabilizer-group.md). Correcting with any one of them is sufficient. Thus the degeneracy in the syndrome is harmless.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
