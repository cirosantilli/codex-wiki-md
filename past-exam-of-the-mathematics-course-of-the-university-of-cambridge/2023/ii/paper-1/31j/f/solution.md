<h1 id="31j/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Using the harmless normalization $1/(2n)$, the [squared-loss empirical risk for linear prediction](../../../../../../squared-loss-empirical-risk-for-linear-prediction.md) is

$$
R_n(\beta)
=\frac1{2n}\sum_{i=1}^n(\beta^TX_i-Y_i)^2,
$$

with explicit [gradient](../../../../../../gradient.md)

$$
\boxed{
\nabla R_n(\beta)
=\frac1n\sum_{i=1}^n(\beta^TX_i-Y_i)X_i
}.
$$

Starting from any $\beta_0\in C$, [projected gradient descent](../../../../../../projected-gradient-descent.md) with step sizes $\eta_k>0$ is

$$
\widetilde\beta_{k+1}
=\beta_k-\eta_k\nabla R_n(\beta_k),
\qquad
\boxed{\beta_{k+1}=\pi_C(\widetilde\beta_{k+1})}.
$$

For a fully explicit update, write $\widetilde\beta_{k+1}=(u_k,t_k)$ and $\rho_k=\|u_k\|_2$. The projection from part (e) is

$$
\pi_C(u_k,t_k)=
\begin{cases}
(u_k,t_k),&\rho_k\leq t_k,\\
(0,0),&\rho_k\leq-t_k,\\
\displaystyle
\frac12\left(1+\frac{t_k}{\rho_k}\right)(u_k,\rho_k),
&\rho_k>|t_k|.
\end{cases}
$$

Every iterate therefore lies in the prescribed hypothesis class, and any convergent run under the standard convex-optimization step-size conditions targets its empirical-risk minimizer.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [31J](../../31j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
