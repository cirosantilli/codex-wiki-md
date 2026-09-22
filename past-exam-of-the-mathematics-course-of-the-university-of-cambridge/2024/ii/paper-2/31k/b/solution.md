<h1 id="31k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $m_i=\mathbb E(Y_i\mid X_i)$. Conditional on $X_{1:n}$,

$$
\gamma_j=\frac1{N_j+1}\sum_i
m_i\mathbf1_{\widehat R_j}(X_i).
$$

The responses are conditionally independent, so cross-covariances vanish and

$$
\boxed{
\mathbb E[(\widetilde\gamma_j-\gamma_j)^2\mid X_{1:n}]
=\frac1{(N_j+1)^2}\sum_i
\operatorname{Var}(Y_i\mid X_i)
\mathbf1_{\widehat R_j}(X_i)}.
$$

Because the regions partition predictor space,

$$
\widetilde T(X)-\mathbb E(\widetilde T(X)\mid X,X_{1:n})
=\sum_j\mathbf1_{\widehat R_j}(X)
(\widetilde\gamma_j-\gamma_j).
$$

Only one summand is nonzero. Put  
$q_j=\mathbb P(X\in\widehat R_j)$; the partition is deterministic because $D'$ is fixed, and $N_j\sim\operatorname{Bin}(n,q_j)$. The variance bound and  
$N_j/(N_j+1)^2\leq1/(N_j+1)$ give

$$
\begin{aligned}
\mathbb E[\{\widetilde T(X)-\mathbb E(\widetilde T(X)\mid X,X_{1:n})\}^2]
&\leq\sigma^2\sum_jq_j\,
\mathbb E\frac1{N_j+1}\\
&\leq\sigma^2\sum_{j:q_j>0}\frac1n
\leq\boxed{\frac{\sigma^2J}{n}}.
\end{aligned}
$$

This is the [conditional variance of a fixed regression-tree partition](../../../../../../conditional-variance-of-a-fixed-regression-tree-partition.md) bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31K](../../31k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
