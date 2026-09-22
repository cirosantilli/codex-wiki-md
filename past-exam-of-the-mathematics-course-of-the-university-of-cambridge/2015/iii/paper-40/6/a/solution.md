<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Normalize $B_0=1$ and put $\widetilde S_t=e^{-rt}S_t$. Its dynamics are $d\widetilde S_t=\widetilde S_t\sigma(t,S_t)\,dW_t$. Bounded volatility makes this [stochastic exponential](../../../../../../doleans-dade-exponential.md) a true [martingale](../../../../../../martingale-split.md) on each finite horizon, by the [Novikov condition](../../../../../../novikov-s-condition.md). It also gives a finite second moment: stopping the [Itô formula](../../../../../../ito-s-lemma.md) for $S^2$ and applying the [Gronwall inequality](../../../../../../gronwall-inequality.md) yields $\mathbb E S_T^2\leq S_0^2e^{(2r+L^2)T}$ when $\sigma\leq L$.

The discounted payoff $\xi=e^{-rT}(S_T-K)^+$ is thus square-integrable. Define the nonnegative [martingale](../../../../../../martingale-split.md)

$$
M_t=\mathbb E[\xi\mid\mathcal F_t],\qquad M_0=C(T,K).
$$

The [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) says that every square-integrable martingale in the Brownian filtration has a representation $M_t=M_0+\int_0^th_u\,dW_u$ with predictable $h$ and $\mathbb E\int_0^Th_u^2du<\infty$. Since $\widetilde S>0$ and $\sigma>0$, choose

$$
\boxed{\pi_t=\frac{h_t}{\widetilde S_t\sigma(t,S_t)},\qquad
\phi_t=M_t-\pi_t\widetilde S_t.}
$$

Then discounted gains satisfy $dM_t=\pi_t\,d\widetilde S_t$. Consequently $X_t=B_tM_t=\phi_tB_t+\pi_tS_t$ is [self-financing](../../../../../../self-financing-portfolio.md), nonnegative, and hence an [admissible trading strategy](../../../../../../admissible-trading-strategy.md). At maturity $X_T=(S_T-K)^+$, proving [claim replication](../../../../../../claim-replication.md) at cost $C(T,K)$.

For minimality, discounted wealth of any admissible [self-financing portfolio](../../../../../../self-financing-portfolio.md) is a [local martingale](../../../../../../local-martingale.md) bounded below, hence a [supermartingale](../../../../../../supermartingale.md) by localization and the conditional [Fatou lemma](../../../../../../fatou-s-lemma.md). Thus any such replication with initial wealth $x$ obeys

$$
x\geq\mathbb E[e^{-rT}X_T]=C(T,K).
$$

Together with the constructed portfolio, this proves

$$
\boxed{\text{minimal admissible replication cost}=C(T,K).}
$$

This is [Brownian representation replication in a local volatility market](../../../../../../brownian-representation-replication-in-a-local-volatility-market.md). The given drift $r$ means that the original probability measure already serves as the [risk-neutral measure](../../../../../../risk-neutral-measure.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
