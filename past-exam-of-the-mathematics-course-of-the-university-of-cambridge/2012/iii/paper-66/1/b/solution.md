<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the nonnegative representative of reduction modulo four. The four product [eigenstates](../../../../../../eigenstate.md) and [eigenvalues](../../../../../../eigenvalue.md) are

$$
\begin{array}{c|rrrr}
\text{state}&|00\rangle&|01\rangle&|10\rangle&|11\rangle\\
\text{eigenvalue}&2&0&0&2
\end{array}
$$

because $-2\equiv2\pmod4$. Consequently the observable is **$I+Z_AZ_B$**. It has the even sector $\operatorname{span}\{|00\rangle,|11\rangle\}$ with value two and the odd sector $\operatorname{span}\{|01\rangle,|10\rangle\}$ with value zero.

The [entanglement-assisted nondemolition parity measurement](../../../../../../entanglement-assisted-nondemolition-parity-measurement.md) needs just the single shared $|\Phi^+\rangle$ provided in the question. Apply $\operatorname{CNOT}_{A\to d_1}$ and $\operatorname{CNOT}_{B\to d_2}$. For a computational-basis input $|a b\rangle$, the meter becomes

$$
\frac{|a b\rangle_d+|1\oplus a,1\oplus b\rangle_d}{\sqrt2}.
$$

Measuring the meters gives $u\oplus v=a\oplus b$. For an arbitrary coherent system input, its conditional [Kraus operator](../../../../../../kraus-operator.md) is

$$
K_{uv}=\frac1{\sqrt2}P_{u\oplus v},\qquad
P_p=\frac{I+(-1)^pZ_AZ_B}{2}.
$$

It preserves every superposition within the measured sector, so this realizes the [Lüders rule](../../../../../../luders-rule.md) for the two degenerate [eigenvalues](../../../../../../eigenvalue.md). The answer is **two for equal meter bits, zero for unequal meter bits**. Each individual meter bit is uniform; only later comparison reveals the parity, respecting [quantum no-signalling](../../../../../../quantum-no-signalling.md). This construction is independent of the defective one-pair singlet-verification request in part (a).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
