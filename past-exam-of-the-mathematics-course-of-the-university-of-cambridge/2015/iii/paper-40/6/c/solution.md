<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) argument in part (a) also replicates the bounded put payoff. The discounted [stock](../../../../../../stock.md) is a true [martingale](../../../../../../martingale-split.md), so the elementary terminal payoff identity yields [put-call parity](../../../../../../put-call-parity.md)

$$
\boxed{P(T,K)=C(T,K)-S_0+Ke^{-rT}.}
$$

Set $H(T,K)=-S_0+Ke^{-rT}$. Then $H_T=-rKe^{-rT}$, $H_K=e^{-rT}$, and $H_{KK}=0$. Thus

$$
H_T=\frac12K^2\sigma(T,K)^2H_{KK}-rKH_K.
$$

Linearity of the [Dupire equation](../../../../../../dupire-equation.md) and $P=C+H$ give

$$
\boxed{P_T(T,K)=\frac12K^2\sigma(T,K)^2P_{KK}(T,K)-rKP_K(T,K).}
$$

The initial payoff is $P(0,K)=(K-S_0)^+$, and $P(T,0)=0$. Therefore calls and puts obey the same maturity-strike differential equation, with their respective initial and boundary data.

## ↑ Ancestors (11)

1. [C](../c.md)
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
