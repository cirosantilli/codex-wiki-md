<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Gottesman--Knill theorem](../../../../../../gottesman-knill-theorem.md) states that [stabilizer-state preparation](../../../../../../stabilizer-state-preparation.md), [Clifford circuits](../../../../../../clifford-circuit.md), and adaptive [Measurements of Pauli observables](../../../../../../measurement-of-a-pauli-observable.md) can be simulated in classical polynomial time. For $|\Psi_{\rm in}\rangle=|+\rangle^{\otimes3}$, choose generators $XII$, $IXI$, and $IIX$. With each row written as $[x_1x_2x_3\mid z_1z_2z_3]$, its sign-free [stabilizer tableau](../../../../../../stabilizer-tableau.md) is

$$
\begin{pmatrix}
1&0&0&\mid&0&0&0\\
0&1&0&\mid&0&0&0\\
0&0&1&\mid&0&0&0
\end{pmatrix}.
$$

Conjugating these generators successively by $\operatorname{CNOT}_{21}$, $H_2\otimes H_3$, and $\operatorname{CNOT}_{13}$ gives $XIX$, $XZX$, and $ZIZ$. Hence the output tableau, again ignoring signs, is

$$
\begin{pmatrix}
1&0&1&\mid&0&0&0\\
1&0&1&\mid&0&1&0\\
0&0&0&\mid&1&0&1
\end{pmatrix}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
