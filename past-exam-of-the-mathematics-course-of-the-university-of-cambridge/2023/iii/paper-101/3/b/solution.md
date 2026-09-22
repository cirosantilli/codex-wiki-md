<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose finite generating sets $I=(g_1,\ldots,g_s)$ and $J=(f_1,\ldots,f_t)$, using the [Hilbert basis theorem](../../../../../../hilbert-basis-theorem.md). The assumed inclusion says that each $f_j$ vanishes on $V_{\mathbb C}(I)$. By the [Strong Hilbert Nullstellensatz](../../../../../../strong-hilbert-nullstellensatz.md), for every $j$ there is an exponent $N_j$ such that

$$
f_j^{N_j}\in I\mathbb C[T_1,\ldots,T_n].
$$

The coefficients in an expression $f_j^{N_j}=\sum_iq_{ij}g_i$ solve a finite [system of linear equations](../../../../../../system-of-linear-equations.md) with rational coefficients. Since it has a complex solution, [Gaussian elimination](../../../../../../gaussian-elimination.md) gives a rational solution. Clearing the finitely many denominators produces a nonzero integer $D$ such that

$$
D f_j^{N_j}\in I
$$

for every $j$.

For any prime $p\nmid D$, reduce these identities modulo $p$. At a common zero of $\pi_p(I)$ in the [algebraic closure](../../../../../../algebraic-closure.md) $\overline{\mathbb F}_p$, they give $\pi_p(f_j)^{N_j}=0$, hence $\pi_p(f_j)=0$, for all $j$. Therefore

$$
V_{\overline{\mathbb F}_p}(\pi_p(I))
\subseteq
V_{\overline{\mathbb F}_p}(\pi_p(J))
$$

for every prime except the finitely many divisors of $D$. This is the [spreading out of an affine zero-set inclusion](../../../../../../spreading-out-of-an-affine-zero-set-inclusion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
