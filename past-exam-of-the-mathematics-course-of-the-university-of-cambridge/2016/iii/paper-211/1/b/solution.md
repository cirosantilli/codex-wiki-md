<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $h=T-t$. Conditional on $\mathcal F_t^S$, [independent increments](../../../../../../independent-increments.md) of the [Brownian motion](../../../../../../brownian-motion-split.md) give

$$
S_T=S_t\exp\{-\sigma^2h/2+\sigma\sqrt h\,Y\},
\qquad Y\sim N(0,1),
$$

where $Y$ has the [standard normal distribution](../../../../../../standard-normal-distribution.md) and is [independent](../../../../../../independent-random-variables.md) of $\mathcal F_t^S$. Factoring $S_t$ out of the positive part identifies the [normalized Black-Scholes call function](../../../../../../normalized-black-scholes-call-function.md):

$$
\mathbb E[(S_T-K)^+\mid\mathcal F_t^S]
=S_t F(\sigma^2h,K/S_t)=C_t.
$$

The [European call option](../../../../../../european-call-option.md) payoff is [integrable](../../../../../../integrability.md), because $0\leq(S_T-K)^+\leq S_T$ and $\mathbb E S_T=S_0$. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) therefore proves that $C$ is a true [martingale](../../../../../../martingale-split.md). At $t=T$, the boundary value $F(0,m)=(1-m)^+$ gives $C_T=(S_T-K)^+$. **The answer is the conditional payoff martingale**

$$
\boxed{C_t=\mathbb E[(S_T-K)^+\mid\mathcal F_t^S].}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
