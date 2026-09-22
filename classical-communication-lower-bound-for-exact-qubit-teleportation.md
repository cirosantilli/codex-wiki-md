# Classical communication lower bound for exact qubit teleportation

↑ **Parent:** [Quantum teleportation](quantum-teleportation.md)

Exact [quantum teleportation](quantum-teleportation.md) that preserves an arbitrary reference requires at least two classical [bits](bit.md) from sender to receiver, even with preshared [quantum entanglement](entangled-state.md). For the essential reduction, encode two classical [bits](bit.md) in the four [Bell states](bell-state-split.md) by [Pauli gates](pauli-gate.md) on the sender's half of a [Bell pair](bell-pair.md). [Teleportation as an identity channel on a reference](teleportation-as-an-identity-channel-on-a-reference.md) transfers this half while preserving the encoding. The receiver then has both halves and recovers both [bits](bit.md) by a [Bell-basis measurement](bell-basis-measurement.md), as in [superdense coding](superdense-coding.md).

The classical [bit](bit.md) bound itself has a short [no-communication theorem](no-communication-theorem.md) proof. For $N$ possible messages and $K$ possible classical transmissions, let $\sigma_{m,c}$ be the receiver's subnormalized conditional [density matrix](density-matrix-split.md) before decoding. The [no-communication theorem](no-communication-theorem.md) gives $\sum_c\sigma_{m,c}=\tau$, independent of $m$, so $0\leq\sigma_{m,c}\leq\tau$. For each transmission $c$, let $\{E_{m|c}\}_m$ be the decoding [POVM](positive-operator-valued-measure.md). Averaging over equiprobable messages,

$$
p_{\mathrm{success}}=\frac1N\sum_{m,c}\operatorname{Tr}(E_{m|c}\sigma_{m,c})
\leq\frac1N\sum_c\operatorname{Tr}\left(\sum_m E_{m|c}\tau\right)=\frac KN.
$$

Perfect decoding of four messages requires $K\geq4$, hence at least two classical [bits](bit.md). This applies to the preshared resources of the proposed [quantum teleportation](quantum-teleportation.md) protocol as well as the [Bell pair](bell-pair.md) used for the encoding.

## ↑ Ancestors (7)

1. [Quantum teleportation](quantum-teleportation.md)
2. [Local operations and classical communication](local-operations-and-classical-communication.md)
3. [Bell state](bell-state-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/quantum-information/3/d/iii/solution.md)
