<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
M_t=\mathbb E[Y_T\xi_T\mid\mathcal F_t],
\qquad V_t=\frac{M_t}{Y_t}.
$$

The boundedness of $\xi_T$ and positivity of the deflator make $M$ a nonnegative true martingale. By the [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md), $dM_t=\eta_t dW_t$. A self-financing wealth process with stock holding $\pi_t$ satisfies

$$
dV_t=\{r_tV_t+\pi_tS_t(\mu_t-r_t)\}dt
+\pi_tS_t\sigma_t dW_t.
$$

The product $YV$ then has diffusion coefficient

$$
Y_t(\pi_tS_t\sigma_t-V_t\lambda_t).
$$

Choose

$$
\pi_t=\frac{\eta_t/Y_t+V_t\lambda_t}{S_t\sigma_t},
\qquad
\phi_t=\frac{V_t-\pi_tS_t}{B_t}.
$$

Then $Y_tV_t=M_t$, so $V_T=\xi_T$ and the strategy replicates the claim. It is admissible because $V=M/Y$ is nonnegative.

For any other admissible replicating wealth $\widetilde V$, the nonnegative local martingale $Y\widetilde V$ is a supermartingale. Hence

$$
\widetilde V_0\geq\mathbb E[Y_T\widetilde V_T]
=\mathbb E[Y_T\xi_T].
$$

The constructed strategy has

$$
\boxed{V_0=\phi_0B_0+\pi_0S_0
=\mathbb E[Y_T\xi_T],}
$$

so this is the minimal replication cost.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
