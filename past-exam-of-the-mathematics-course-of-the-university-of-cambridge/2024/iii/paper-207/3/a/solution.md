<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $K\in\mathbb R^{n\times n}$ have entries $K_{ij}=\kappa(x_i,x_j)$, let $k_*\in\mathbb R^n$ have entries $(k_*)_i=\kappa(x_i,x_*)$, and let $k_{**}=\kappa(x_*,x_*)$. The [Gaussian process](../../../../../../gaussian-process.md) prior and independent [Gaussian noise](../../../../../../gaussian-noise.md) imply

$$
\begin{pmatrix}f(x_*)\\y\end{pmatrix}
\sim N\!\left[
\begin{pmatrix}0\\0_n\end{pmatrix},
\begin{pmatrix}
k_{**}&k_*^T\\
k_*&K+\sigma^2I_n
\end{pmatrix}
\right].
$$

Applying the [conditional multivariate normal distribution](../../../../../../conditional-multivariate-normal-distribution.md) gives the [Gaussian process regression posterior](../../../../../../gaussian-process-regression-posterior.md)

$$
f(x_*)\mid y,X,x_*
\sim N(m_*,v_*),
$$

where

$$
m_*=k_*^T(K+\sigma^2I_n)^{-1}y,
\qquad
v_*=k_{**}-k_*^T(K+\sigma^2I_n)^{-1}k_*.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
