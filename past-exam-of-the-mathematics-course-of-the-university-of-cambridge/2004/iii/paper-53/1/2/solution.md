<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The mixed-state expression in the PDF contains a mismatched bra in its second term. A probability mixture of the stated orthonormal [eigenvectors](../../../../../../eigenvector.md) must be interpreted as $\rho=\sum_kp_k|u_k\rangle\langle u_k|$. Taken literally with a different bra, it need not be Hermitian or positive and is not generally a [density operator](../../../../../../density-matrix.md).

Let $m=\sum_kp_ke^{i\phi_k}=\operatorname{Tr}(\rho U)$. A [quantum channel](../../../../../../quantum-channel.md) and its measurement probabilities are linear in the [density operator](../../../../../../density-matrix.md), so averaging the pure-state results gives

$$
P_0-P_1=\operatorname{Re}m,\qquad P_--P_+=\operatorname{Im}m.
$$

Therefore the same frequency estimator yields

$$
\boxed{\widehat m=(\widehat P_0-\widehat P_1)+i(\widehat P_--\widehat P_+).}
$$

More generally, after the controlled operation and before the final [Hadamard gate](../../../../../../hadamard-gate.md), the reduced control [density operator](../../../../../../density-matrix.md) is

$$
\frac12\begin{pmatrix}1&\overline{\operatorname{Tr}(\rho U)}\\\operatorname{Tr}(\rho U)&1\end{pmatrix}.
$$

This follows by a [partial trace](../../../../../../partial-trace.md) of the control blocks $\rho$, $\rho U^\dagger$, $U\rho$ and $U\rho U^\dagger$. It proves the [mixed-state Hadamard-test quadratures](../../../../../../mixed-state-hadamard-test-quadratures.md) for any auxiliary [density operator](../../../../../../density-matrix.md), even one not diagonal in the eigenbasis. Conjugation by the final [Hadamard gate](../../../../../../hadamard-gate.md) maps $X$ to $Z$ and $Y$ to $-Y$, explaining the imaginary-part sign.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
