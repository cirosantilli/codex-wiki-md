<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Number the wires from top to bottom as $1,\ldots,5$. The first two [controlled-NOT gates](../../../../../../controlled-not-gate.md) encode $|\psi\rangle=u|0\rangle+v|1\rangle$ into the [bit-flip repetition code](../../../../../../bit-flip-repetition-code.md)

$$
u|000\rangle+v|111\rangle
$$

on data wires $1,2,3$. The lower two zero ancillas store an [error syndrome](../../../../../../error-syndrome.md). Reading the PDF's four detection CNOTs gives

$$
s_4=b_2\oplus b_3,\qquad s_5=b_1\oplus b_3.
$$

The syndrome and the data qubit to be flipped are therefore

$$
\begin{array}{c|c|c}
\text{physical error}&(s_4,s_5)&\text{recovery target}\\\hline
I&00&\text{none}\\
X_1&01&1\\
X_2&10&2\\
X_3&11&3
\end{array}
$$

This is [coherent syndrome extraction for the three-qubit repetition code](../../../../../../coherent-syndrome-extraction-for-the-three-qubit-repetition-code.md). The recovery [Toffoli gates](../../../../../../toffoli-gate.md) implement these conditions; the intervening [Pauli X gates](../../../../../../pauli-x-gate.md) temporarily turn zero-valued controls into one-valued controls and then restore the syndrome wires. Finally, inverse encoding returns the logical state to the top wire and resets data wires 2 and 3 to zero.

For the specified error $X_1$, the encoded data becomes $u|100\rangle+v|011\rangle$. Both terms have syndrome $01$, so detection factors out $|01\rangle_{45}$ without revealing the logical amplitudes. Recovery flips data wire 1, restoring $u|000\rangle+v|111\rangle$, and decoding yields

$$
\boxed{|\psi\rangle_1\otimes|0\rangle_2\otimes|0\rangle_3\otimes|0\rangle_4\otimes|1\rangle_5.}
$$

The lower four wires need not all return to zero: their syndrome record is independent of the logical state, which is what the correction requirement needs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
