<h1 id="20f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the two-dimensional span of the first two [energy eigenstates](../../../../../../energy-eigenstate.md), the measured [observable](../../../../../../observable.md) has matrix $S=\begin{pmatrix}7&24\\24&-7\end{pmatrix}$. Its square is $625I$, and its trace is zero, giving [eigenvalues](../../../../../../eigenvalue.md) $25,-25$. The orthogonal complement has eigenvalue zero. Thus the full spectrum is $\boxed{\{-25,0,25\}}$.

The normalized eigenstates for $-25$ and $25$ are respectively

$$
\chi_- =\frac{3\psi_1-4\psi_2}{5},\qquad \chi_+=\frac{4\psi_1+3\psi_2}{5}.
$$

The lowest measurement outcome prepares $\chi_-$ up to an irrelevant overall phase. The subsequent [unitary time evolution](../../../../../../unitary-time-evolution.md) gives

$$
\chi_-(t)=\frac35e^{-iE_1t/\hbar}\psi_1-\frac45e^{-iE_2t/\hbar}\psi_2.
$$

By the [Born rule](../../../../../../born-rule.md), the probability of measuring the lowest eigenvalue again is the squared projection onto its one-dimensional [eigenspace](../../../../../../eigenspace.md):

$$
\begin{aligned}
P_-&=|\langle\chi_-,\chi_-(t)\rangle|^2=\left|\frac9{25}e^{-iE_1t/\hbar}+\frac{16}{25}e^{-iE_2t/\hbar}\right|^2\\
&=\boxed{\frac{337+288\cos((E_1-E_2)t/\hbar)}{625}}.
\end{aligned}
$$

This is the [two-level quantum return probability](../../../../../../two-level-quantum-return-probability.md) with $q=9/25$. At $t=0$ the probability is one; if the two energies happen to be equal it remains one for every time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
