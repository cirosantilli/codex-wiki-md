<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first two [CNOT gates](../../../../../../controlled-not-gate.md) encode $u|0\rangle+v|1\rangle$ as

$$
|\psi_L\rangle=u|000\rangle+v|111\rangle,
$$

the three-qubit [bit-flip repetition code](../../../../../../bit-flip-repetition-code.md). In the printed detection circuit the first [quantum ancilla](../../../../../../quantum-ancilla.md) records $q_3\oplus q_2$ and the second records $q_2\oplus q_1$. Both start in $|0\rangle$. For an incoming bit-error pattern $e=(e_1,e_2,e_3)$, the two logical basis branches give the same [error syndrome](../../../../../../error-syndrome.md)

$$
s(e)=(e_2\oplus e_3,\ e_1\oplus e_2).
$$

Adding $111$ to a computational string leaves both parities unchanged, so the ancillas acquire no information about $u$ or $v$. The joint state after extraction is

$$
X_1^{e_1}X_2^{e_2}X_3^{e_3}|\psi_L\rangle\otimes|s(e)\rangle_{a_1a_2}.
$$

The syndrome measurement therefore preserves the unknown logical amplitudes. For zero or one bit flip the corrections are

$$
\boxed{\begin{array}{c|c|c}
(a_1,a_2)&\text{error}&\text{correction}\\\hline
00&I&I\\
01&X_1&X_1\\
10&X_3&X_3\\
11&X_2&X_2
\end{array}}
$$

Each indicated correction squares to the identity and restores the encoded state. The order of the two ancilla labels matters: the printed first ancilla is the $q_2,q_3$ parity, not the $q_1,q_2$ parity. This is [coherent syndrome extraction for the three-qubit repetition code](../../../../../../coherent-syndrome-extraction-for-the-three-qubit-repetition-code.md) with the circuit's specific parity choices.

For later use, an error pattern and its complement have the same syndrome. Minimum-weight recovery corrects patterns of weight zero or one. Patterns of weight two or three instead leave $X_1X_2X_3$, the logical bit flip that exchanges the two codewords. The code protects against the stated bit-flip channel, not arbitrary single-qubit phase errors.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
