<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $C_U=|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes U$ for the [controlled unitary gate](../../../../../controlled-unitary-gate.md). For a normalized [eigenvector](../../../../../eigenvector.md) $|u\rangle$, the first [Hadamard gate](../../../../../hadamard-gate.md) and [quantum phase kickback](../../../../../phase-kickback.md) give

$$
|0\rangle|u\rangle\longmapsto\frac{|0\rangle+|1\rangle}{\sqrt2}|u\rangle\longmapsto\frac{|0\rangle+e^{i\phi}|1\rangle}{\sqrt2}|u\rangle.
$$

The final [Hadamard gate](../../../../../hadamard-gate.md) therefore produces the unentangled output

$$
|\chi_\phi\rangle|u\rangle,\qquad |\chi_\phi\rangle=\frac{1+e^{i\phi}}2|0\rangle+\frac{1-e^{i\phi}}2|1\rangle.
$$

The auxiliary system is unchanged, while its eigenphase becomes accessible through interference of the control [qubit](../../../../../qubit.md). The [special unitary group](../../../../../special-unitary-group.md) assumption is not needed for this calculation; unitarity and the normalized [eigenvector](../../../../../eigenvector.md) suffice.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
