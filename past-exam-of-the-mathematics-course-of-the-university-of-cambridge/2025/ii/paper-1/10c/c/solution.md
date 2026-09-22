<h1 id="10c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Both $Z\otimes Z$ and $X\otimes I$ are unitary and Hermitian, so their expectations are real. Run the real-part [Hadamard test](../../../../../../hadamard-test.md) twice, once with controlled $Z\otimes Z$ and once with controlled $X\otimes I$. If the respective ancilla outcome-one probabilities are $p_{ZZ}$ and $p_{XI}$, then

$$
\langle\psi|Z\otimes Z|\psi\rangle=1-2p_{ZZ},\qquad
\langle\psi|X\otimes I|\psi\rangle=1-2p_{XI}.
$$

The identity in part (b) implements each controlled tensor product by gates on its two target wires with the common control. By [linearity](../../../../../../linearity.md),

$$
\langle\psi|W|\psi\rangle=2-2(p_{ZZ}+p_{XI}).
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10C](../../10c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
