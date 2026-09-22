<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The pure state $|\Psi\rangle_{AB}$ is [entangled](../../../../../entangled-state.md) when it cannot be written as a [product state](../../../../../product-state.md) $|a\rangle_A|b\rangle_B$, equivalently when its [Schmidt rank](../../../../../schmidt-rank.md) exceeds one. Its subsystem states are the [reduced density matrices](../../../../../reduced-density-matrix.md)

$$
\rho_A=\operatorname{Tr}_B|\Psi\rangle\langle\Psi|,
\qquad
\rho_B=\operatorname{Tr}_A|\Psi\rangle\langle\Psi|,
$$

where the [partial trace](../../../../../partial-trace.md) is characterized by $\operatorname{Tr}(M_A\rho_A)=\langle\Psi|M_A\otimes I_B|\Psi\rangle$ for every observable $M_A$.

Let Bob's measurement have [Kraus operators](../../../../../kraus-operator.md) $M_b$ satisfying $\sum_bM_b^\dagger M_b=I_B$. If Alice does not learn Bob's random outcome, her state after the measurement is

$$
\begin{aligned}
\rho'_A
&=\operatorname{Tr}_B\sum_b(I\otimes M_b)\rho_{AB}(I\otimes M_b^\dagger)\\
&=\operatorname{Tr}_B\left[\rho_{AB}
\left(I\otimes\sum_bM_b^\dagger M_b\right)\right]
=\rho_A.
\end{aligned}
$$

This [no-communication theorem](../../../../../no-communication-theorem.md) means that Bob can change Alice's conditional state after she learns his outcome, but cannot change any local outcome distribution available to her alone. Standard [nonrelativistic quantum mechanics](../../../../../nonrelativistic-quantum-mechanics.md) is therefore operationally compatible with the prohibition of [superluminal signalling](../../../../../faster-than-light-communication.md) in [special relativity](../../../../../special-relativity-split.md), despite its nonlocal conditional-state updates.

An exact nondisturbing state readout would destroy this protection if it reported the globally collapsed state on an absolute-time slice. For example, Alice and Bob may share [Bell states](../../../../../bell-state-split.md). At a prearranged time Bob encodes a bit by measuring his qubit in either the computational or [Hadamard basis](../../../../../hadamard-basis.md). The usual projection postulate assigns Alice respectively one of $|0\rangle,|1\rangle$ or one of $|+\rangle,|-\rangle$. A device returning the exact pure state lets Alice identify which basis Bob chose without waiting for his outcome, producing a [superluminal signal](../../../../../faster-than-light-communication.md). Equivalently, Bob may choose whether to measure, and the device distinguishes the resulting proper pure state from the original improper maximally mixed local state.

A causal alternative is a [quantum state readout device](../../../../../quantum-state-readout-device.md) located at a spacetime point $x$ that reports the [local quantum state under objective collapse](../../../../../local-quantum-state-under-objective-collapse.md): take reduced states on spacelike hypersurfaces through $x$ and let those hypersurfaces approach the past [light cone](../../../../../light-cone.md) of $x$. The result includes localized collapses in $J^-(x)$ and excludes spacelike-separated collapses. This assumes a fixed [Minkowski spacetime](../../../../../minkowski-spacetime.md), localized collapse events, ordinary local unitary dynamics between them, and outputs that may control only operations in their causal future. The postulate is logically consistent because it adds a classical record of this local state without changing the state or any standard measurement probability. It also cannot support an indirect signalling algorithm. Inductively through the algorithm's events, every readout at $x$ depends only on operations, collapses, and earlier readouts in $J^-(x)$; any operation selected from that output lies in the readout's future light cone. Composing readouts, unitary evolutions, and measurements therefore never carries a controllable dependence outside a future light cone, so [relativistic causality](../../../../../relativistic-causality.md) is preserved.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
