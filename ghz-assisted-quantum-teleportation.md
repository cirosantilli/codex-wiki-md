# GHZ-assisted quantum teleportation

↑ **Parent:** [Controlled quantum teleportation](controlled-quantum-teleportation.md)

Share a [GHZ state](greenberger-horne-zeilinger-state.md) on $A,B,C$ and let the unknown input $Q$ be $|\chi\rangle$. Alice applies CNOT from $Q$ to $A$, then a [Hadamard gate](hadamard-gate.md) to $Q$, and measures $Q,A$ computationally, giving $s,t$. Charlie measures $C$ in the [Hadamard basis](hadamard-basis.md), giving $c$. Bob's conditional state is

$$
X^tZ^{s\oplus c}|\chi\rangle,
$$

up to a [global phase](global-phase.md). Alice's two [bits](bit.md) and Charlie's one [bit](bit.md) therefore specify Bob's inverse correction $Z^{s\oplus c}X^t$.

To prove the phase rule, write $|\chi\rangle=\alpha|0\rangle+\beta|1\rangle$. After Alice's result, $BC$ is $\alpha|tt\rangle+(-1)^s\beta|(1\oplus t)(1\oplus t)\rangle$. Taking Charlie's [Hadamard basis](hadamard-basis.md) partial [inner product](inner-product-split.md) multiplies its second term relative to its first by $(-1)^c$. The remaining common phase is $(-1)^{ct}$, which is physically irrelevant. All eight result triples have [probability](probability.md) $1/8$. Charlie's record localizes a known-phase [Bell pair](bell-pair.md), allowing the standard [Bell-basis teleportation identity](bell-basis-teleportation-identity.md) to complete the transfer.

## ↑ Ancestors (8)

1. [Controlled quantum teleportation](controlled-quantum-teleportation.md)
2. [Quantum teleportation](quantum-teleportation.md)
3. [Local operations and classical communication](local-operations-and-classical-communication.md)
4. [Bell state](bell-state-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/quantum-information/3/c/ii/solution.md)
