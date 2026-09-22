<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [positive operator-valued measure](../../../../../positive-operator-valued-measure.md) consists of [positive semidefinite](../../../../../positive-semidefinite-matrix.md) effects $E_r$ with $\sum_rE_r=I$. Its outcome probabilities are $p_r=\operatorname{Tr}(\rho E_r)$, which are nonnegative and sum to one. Unlike a [projective measurement](../../../../../projective-measurement.md), its effects need not be mutually [orthogonal projections](../../../../../orthogonal-projection.md), and there can be more outcomes than the system's Hilbert-space dimension.

For example, choose three equatorial [Bloch vectors](../../../../../bloch-vector.md) $\mathbf n_r$ separated by $120^\circ$ and set $E_r=(I+\mathbf n_r\cdot\boldsymbol\sigma)/3$. Each effect has [eigenvalues](../../../../../eigenvalue.md) zero and $2/3$, and the vectors sum to zero, so the three effects sum to $I$. This [trine qubit POVM](../../../../../trine-qubit-povm.md) gives $p_r=(1+\mathbf s\cdot\mathbf n_r)/3$ for input [Bloch vector](../../../../../bloch-vector.md) $\mathbf s$. It cannot be a three-outcome orthogonal [projective measurement](../../../../../projective-measurement.md) on that [qubit](../../../../../qubit.md).

A physical implementation can couple the system to an [ancilla](../../../../../quantum-ancilla.md) and projectively measure the enlarged system. More generally, operators $M_{r\alpha}$ implement an outcome with $E_r=\sum_\alpha M_{r\alpha}^\dagger M_{r\alpha}$; the normalized conditional state is $\sum_\alpha M_{r\alpha}\rho M_{r\alpha}^\dagger/p_r$. Thus a [POVM does not determine the post-measurement state](../../../../../povm-does-not-determine-the-post-measurement-state.md): different [measurement instruments](../../../../../quantum-instrument.md) can have the same outcome probabilities and different disturbance. [Generalized measurements](../../../../../generalized-measurement-postulate.md) are useful for state discrimination and realistic detection, including explicitly modeled inconclusive outcomes.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the quantum information course of the University of Cambridge](../../../../split.md)
6. [Quantum Information course of the University of Cambridge](../../../../../quantum-information-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
