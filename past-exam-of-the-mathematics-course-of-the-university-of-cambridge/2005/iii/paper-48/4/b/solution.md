<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $d(B_t^{-1})=-r_tB_t^{-1}dt$, multiplying the given bond dynamics by $B_t^{-1}$ cancels the drift and gives $dZ_t=Z_t\Sigma(t,T)dW_t^Q$. For an integrable discounted terminal payoff, the risk-neutral value process is the discounted-payoff [martingale](../../../../../../martingale-split.md)

$$
M_t=\mathbb E_Q[B_T^{-1}X\mid\mathcal F_t],\qquad V_t=B_tM_t.
$$

For an attainable claim this also follows directly from its self-financing discounted wealth being a true [martingale](../../../../../../martingale-split.md), with terminal value $B_T^{-1}X$. In a Brownian market, the [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) provides $dM_t=\psi_tdW_t^Q$; a traded bond with nonzero diffusion exposure can hedge it by holding $\psi_t/(Z_t\Sigma_t)$ bond units, with the remainder in the [bank account](../../../../../../bank-account.md). Thus, under the usual attainability and integrability assumptions, this construction gives the replicated price as well as the [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) formula.

Because $B_t$ is $\mathcal F_t$-measurable,

$$
\boxed{V_t=\mathbb E_Q\left[\exp\left(-\int_t^Tr_sds\right)X\,\middle|\,\mathcal F_t\right].}
$$

In a general [Heath-Jarrow-Morton model](../../../../../../heath-jarrow-morton-model.md), writing this value as $V(t,r_t)$ requires an additional state-reduction assumption. The [conditional expectation](../../../../../../conditional-expectation.md) is valid without asserting that the [short rate](../../../../../../short-rate.md) alone is the full state.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
