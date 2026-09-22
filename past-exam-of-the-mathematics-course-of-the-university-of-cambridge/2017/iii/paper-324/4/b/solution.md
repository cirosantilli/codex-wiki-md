<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [logical depth of a measurement pattern](../../../../../../logical-depth-of-a-measurement-pattern.md) counts sequential layers of [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) forced by dependence of measurement bases on earlier outcomes. Depth one means every basis can be fixed before measurements start, allowing all [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) on distinct [qubits](../../../../../../qubit.md) to be performed in parallel. This does not require depth-one resource-state preparation or constant-depth classical parity processing.

Suppose the circuit contains $m$ gates $J(\alpha_1),\ldots,J(\alpha_m)$ in time order, with each $\alpha_j\in\{0,\pi/2\}$. Prepare an $(m+1)$-[vertex](../../../../../../vertex-graph-theory.md) path [graph state](../../../../../../graph-state.md) from $|+\rangle^{\otimes(m+1)}$ and [Controlled-Z gates](../../../../../../controlled-z-gate.md) between neighbours. Its first [qubit](../../../../../../qubit.md) supplies the specified input $|+\rangle$. Measure [vertex](../../../../../../vertex-graph-theory.md) $j-1$ in the fixed [equatorial qubit measurement](../../../../../../equatorial-qubit-measurement.md) basis at angle $\alpha_j$ for $j=1,\ldots,m$, obtaining $s_j$. Measure the final [vertex](../../../../../../vertex-graph-theory.md) in the [computational basis](../../../../../../computational-basis.md), obtaining $d$.

Track the [Pauli frame](../../../../../../pauli-frame.md) as $X^{a_j}Z^{b_j}$, starting with $a_0=b_0=0$. A hypothetical sequential reading of the same [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) gives the step $X^{s_j}J(\alpha_j)X^{a_{j-1}}Z^{b_{j-1}}$. The supplied commutation rules imply, up to [global phase](../../../../../../global-phase.md),

$$
X^{s_j}J(\alpha_j)X^aZ^b=X^{s_j\oplus b}Z^aJ((-1)^a\alpha_j).
$$

For $\alpha_j=0$, the sign is irrelevant. For $\alpha_j=\pi/2$, the identity $J(-\pi/2)=XJ(\pi/2)$ absorbs the possible sign change into the [Pauli frame](../../../../../../pauli-frame.md). If $t_j=0$ for $\alpha_j=0$ and $t_j=1$ for $\alpha_j=\pi/2$, the update is

$$
\boxed{a_j=s_j\oplus b_{j-1}\oplus t_ja_{j-1},\qquad b_j=a_{j-1},\qquad k=d\oplus a_m.}
$$

Inductively the final unmeasured [quantum state](../../../../../../quantum-state.md) would be $X^{a_m}Z^{b_m}J(\alpha_m)\cdots J(\alpha_1)|+\rangle$. The final [computational basis](../../../../../../computational-basis.md) outcome is corrected by $a_m$ and is unaffected by $b_m$. The induction on a sequential interpretation proves the joint statistics; projectors on distinct [vertices](../../../../../../vertex-graph-theory.md) commute, so the identical fixed-basis pattern can actually be measured simultaneously, including its final [vertex](../../../../../../vertex-graph-theory.md).

The first printed commutation formula has an incorrect exact scalar phase: with the printed matrix definition, $J(\alpha)X=e^{i\alpha}ZJ(-\alpha)$, rather than the negative-exponent prefactor. For example, at $\alpha=\pi/4$ the two versions differ by a factor $i$. They agree up to [global phase](../../../../../../global-phase.md), so this error does not affect the [Pauli frame](../../../../../../pauli-frame.md) recurrence or any [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) probability.

Consequently **a fixed-basis path-state pattern of logical depth one simulates every such circuit**. Only [Pauli measurements](../../../../../../measurement-of-a-pauli-observable.md) occur: the angle-zero basis measures $X$, and the angle-$\pi/2$ basis measures $-Y$ with the printed eigenvector labels. Classical [exclusive or](../../../../../../exclusive-or.md) processing suffices for all output corrections. These gates are [Clifford gates](../../../../../../clifford-gate.md), which explains why angle adaptation can be eliminated. For $m=0$, simply measure the initial $|+\rangle$ in the [computational basis](../../../../../../computational-basis.md); it is already a depth-one pattern.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
