<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Arrange the amplitudes of $|\phi_1\rangle$ as the matrix

$$
C_1=\begin{pmatrix}a&b\\c&d\end{pmatrix}.
$$

The second state has $C_2=C_1X$, where $X$ swaps the $A_2$ basis states. If Bob receives $A_1$, his two [reduced density matrices](../../../../../../../reduced-density-matrix.md) are

$$
\rho_{A_1}^{(1)}=C_1C_1^\dagger,
\qquad
\rho_{A_1}^{(2)}=C_2C_2^\dagger
=C_1XX^\dagger C_1^\dagger,
$$

and are identical. No measurement on $A_1$ contains any information about the shared state.

If Bob instead receives $A_2$,

$$
\rho_{A_2}^{(1)}
=\begin{pmatrix}
a^2+c^2&ab+cd\\
ab+cd&b^2+d^2
\end{pmatrix},
\qquad
\rho_{A_2}^{(2)}=X\rho_{A_2}^{(1)}X.
$$

They differ because $a^2+c^2<b^2+d^2$. Bob can therefore distinguish them with better-than-random success. For equal priors,

$$
\boxed{D(\rho_{A_2}^{(1)},\rho_{A_2}^{(2)})
=b^2+d^2-a^2-c^2},
$$

so the optimal success probability is $\frac12(1+D)$. It is generally below one, so a single copy does not permit certain identification.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
