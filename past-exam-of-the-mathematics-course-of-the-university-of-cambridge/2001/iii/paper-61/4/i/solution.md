<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Represent any universally quantum device, including its auxiliaries and arbitrary final readout, by a [positive operator-valued measure](../../../../../../positive-operator-valued-measure.md) $\{E_i\}$ on the input. Perfect identification would require

$$
E_i\geq0,\qquad \sum_iE_i=I,\qquad
\langle\phi_j|E_i|\phi_j\rangle=\delta_{ij}.
$$

Since a positive operator has a positive square root, zero expectation implies $E_i|\phi_j\rangle=0$ for $j\ne i$. Also $I-E_i\geq0$ and its expectation in $\phi_i$ is zero, so $E_i|\phi_i\rangle=|\phi_i\rangle$. Consequently

$$
\langle\phi_i|\phi_j\rangle
=\langle\phi_i|E_i|\phi_j\rangle=0
\qquad(i\ne j).
$$

This proves that [perfect discrimination of pure states requires orthogonality](../../../../../../perfect-discrimination-of-pure-states-requires-orthogonality.md). Any nonzero overlap contradicts perfect identification, independently of whether the device disturbs its input.

Equivalently, a [unitary operator](../../../../../../unitary-operator.md) coupling the input to a readout apparatus must preserve inner products. Distinct perfectly readable records have zero inner product, so their corresponding input vectors must already be orthogonal. **Nonorthogonal candidate states cannot be identified with certainty in one use.** Probabilistic [unambiguous quantum state discrimination](../../../../../../unambiguous-quantum-state-discrimination.md) can have an inconclusive outcome, which is excluded by the guaranteed-identification requirement.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
