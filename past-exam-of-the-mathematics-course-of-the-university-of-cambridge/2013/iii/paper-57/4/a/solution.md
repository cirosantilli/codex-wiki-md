<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $B=\sum_k g_kZ_k$. In the [Zurek spin-bath model](../../../../../../zurek-spin-bath-model.md), $H=-Z_D\otimes B$, so [unitary time evolution](../../../../../../unitary-time-evolution.md) with $\hbar=1$ is $U(t)=e^{itZ_D\otimes B}$. The bath Hamiltonian terms commute, and device states $|0\rangle,|1\rangle$ have $Z_D$ eigenvalues $+1,-1$. Hence

$$
|\Psi(t)\rangle=a|0\rangle|E_0(t)\rangle+b|1\rangle|E_1(t)\rangle,
$$

where the two normalized conditional bath states are

$$
|E_0(t)\rangle=\bigotimes_k\left(\alpha_k e^{ig_kt}|\uparrow_k\rangle+\beta_k e^{-ig_kt}|\downarrow_k\rangle\right),\qquad
|E_1(t)\rangle=\bigotimes_k\left(\alpha_k e^{-ig_kt}|\uparrow_k\rangle+\beta_k e^{ig_kt}|\downarrow_k\rangle\right).
$$

Take each bath factor normalized, $|\alpha_k|^2+|\beta_k|^2=1$, and $|a|^2+|b|^2=1$. This entails no restriction: if only the product is initially normalized, divide each nonzero factor by its norm; the product of these norms is one.

Taking the [partial trace](../../../../../../partial-trace.md) over the bath gives the [reduced density matrix](../../../../../../reduced-density-matrix.md)

$$
\boxed{\rho_D(t)=\begin{pmatrix}|a|^2&ab^*z(t)\\a^*b z(t)^*&|b|^2\end{pmatrix}},\qquad
z(t)=\langle E_1(t)|E_0(t)\rangle.
$$

The orientation of this [conditional environment overlap](../../../../../../conditional-environment-overlap.md) fixes the sign of the phase in the upper-right entry. Factorizing the overlap yields the [decoherence factor](../../../../../../decoherence-factor.md)

$$
\boxed{z(t)=\prod_{k=1}^N\left(|\alpha_k|^2e^{2ig_kt}+|\beta_k|^2e^{-2ig_kt}\right)
=\prod_{k=1}^N\left[\cos(2g_kt)+i\left(|\alpha_k|^2-|\beta_k|^2\right)\sin(2g_kt)\right]}.
$$

The populations are conserved because $[H,Z_D]=0$. Only phase coherence can be reduced. In particular,

$$
|z(t)|^2=\prod_k\left[1-4|\alpha_k|^2|\beta_k|^2\sin^2(2g_kt)\right]\leq1.
$$

[Quantum decoherence](../../../../../../quantum-decoherence.md) here results from distinguishable conditional bath states, although the complete system remains in a [pure state](../../../../../../pure-state.md) under [unitary time evolution](../../../../../../unitary-time-evolution.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
