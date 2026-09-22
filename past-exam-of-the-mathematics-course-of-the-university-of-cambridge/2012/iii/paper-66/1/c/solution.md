<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use one shared $|\Phi^+\rangle$ pair to measure $Z_AZ_B$, and the other to measure $X_AX_B$. The latter [entanglement-assisted nondemolition parity measurement](../../../../../../entanglement-assisted-nondemolition-parity-measurement.md) is obtained by applying [Hadamard gates](../../../../../../hadamard-gate.md) to both system [qubits](../../../../../../qubit.md) before and after the $Z$-parity circuit. Since $ZX=-XZ$ at each site, the two minus signs cancel, giving $[Z_AZ_B,X_AX_B]=0$.

The [Bell states](../../../../../../bell-state-split.md) have joint [eigenvalues](../../../../../../eigenvalue.md)

$$
\begin{array}{c|rrrr}
\text{state}&\Phi^+&\Phi^-&\Psi^+&\Psi^-\\
Z_AZ_B&+1&+1&-1&-1\\
X_AX_B&+1&-1&+1&-1
\end{array}
$$

and are therefore distinguished uniquely by the two meter parities. For records $(u,v)$ and $(r,s)$, the combined [Kraus operator](../../../../../../kraus-operator.md) is

$$
K_{uvrs}=\frac12P_{z,x},\qquad
P_{z,x}=\frac14(I+zZ_AZ_B)(I+xX_AX_B),
\quad z=(-1)^{u\oplus v},\quad x=(-1)^{r\oplus s}.
$$

Each $P_{z,x}$ is the rank-one projector onto the corresponding [Bell state](../../../../../../bell-state-split.md). This is a [Bell-state nondemolition measurement](../../../../../../bell-state-nondemolition-measurement.md): an input [Bell state](../../../../../../bell-state-split.md) remains exactly that state for every possible local record. The local circuits can be scheduled without communication; the identity of the [Bell state](../../../../../../bell-state-split.md) is known only when the classical records are brought together. **Two parity bits distinguish all four Bell states without disturbing them.**

## ↑ Ancestors (11)

1. [C](../c.md)
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
