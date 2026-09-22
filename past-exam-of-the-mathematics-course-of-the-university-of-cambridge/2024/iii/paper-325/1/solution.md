<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let a [projective measurement](../../../../../projective-measurement.md) have mutually [orthogonal projections](../../../../../orthogonal-projection.md) $P_i$ satisfying $\sum_iP_i=I$. On a [density operator](../../../../../density-matrix.md) $\rho$, the [Born rule](../../../../../born-rule.md) and the [Lüders rule](../../../../../luders-rule.md) give

$$
\Pr(i)=\operatorname{Tr}(P_i\rho),
\qquad
\rho\longmapsto
\frac{P_i\rho P_i}{\operatorname{Tr}(P_i\rho)}
$$

conditional on outcome $i$. On the first part of a [bipartite quantum system](../../../../../tensor-product-of-quantum-systems.md), replace $P_i$ by $P_i\otimes I_2$.

The subsystems are isolated when there is no interaction term coupling them. Their [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) has the form

$$
H=H_1\otimes I_2+I_1\otimes H_2,
$$

so their subsequent [unitary time evolution](../../../../../unitary-time-evolution.md) factorizes as $U_1\otimes U_2$.

The [reduced density matrix](../../../../../reduced-density-matrix.md) of subsystem 1 is

$$
\boxed{\rho_1=\operatorname{Tr}_2\rho_{12}},
$$

where the [partial trace](../../../../../partial-trace.md) is characterized by

$$
\operatorname{Tr}_1(M_1\rho_1)
=\operatorname{Tr}_{12}[(M_1\otimes I_2)\rho_{12}]
$$

for every local [observable](../../../../../observable.md) $M_1$. Thus $\rho_1$ contains exactly the statistics accessible by measurements on subsystem 1.

Suppose a projective measurement $\{Q_j\}$ is performed on subsystem 2 and its outcome is not communicated. The resulting nonselective state is

$$
\rho'_{12}=\sum_j(I_1\otimes Q_j)\rho_{12}(I_1\otimes Q_j).
$$

For every $M_1$, the [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md) and $\sum_jQ_j^2=I_2$ give

$$
\begin{aligned}
\operatorname{Tr}[(M_1\otimes I_2)\rho'_{12}]
&=\sum_j\operatorname{Tr}[(M_1\otimes Q_j^2)\rho_{12}]\\
&=\operatorname{Tr}[(M_1\otimes I_2)\rho_{12}].
\end{aligned}
$$

Hence $\rho'_1=\rho_1$. No local projective measurement on subsystem 1 can reveal whether the remote unreported measurement occurred. This is [quantum no-signalling](../../../../../quantum-no-signalling.md), which prevents a choice made at a [spacelike separation](../../../../../spacelike-separation.md) from transmitting information faster than light and makes the measurement formalism compatible with [relativistic causality](../../../../../relativistic-causality.md).

The proposed nondisturbing device would violate [no information without disturbance](../../../../../no-information-without-disturbance.md). In an ordinary quantum instrument, let $M_{i\alpha}$ be the [Kraus operators](../../../../../kraus-operator.md) associated with classical output $i$. If every pure state $|\psi\rangle$ remains unchanged even conditional on the displayed outcome, every nonzero $M_{i\alpha}|\psi\rangle$ must be parallel to $|\psi\rangle$. A linear operator for which every vector is an [eigenvector](../../../../../eigenvector.md) is a scalar multiple of the identity, so $M_{i\alpha}=c_{i\alpha}I$. Its output probability

$$
\sum_\alpha\langle\psi|M_{i\alpha}^\dagger M_{i\alpha}|\psi\rangle
=\sum_\alpha|c_{i\alpha}|^2
$$

is independent of the state. It cannot equal $\langle\psi|P_i|\psi\rangle$ for arbitrary projectors. Equivalently, repeated nondisturbing samples would permit [quantum state tomography](../../../../../quantum-state-tomography.md) of one specimen and then [quantum cloning](../../../../../quantum-cloning.md), contradicting ordinary quantum theory.

Such devices would not _necessarily_ enable [superluminal signalling](../../../../../faster-than-light-communication.md). One consistent operational extension could make every sequence of outputs depend only on the local [reduced density matrix](../../../../../reduced-density-matrix.md) and local settings. Since an unreported remote measurement leaves that matrix unchanged, all local device statistics would remain unchanged too. Other extensions could add nonlocal outcome-dependent rules and permit signalling, but that behavior is additional to the device specification rather than forced by it.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
