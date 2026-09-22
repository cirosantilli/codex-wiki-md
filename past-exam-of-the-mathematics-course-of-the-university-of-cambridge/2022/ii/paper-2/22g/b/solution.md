<h1 id="22g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [compact operator](../../../../../../compact-operator-split.md) maps every bounded sequence to a sequence with a norm-convergent subsequence. A [Hilbertian basis](../../../../../../hilbertian-basis.md) is a complete orthonormal sequence.

If $T$ is compact and $\lambda_n$ does not tend to zero, some subsequence has  
$|\lambda_{n_j}|\geq\varepsilon$. The vectors  
$Te_{n_j}=\lambda_{n_j}e_{n_j}$ are pairwise separated by at least $\sqrt2\varepsilon$, so they have no convergent subsequence, a contradiction.

Conversely, if $\lambda_n\to0$, define the [finite-rank operator](../../../../../../finite-rank-operator.md)

$$
T_Ne_n=\begin{cases}\lambda_ne_n,&n\leq N,\\0,&n>N.\end{cases}
$$

Then

$$
\|T-T_N\|=\sup_{n>N}|\lambda_n|\longrightarrow0.
$$

An operator-norm limit of compact operators is compact, so $T$ is compact.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22G](../../22g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
