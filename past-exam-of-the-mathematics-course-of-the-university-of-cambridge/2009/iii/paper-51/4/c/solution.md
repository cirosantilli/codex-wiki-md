<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Number the three data [qubits](../../../../../../qubit.md) from top to bottom. It suffices initially to follow a pure input $|\psi\rangle=a|0\rangle+b|1\rangle$; linearity will extend the result to every [density operator](../../../../../../density-matrix.md). The first two [controlled-NOT gates](../../../../../../controlled-not-gate.md) create $a|000\rangle+b|111\rangle$. The first layer of [Hadamard gates](../../../../../../hadamard-gate.md) then encodes this as

$$
a|+++\rangle+b|---\rangle,
$$

the three-[qubit](../../../../../../qubit.md) [phase-flip repetition code](../../../../../../phase-flip-repetition-code.md). Let $e_i$ indicate whether a [Pauli Z gate](../../../../../../pauli-z-gate.md) occurred on data [qubit](../../../../../../qubit.md) $i$ during storage. The next layer of [Hadamard gates](../../../../../../hadamard-gate.md) uses $HZH=X$ and gives

$$
a|e_1e_2e_3\rangle+b|1\oplus e_1,1\oplus e_2,1\oplus e_3\rangle.
$$

The two initially zero syndrome [quantum ancillas](../../../../../../quantum-ancilla.md) receive the adjacent parities. In the diagram's top-to-bottom order, their [error syndrome](../../../../../../error-syndrome.md) is

$$
s_1=e_1\oplus e_2,\qquad s_2=e_2\oplus e_3.
$$

Both terms of the logical superposition have these same parities, so the syndrome is independent of $a,b$. Measuring it reveals no logical-state information.

At the marked position of $R$ in the printed circuit, there has already been another layer of [Hadamard gates](../../../../../../hadamard-gate.md) on the data. There is also a layer immediately after $R$. Thus a desired correction $X_i$ in the parity-extraction frame must be implemented as $R=Z_i$ at the actual recovery location, since $H^{\otimes3}Z_iH^{\otimes3}=X_i$. Choose the recovery according to

$$
\boxed{\begin{array}{c|c|c|c}
(s_1,s_2)&\text{weight-zero or one pattern}&\text{complementary pattern}&R\\\hline
00&000&111&I\\
10&100&011&Z_1\\
11&010&101&Z_2\\
01&001&110&Z_3
\end{array}}
$$

The two patterns on each row share a syndrome because complementing all three bits does not change either parity. For a weight-zero or one error, the recovery removes the entire error in the parity-extraction frame. The remaining state is $a|000\rangle+b|111\rangle$, and the two final [controlled-NOT gates](../../../../../../controlled-not-gate.md) give $|\psi\rangle|00\rangle$.

For a weight-two or three error, minimum-weight recovery instead leaves all three bits flipped, giving $a|111\rangle+b|000\rangle$. The final [controlled-NOT gates](../../../../../../controlled-not-gate.md) send this to $(a|1\rangle+b|0\rangle)|00\rangle=X|\psi\rangle|00\rangle$. Consequently, for every input [density operator](../../../../../../density-matrix.md),

$$
\boxed{\rho'=\rho\quad(k=0,1),\qquad\rho'=X\rho X\quad(k=2,3).}
$$

The logical failure is a [Pauli X gate](../../../../../../pauli-x-gate.md) after decoding, even though the stored physical errors were [Pauli Z gates](../../../../../../pauli-z-gate.md): $Z_1Z_2Z_3$ exchanges the two encoded codewords. This is the [logical failure of the three-qubit phase-flip repetition code](../../../../../../logical-failure-of-the-three-qubit-phase-flip-repetition-code.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
