# Snell envelope of a multiplicative process

↑ **Parent:** [Snell envelope](snell-envelope.md)

Let $Y_t=Y_0\prod_{j=1}^tZ_j$, where $Y_0>0$ is deterministic and the positive factors are independent and integrable. Use the natural filtration. Its finite-horizon [Snell envelope](snell-envelope.md) is

$$
U_t=Y_tc_t,\qquad c_T=1,\qquad c_t=\max\{1,c_{t+1}\mathbb E Z_{t+1}\}.
$$

Indeed, backward induction and [independence of random variables](independent-random-variables.md) give $\mathbb E[U_{t+1}\mid\mathcal F_t]=Y_tc_{t+1}\mathbb E Z_{t+1}$; take the maximum with immediate exercise $Y_t$. The constants are finite and at least one. Equivalently, $c_t$ is the maximum of $1$ and the successive products $\prod_{j=t+1}^u\mathbb E Z_j$ for $t<u\le T$. If the factors have a common mean $\lambda>1$, waiting until maturity is optimal and $c_t=\lambda^{T-t}$. Integrability and [independence of random variables](independent-random-variables.md) from the current information are essential to the finite deterministic coefficient conclusion.

## ↑ Ancestors (7)

1. [Snell envelope](snell-envelope.md)
2. [Martingale](martingale-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [American quadratic-payoff option in a binomial market](american-quadratic-payoff-option-in-a-binomial-market.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/2/solution.md)
