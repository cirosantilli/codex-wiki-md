<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Model the environment's vacuum and one-photon states by $|0_E\rangle,|1_E\rangle$. A [unitary dilation of amplitude damping](../../../../../../unitary-dilation-of-amplitude-damping.md) acts on the initially vacant environment as

$$
U|0,0_E\rangle=|0,0_E\rangle,\qquad U|1,0_E\rangle=\sqrt{1-p}|1,0_E\rangle+\sqrt p|0,1_E\rangle.
$$

These images are orthonormal. One unitary completion takes $U|0,1_E\rangle=-\sqrt p|1,0_E\rangle+\sqrt{1-p}|0,1_E\rangle$ and fixes $|1,1_E\rangle$. Taking environment matrix elements $\langle k_E|U|0_E\rangle$ gives $K_0,K_1$.

Evolve $\rho\otimes|0_E\rangle\langle0_E|$ by $U$ and take the [partial trace](../../../../../../partial-trace.md) over the environment. Orthogonality of the two environment records removes the cross-branch terms, giving $\mathcal A_p(\rho)=K_0\rho K_0^\dagger+K_1\rho K_1^\dagger$. Entrywise,

$$
\boxed{\mathcal A_p(\rho)=\begin{pmatrix}\rho_{00}+p\rho_{11}&\sqrt{1-p}\,\rho_{01}\\\sqrt{1-p}\,\rho_{10}&(1-p)\rho_{11}\end{pmatrix}.}
$$

Excited population is transferred to the ground state, while coherence is reduced by the square root of the survival probability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
