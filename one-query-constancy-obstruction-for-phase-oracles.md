# One-query constancy obstruction for phase oracles

↑ **Parent:** [Phase oracle](phase-oracle.md)

An unrestricted [Boolean function](boolean-function.md) on $M>2$ inputs cannot be classified as constant or nonconstant with certainty using a single [phase oracle](phase-oracle.md) query, even with [quantum ancillas](quantum-ancilla.md). Write a purified query input as $|\Psi\rangle=\sum_x|x\rangle|a_x\rangle$ with $p_x=\|a_x\|^2$ and $\sum_xp_x=1$. The zero [constant function](constant-function.md) leaves it unchanged; the function supported only at $j$ produces a vector with [inner product](inner-product-split.md) $1-2p_j$ with it. [Perfect discrimination of pure states requires orthogonality](perfect-discrimination-of-pure-states-requires-orthogonality.md), forcing $p_j=1/2$ for all $j$ and thus $M=2$, a contradiction. This is an [exact quantum query complexity](exact-quantum-query-complexity.md) obstruction for all nonconstant inputs, rather than the restricted promise used by the [Deutsch-Jozsa algorithm](deutsch-jozsa-algorithm.md).

## ↑ Ancestors (8)

1. [Phase oracle](phase-oracle.md)
2. [Quantum oracle](quantum-oracle.md)
3. [Quantum query complexity](quantum-query-complexity.md)
4. [Quantum complexity theory](quantum-complexity-theory.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/quantum-information/2/d/solution.md)
