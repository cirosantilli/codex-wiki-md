<h1 id="4/b/protocol-3/solution">Solution</h1>

↑ **Parent:** [Protocol 3](../protocol-3.md)

**Secure in the intended ideal setting, with a sound entanglement-purification procedure.** Bob confirms receipt before Alice reveals either the random basis string or the randomly chosen check positions. Eve must therefore release the travelling qubits before knowing which basis to use and which positions to protect from disturbance. Bob can then decode because $H^2=I$.

The random check sample tests the same ensemble of encoded transmissions as the retained data. Random [computational basis](../../../../../../../computational-basis.md) and [Hadamard basis](../../../../../../../hadamard-basis.md) encodings make the test sensitive to complementary disturbances; Eve cannot use the targeted zero-error attack available in Protocol 1. For example, measuring every intercepted qubit in one fixed one of these two bases uses the wrong basis half the time, and then disagrees with Alice half the time, producing a [bit error rate](../../../../../../../bit-error-rate.md) of $1/4$. A sound [entanglement purification](../../../../../../../entanglement-distillation.md) protocol uses the tested error bounds, corrects both relevant types of error, and aborts if the noise is too high; secrecy is not claimed for every possible attack without an abort option.

When the protocol succeeds in producing nearly perfect [Bell pairs](../../../../../../../bell-pair.md), [purity decouples a subsystem from its purification](../../../../../../../purity-decouples-a-subsystem-from-its-purification.md) explains why they are nearly independent of Eve, and matching [computational basis](../../../../../../../computational-basis.md) measurements produce an approximately uniform shared secret key. The disclosed check outcomes are discarded rather than included in that key. This is the standard entanglement-based [quantum key distribution](../../../../../../../quantum-key-distribution.md) ordering: receipt first, basis and sample disclosure second, testing and purification next, and private measurements last.

## ↑ Ancestors (12)

1. [Protocol 3](../protocol-3.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
