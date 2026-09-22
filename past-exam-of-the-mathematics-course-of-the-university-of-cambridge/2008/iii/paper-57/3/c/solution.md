<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define [orthonormal](../../../../../../orthonormal-set.md) symmetric [vectors](../../../../../../vector.md)

$$
|s_0\rangle=|\widetilde0\rangle,\qquad |s_j\rangle=\frac{|\widetilde{-j}\rangle+|\widetilde j\rangle}{\sqrt2}\quad(1\leq j\leq N).
$$

The [symmetric-arm reduction of an exchange Hamiltonian](../../../../../../symmetric-arm-reduction-of-an-exchange-hamiltonian.md) here has two arms. To verify it directly, the link between radial distances $j$ and $j+1$ has strength $J_j$ on either side, while the two central links have strength $J_0/\sqrt2$. The calculation of part (a) therefore gives

$$
\begin{aligned}
H_e|s_0\rangle&=J_0|s_1\rangle,\\
H_e|s_j\rangle&=J_{j-1}|s_{j-1}\rangle+J_j|s_{j+1}\rangle\quad(1\leq j<N),\\
H_e|s_N\rangle&=J_{N-1}|s_{N-1}\rangle.
\end{aligned}
$$

In particular this subspace is invariant and contains the initial [vector](../../../../../../vector.md). Define the [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) $F|j\rangle=|s_j\rangle$. The displayed [matrix](../../../../../../matrix.md) entries prove $H_eF=FH_T$, or $F^\dagger H_eF=H_T$. Induction gives $H_e^mF=FH_T^m$ for every nonnegative integer $m$; hence the convergent exponential series proves $e^{-iH_et}F=Fe^{-iH_Tt}$. This establishes the mapping for the entire evolution, rather than just its first two powers. The supplied endpoint transfer also forces every $J_j$ to be nonzero, since a broken link would disconnect the two endpoints. Successive powers applied to $|s_0\rangle$ then generate all $|s_j\rangle$, so this is exactly the [cyclic subspace](../../../../../../cyclic-subspace.md) governing the initial state.

Using the stated [perfect quantum state transfer](../../../../../../perfect-quantum-state-transfer.md) identity at time $\pi/2$,

$$
\boxed{e^{-iH_e\pi/2}|\widetilde0\rangle=F|N\rangle=\frac{|\widetilde{-N}\rangle+|\widetilde N\rangle}{\sqrt2}.}
$$

The two terms have the excitation at sites $0$ and $2N$, respectively, and all intermediate [qubits](../../../../../../qubit.md) are zero in both terms. The full state thus factors into a [Bell state](../../../../../../bell-state-split.md) at the endpoints and the vacuum on the interior. Its [partial trace](../../../../../../partial-trace.md) is

$$
\boxed{\rho_{0,2N}=|\Psi^+\rangle\langle\Psi^+|,\qquad |\Psi^+\rangle=\frac{|10\rangle+|01\rangle}{\sqrt2}.}
$$

The coherent cross terms survive the trace because the interior [vectors](../../../../../../vector.md) coincide. We have used the transfer phase convention supplied in the question; a common transfer phase would leave this [density operator](../../../../../../density-matrix.md) unchanged.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
