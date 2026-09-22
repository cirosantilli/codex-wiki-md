<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use logarithms to base two, so all [Von Neumann entropies](../../../../../../von-neumann-entropy-split.md) and [Shannon entropies](../../../../../../information-entropy.md) are measured in bits. Write the nonzero [eigenvalues](../../../../../../eigenvalue.md) of $\rho_i$ as $\lambda_{ij}$. Orthogonality of the supports makes the mixture a [block diagonal matrix](../../../../../../block-diagonal-matrix.md), with eigenvalues $p_i\lambda_{ij}$. Therefore

$$
\begin{aligned}
S(\rho)&=-\sum_{i,j}p_i\lambda_{ij}\log_2(p_i\lambda_{ij})\\
&=-\sum_i p_i\log_2p_i\sum_j\lambda_{ij}
-\sum_i p_i\sum_j\lambda_{ij}\log_2\lambda_{ij}\\
&=\boxed{H(p)+\sum_i p_iS(\rho_i)}.
\end{aligned}
$$

Each $\rho_i$ has [trace](../../../../../../matrix-trace.md) one. Terms with zero probability or zero eigenvalue vanish under the convention $0\log0=0$. This proves the [entropy of an orthogonal quantum mixture](../../../../../../entropy-of-an-orthogonal-quantum-mixture.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
