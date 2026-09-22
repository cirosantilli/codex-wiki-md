<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume no previously shared [entanglement](../../../../../../entangled-state.md). Alice's encoded ensemble $\{p_x,\rho_x\}$ lives in a [Hilbert space](../../../../../../hilbert-space-split.md) of dimension $2^n$. Its [Holevo quantity](../../../../../../holevo-quantity.md) satisfies

$$
\chi_{\rm in}=S\left(\sum_xp_x\rho_x\right)-\sum_xp_xS(\rho_x)
\leq\log_2(2^n)=n,
$$

using nonnegativity of [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) and the [maximum entropy of a quantum state](../../../../../../maximum-entropy-of-a-quantum-state.md). The [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) implies $\chi_{\rm out}\leq\chi_{\rm in}$ for the transmission [quantum channel](../../../../../../quantum-channel.md). Finally, the [Holevo bound](../../../../../../holevo-s-theorem.md) applied to Bob's [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) gives

$$
\boxed{I(X:Y)\leq\chi_{\rm out}\leq n\text{ bits}}.
$$

This argument also works when the output system has larger dimension than the input. Prior shared [entanglement](../../../../../../entangled-state.md) changes the communication resource: [superdense coding](../../../../../../superdense-coding.md) can transmit two classical bits per sent qubit, so the absence of that resource is part of this bound's setting.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
