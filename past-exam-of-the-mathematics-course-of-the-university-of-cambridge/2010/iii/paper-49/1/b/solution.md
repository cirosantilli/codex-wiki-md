<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If there is no marked entry, the [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) is the identity. The [uniform superposition state](../../../../../../uniform-superposition-state.md) is a positive eigenstate of the [Grover diffusion operator](../../../../../../grover-diffusion-operator.md):

$$
V|s\rangle=(2|s\rangle\langle s|-I)|s\rangle=|s\rangle.
$$

Thus every iteration leaves the full state $|s\rangle\otimes|-\rangle$ unchanged. The measured search bits have the [uniform distribution](../../../../../../continuous-uniform-distribution.md)

$$
\boxed{\mathbb P(\text{output }x)=\frac1N\quad(0\leq x<N).}
$$

Only the first $n$ qubits are measured in the printed circuit. If the untouched ancilla were also measured in the computational basis, its bit would be an independent fair bit, giving probability $1/(2N)$ for each joint outcome.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
