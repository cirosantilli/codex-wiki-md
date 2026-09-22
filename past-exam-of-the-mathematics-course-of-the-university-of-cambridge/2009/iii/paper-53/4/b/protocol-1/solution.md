<h1 id="4/b/protocol-1/solution">Solution</h1>

↑ **Parent:** [Protocol 1](../protocol-1.md)

**Insecure as a proposed test-and-purify protocol: the basis string and check positions are announced before receipt.** Eve can intercept and store the travelling qubits until the announcement. For each data position with basis bit $b_j$, she measures the stored qubit in the basis $\{H^{b_j}|0\rangle,H^{b_j}|1\rangle\}$. If the outcome is $z_j$, the Alice–Bob pair becomes

$$
|z_j\rangle_A\otimes H^{b_j}|z_j\rangle_B,
$$

and Eve knows $z_j$. She forwards that qubit, and forwards every publicly identified check qubit untouched. After Bob's [Hadamard gate](../../../../../../../hadamard-gate.md) decoding, every data pair is the known [product state](../../../../../../../product-state.md) $|z_jz_j\rangle$, while the unmodified check pairs remain perfect. Thus the check [bit error rate](../../../../../../../bit-error-rate.md) is zero even though Eve knows all raw data bits. This is [premature basis announcement in quantum key distribution](../../../../../../../premature-basis-announcement-in-quantum-key-distribution.md).

The retained data are a [separable quantum state](../../../../../../../separable-quantum-state.md) with a classical label held by Eve; [LOCC](../../../../../../../local-operations-and-classical-communication.md) cannot turn them into private [Bell pairs](../../../../../../../bell-pair.md). Consequently the listed check does not justify the claimed success of the subsequent [entanglement purification](../../../../../../../entanglement-distillation.md). A sound purification procedure that independently detects the missing entanglement must fail or abort on this attack. If Step 9 were instead read as an independently guaranteed production of private, nearly perfect [Bell pairs](../../../../../../../bell-pair.md), their subsequent key would of course be private; the flaw is that this protocol's test cannot establish that guarantee. Naming an EPP does not repair the information leak or the invalid sampling test.

## ↑ Ancestors (12)

1. [Protocol 1](../protocol-1.md)
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
