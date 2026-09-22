<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $V=(X_1(t_1),X_1(t_2))^T$. The [Karhunen–Loève expansion](../../../../../../karhunen-loeve-expansion.md) and Gaussianity give

$$
\operatorname{Cov}(a_{1k},V)
=\lambda_k(\phi_k(t_1),\phi_k(t_2))
$$

and

$$
\operatorname{Cov}(V)=
\Sigma=
\begin{pmatrix}
c_X(t_1,t_1)&c_X(t_1,t_2)\\
c_X(t_2,t_1)&c_X(t_2,t_2)
\end{pmatrix}.
$$

The [conditional multivariate normal distribution](../../../../../../conditional-multivariate-normal-distribution.md) formula yields

$$
\boxed{
\mathbb E[a_{1k}\mid X_1(t_1),X_1(t_2)]
=\lambda_k(\phi_k(t_1),\phi_k(t_2))
\Sigma^{-1}
\begin{pmatrix}X_1(t_1)\\X_1(t_2)\end{pmatrix}}.
$$

If $\Sigma$ is singular, the same formula uses its Moore-Penrose pseudoinverse.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
