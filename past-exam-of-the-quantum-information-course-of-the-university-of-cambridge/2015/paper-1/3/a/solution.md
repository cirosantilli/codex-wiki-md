<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A bipartite pure state is entangled when it is not a [product state](../../../../../product-state.md). Its [Schmidt decomposition](../../../../../schmidt-decomposition.md) is $|\psi\rangle=\sum_i\sqrt{\lambda_i}|i_Ai_B\rangle$, where $\lambda_i\ge0$ and $\sum_i\lambda_i=1$. More than one nonzero coefficient means entanglement. The two [reduced density matrices](../../../../../reduced-density-matrix.md) have the same nonzero spectrum, and their [Von Neumann entropy](../../../../../von-neumann-entropy-split.md) $-\sum_i\lambda_i\log_2\lambda_i$ is the pure-state [entanglement entropy](../../../../../entanglement-entropy.md). A maximally entangled pair of qubits has one bit of this entropy.

For mixed states, classical correlations are not sufficient: a [separable quantum state](../../../../../separable-quantum-state.md) is a convex mixture $\sum_jp_j\rho_A^{(j)}\otimes\rho_B^{(j)}$, and entanglement means that no such decomposition exists. A reduced entropy alone no longer measures mixed-state entanglement. An [entanglement witness](../../../../../entanglement-witness.md) or a suitable separability criterion can detect it.

[Local unitary transformations](../../../../../local-unitary-operation.md) preserve the Schmidt spectrum. More general [local operations and classical communication](../../../../../local-operations-and-classical-communication.md) can discard entanglement but cannot freely create it from a separable input. [Nielsen's pure-state conversion theorem](../../../../../nielsen-s-pure-state-conversion-theorem.md) gives the exact deterministic criterion: $|\psi\rangle\to|\phi\rangle$ is possible precisely when $\lambda^\psi\prec\lambda^\phi$. In decreasing order, every partial sum for the input is no larger than the corresponding output sum, with equal totals. The direction matters: a uniform spectrum can be converted to a concentrated one; a product state cannot deterministically become a Bell pair.

A probabilistic local filter can concentrate a partially entangled pair. For $|\psi\rangle=\sqrt\lambda|00\rangle+\sqrt{1-\lambda}|11\rangle$ with $1/2\le\lambda<1$, Alice's successful operator $F=\operatorname{diag}(\sqrt{(1-\lambda)/\lambda},1)$ produces equal amplitudes. The outcome is a Bell pair with probability $2(1-\lambda)$; a complementary operator supplies a complete measurement. Failure is heralded, so there is no deterministic creation of a more entangled pair. This illustrates [entanglement concentration](../../../../../entanglement-concentration.md).

Many-copy [entanglement distillation](../../../../../entanglement-distillation.md) and [entanglement dilution](../../../../../entanglement-dilution.md) connect noisy or nonuniform resources with standard Bell pairs. Entanglement enables [quantum teleportation](../../../../../quantum-teleportation.md) and other protocols, but classical communication is still required; the [no-communication theorem](../../../../../no-communication-theorem.md) excludes message transmission merely by choosing a distant local measurement.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
