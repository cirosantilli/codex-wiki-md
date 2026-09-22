<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the maturity horizon. Since $YB$ is a nonnegative [local martingale](../../../../../../local-martingale.md) and $r$ is bounded, $\mathbb EY_T<\infty$: $B_T\geq B_0e^{-\|r\|_\infty T}$ and $\mathbb E(Y_TB_T)\leq B_0$. The bounded nonnegative payoff thus makes $Y_T\xi_T$ integrable. Set

$$
N_t=\mathbb E[Y_T\xi_T\mid\mathcal F_t],\qquad X_t=\frac{N_t}{Y_t}.
$$

The [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) yields $N_t=N_0+\int_0^t\zeta_s\,dW_s$, using its locally [square-integrable](../../../../../../square-integrable-function.md) version for an integrable terminal [random variable](../../../../../../random-variable-split.md). The [Itô formula](../../../../../../ito-s-lemma.md) for $N/Y$ gives

$$
dX_t=\bigl(r_tX_t+\lambda_t(\zeta_t/Y_t+\lambda_tX_t)\bigr)dt+(\zeta_t/Y_t+\lambda_tX_t)\,dW_t.
$$

Choose the [replicating strategy](../../../../../../replicating-strategy.md)

$$
\boxed{\theta_t=\frac{\zeta_t/Y_t+\lambda_tX_t}{S_t\sigma_t},\qquad\eta_t=\frac{X_t-\theta_tS_t}{B_t}.}
$$

Its [self-financing portfolio](../../../../../../self-financing-portfolio.md) equation has exactly the displayed [drift](../../../../../../drift-coefficient.md) and diffusion, because $\mu-r=\sigma\lambda$. All coefficients are locally integrable after stopping; the holdings are [predictable](../../../../../../predictable-process.md) in the augmented [natural Brownian filtration](../../../../../../natural-brownian-filtration.md). This construction has $X_t\geq0$ and $X_T=\xi_T$, so it is an admissible [replicating strategy](../../../../../../replicating-strategy.md) under the question's nonnegative-wealth convention.

For any other nonnegative [self-financing portfolio](../../../../../../self-financing-portfolio.md) $\widehat X$ replicating the same payoff, part (b) implies $\widehat X_0\geq\mathbb E[Y_T\xi_T]$. The constructed strategy attains equality, since $Y_0=1$ and $N_0=\mathbb E[Y_T\xi_T]$ in the augmented [natural Brownian filtration](../../../../../../natural-brownian-filtration.md). Hence

$$
\boxed{\text{minimal initial cost}=\mathbb E[Y_T\xi_T].}
$$

This is [deflator-based claim replication](../../../../../../deflator-based-claim-replication.md); it does not require upgrading the [local martingale deflator](../../../../../../local-martingale-deflator.md) to a true [martingale](../../../../../../martingale-split.md) density.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
