<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $V$ denote the coherent [exact quantum phase estimation](../../../../../../../exact-quantum-phase-estimation.md) [unitary operator](../../../../../../../unitary-operator.md) from the preceding part, with the data [quantum register](../../../../../../../quantum-register.md) written first. For every [eigenvector](../../../../../../../eigenvector.md) of $A$,

$$
V|u_j\rangle|0^n\rangle=|u_j\rangle|c_j\rangle,
$$

because $e^{2\pi iA}|u_j\rangle=e^{2\pi i\lambda_j}|u_j\rangle$ and $\lambda_j=c_j/2^n$ lies in $[0,1)$, with no phase-aliasing ambiguity. Apply $V$ coherently to the input [quantum state](../../../../../../../quantum-state.md) and a clean [quantum register](../../../../../../../quantum-register.md); do not measure the [eigenvalue](../../../../../../../eigenvalue.md) label. By [linearity](../../../../../../../linearity.md) it produces $\sum_j\beta_j|u_j\rangle|c_j\rangle$.

Append a [quantum ancilla](../../../../../../../quantum-ancilla.md) in $|0\rangle$, and use the provided [quantum variable rotation](../../../../../../../quantum-variable-rotation.md) with $\theta_{c_j}=\arcsin\lambda_j$, choosing the nonnegative cosine. The resulting normalized [quantum state](../../../../../../../quantum-state.md) is

$$
\boxed{\sum_j\beta_j|u_j\rangle|c_j\rangle\left(\sqrt{1-\lambda_j^2}|0\rangle+\lambda_j|1\rangle\right).}
$$

The sum covers both terms; this fixes the potentially ambiguous sum placement in the abbreviated display. The [orthonormal basis](../../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../../eigenvector.md) and the unit length of each rotated [quantum ancilla](../../../../../../../quantum-ancilla.md) show that its [norm](../../../../../../../norm.md) is one. This is [quantum spectral filtering](../../../../../../../quantum-spectral-filtering.md) by multiplication, not the reciprocal rotation used in the [HHL algorithm](../../../../../../../hhl-algorithm.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
