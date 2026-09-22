<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Stack $y=(y_1^\top,y_2^\top)^\top$. After integrating out the [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md),

$$
y\mid t,\theta\sim N_{2N}(\mu_\theta,\Sigma_\theta),
\qquad
\mu_\theta=
\begin{pmatrix}c\mathbf1\\(c+\Delta m)\mathbf1\end{pmatrix}.
$$

Writing $k(a,b)=A^2e^{-|a-b|/\tau}$, the covariance blocks are

$$
(\Sigma_{11})_{jk}=k(t_j,t_k)+\sigma_{1,j}^2\mathbf1_{\{j=k\}},
$$



$$
(\Sigma_{22})_{jk}=k(t_j-\Delta t,t_k-\Delta t)+\sigma_{2,j}^2\mathbf1_{\{j=k\}},
$$

and $(\Sigma_{12})_{jk}=k(t_j,t_k-\Delta t)$, with $\Sigma_{21}=\Sigma_{12}^\top$. Therefore

$$
\boxed{p(y_1,y_2\mid t,\theta)
=(2\pi)^{-N}|\Sigma_\theta|^{-1/2}
\exp\left[-\frac12(y-\mu_\theta)^\top
\Sigma_\theta^{-1}(y-\mu_\theta)\right].}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
