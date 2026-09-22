# Premature basis announcement in quantum key distribution

↑ **Parent:** [Quantum key distribution](quantum-key-distribution.md)

If basis information and test positions are announced before the receiver confirms receipt of quantum carriers, an eavesdropper can store the carriers until learning that information. In a scheme sending one half of each [Bell pair](bell-pair.md) after a [Hadamard gate](hadamard-gate.md) encoding, the eavesdropper then forwards test qubits untouched and measures all data qubits in their now-known correct bases. Every test passes, while data are changed to classically correlated [product states](product-state.md) whose bit labels the eavesdropper knows. This invalidates the sampling argument needed to justify [entanglement purification](entanglement-distillation.md) and [quantum key distribution](quantum-key-distribution.md). A sound additional purification certification could detect this attack and abort; it cannot generate private [Bell pairs](bell-pair.md) from the separable attacked data. Announcing bases only after receipt prevents this particular delayed-carrier attack.

## ↑ Ancestors (4)

1. [Quantum key distribution](quantum-key-distribution.md)
2. [Cryptography](cryptography.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/4/b/protocol-1/solution.md)
