<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

We prove the [one-query constancy obstruction for phase oracles](../../../../../one-query-constancy-obstruction-for-phase-oracles.md) while allowing arbitrary [quantum ancillas](../../../../../quantum-ancilla.md). By [purification of a density operator](../../../../../purification-of-a-density-operator.md), the [quantum state](../../../../../quantum-state.md) immediately before the sole query can be taken as

$$
|\Psi\rangle=\sum_{x=0}^{M-1}|x\rangle|a_x\rangle,
\qquad p_x=\langle a_x|a_x\rangle,
\qquad\sum_xp_x=1.
$$

The [ancilla](../../../../../quantum-ancilla.md) vectors need not be normalized or [orthogonal](../../../../../orthogonal-vectors.md). Classical randomness and earlier [quantum measurements](../../../../../quantum-measurement-split.md) can be included in additional [ancillas](../../../../../quantum-ancilla.md); allowing access to these systems only gives the proposed algorithm more power.

For the zero [constant function](../../../../../constant-function.md), the [phase oracle](../../../../../phase-oracle.md) is $I$, leaving $|\Psi\rangle$ unchanged. For each $j$, consider the [Boolean function](../../../../../boolean-function.md) that is one at $j$ and zero elsewhere. Since $M>2$, it is nonconstant, and its [phase oracle](../../../../../phase-oracle.md) produces

$$
|\Psi_j\rangle=|\Psi\rangle-2|j\rangle|a_j\rangle,
\qquad\langle\Psi|\Psi_j\rangle=1-2p_j.
$$

Any later fixed [unitary transformation](../../../../../unitary-operator.md) preserves these [inner products](../../../../../inner-product-split.md). An arbitrary final [quantum measurement](../../../../../quantum-measurement-split.md) cannot distinguish the constant output from each nonconstant output with certainty unless they are [orthogonal](../../../../../orthogonal-vectors.md), by [perfect discrimination of pure states requires orthogonality](../../../../../perfect-discrimination-of-pure-states-requires-orthogonality.md). Explicitly, an accepting [POVM](../../../../../positive-operator-valued-measure.md) effect $E$ would satisfy $E|\Psi\rangle=|\Psi\rangle$ and $E|\Psi_j\rangle=0$, forcing $\langle\Psi|\Psi_j\rangle=0$.

Therefore exact classification requires $p_j=1/2$ for every $j$. Summing gives

$$
\boxed{1=\sum_{j=0}^{M-1}p_j=\frac M2,}
$$

which contradicts $M>2$. Thus **one query cannot decide constancy with certainty**. The other [constant function](../../../../../constant-function.md) gives $-I$, differing only by a [global phase](../../../../../global-phase.md), so it does not change the argument. For comparison, $M=2$ permits $p_0=p_1=1/2$; the impossibility arises from demanding the test work for every nonconstant [Boolean function](../../../../../boolean-function.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
