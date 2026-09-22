<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $\rho$. For an observation with covariates $x$, put

$$
u=-x^T\alpha,
\qquad
v_a=-a\beta-x^T\gamma,
$$

and let $\Phi$ be the standard-normal distribution function. The four conditional cell probabilities are

$$
\begin{aligned}
p_{00}(x)&=F_\rho(u,v_0),\\
p_{01}(x)&=\Phi(u)-F_\rho(u,v_0),\\
p_{10}(x)&=\Phi(v_1)-F_\rho(u,v_1),\\
p_{11}(x)&=1-\Phi(u)-\Phi(v_1)+F_\rho(u,v_1),
\end{aligned}
$$

where the first index is $A$ and the second is $Y$.

Define $(\widehat\alpha_\rho,\widehat\beta_\rho,\widehat\gamma_\rho)$ as any maximizer of the [log likelihood](../../../../../../../maximum-likelihood-estimation.md)

$$
\sum_{i=1}^n\sum_{a,y\in\{0,1\}}
\mathbf1_{\{A_i=a,Y_i=y\}}\log p_{ay}(X_i).
$$

Then $\widehat\beta_\rho$ is the requested estimator for the fixed sensitivity value $\rho$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 221](../../../../paper-221-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
