<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $q_{15},q_{12},q_9$ for the state probabilities under an [equivalent martingale measure](../../../../../../risk-neutral-measure.md). Since cash is constant and the [European put option](../../../../../../european-put-option.md) pays only in the lowest state, the pricing equations are

$$
q_{15}+q_{12}+q_9=1,\qquad15q_{15}+12q_{12}+9q_9=10,\qquad2q_9=\xi_0.
$$

Their unique solution is $q_9=\xi_0/2$, $q_{15}=\xi_0/2-2/3$, $q_{12}=5/3-\xi_0$. Every physical state has positive [probability](../../../../../../probability.md), so equivalence requires all three values to be strictly positive. Thus

$$
\boxed{\frac43<\xi_0<\frac53.}
$$

For each price in this open interval the [pricing kernel](../../../../../../state-price-density.md) takes values $3q_{15},3q_{12},3q_9$ in the three equally likely states, proving absence of [arbitrage](../../../../../../arbitrage.md).

The necessity, including the exclusion of endpoints, can also be checked directly. The three terminal payoff vectors of cash, the [stock](../../../../../../stock.md) and the [European put option](../../../../../../european-put-option.md) form the invertible matrix

$$
\begin{pmatrix}1&15&0\\1&12&0\\1&9&2\end{pmatrix},\qquad\det=-6.
$$

Each unit state payoff therefore has a [replicating strategy](../../../../../../replicating-strategy.md), whose initial cost is the corresponding $q$. A zero or negative $q$ supplies an [arbitrage](../../../../../../arbitrage.md), so the endpoints are genuinely excluded.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
