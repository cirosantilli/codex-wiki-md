<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each fixed phase $\phi_k$, the single-transition [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) is $\Omega_k(t)H_k(\phi_k)$, so its generators at different times commute. Its exact propagator depends only on $\theta_k(t)=\hbar^{-1}\int_0^t\Omega_k(\tau)d\tau$. On the active two-level subspace, $H_k^2=I$; on the spectator state, $H_k=0$. Thus it is an [embedded two-level quantum rotation](../../../../../../embedded-two-level-quantum-rotation.md), not an involution on the whole three-dimensional space. Explicitly,

$$
\boxed{U_1=\begin{pmatrix}
\cos\theta_1&-ie^{-i\phi_1}\sin\theta_1&0\\
-ie^{i\phi_1}\sin\theta_1&\cos\theta_1&0\\
0&0&1
\end{pmatrix},\qquad
U_2=\begin{pmatrix}
1&0&0\\
0&\cos\theta_2&-ie^{-i\phi_2}\sin\theta_2\\
0&-ie^{i\phi_2}\sin\theta_2&\cos\theta_2
\end{pmatrix}.}
$$

The spectator entries in both matrices are exactly one; the converted TeX damages the second matrix, so these entries use the PDF.

The proposed combined exponential is **false in general** for two independent envelopes. Direct multiplication gives

$$
[H_1,H_2]=e^{-i(\phi_1+\phi_2)}E_{13}-e^{i(\phi_1+\phi_2)}E_{31}\ne0,
$$

so

$$
[H(t),H(s)]=[\Omega_1(t)\Omega_2(s)-\Omega_2(t)\Omega_1(s)][H_1,H_2].
$$

The [constant pulse-axis condition for removing time ordering](../../../../../../constant-pulse-axis-condition-for-removing-time-ordering.md) holds if both envelopes are proportional to the same function, but not for generic independent controls. For example, turn on only the first transition, then only the second. The result is $e^{-i\theta_2H_2}e^{-i\theta_1H_1}$, whose [Baker--Campbell--Hausdorff formula](../../../../../../baker-campbell-hausdorff-formula.md) includes a nonzero [commutator](../../../../../../commutator.md) correction, rather than simply $e^{-i(\theta_1H_1+\theta_2H_2)}$.

There is also a literal source defect: the PDF's right-hand exponent omits the factor $-i$ on its second term. With $\theta_1=0$ it would give $e^{\theta_2H_2}$, which has [eigenvalues](../../../../../../eigenvalue.md) $e^{\pm\theta_2}$ and is not unitary for real nonzero $\theta_2$, whereas the true propagator is unitary. Even after repairing that missing factor, [time ordering](../../../../../../time-ordering.md) is still necessary unless the [commutators](../../../../../../commutator.md) vanish.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
