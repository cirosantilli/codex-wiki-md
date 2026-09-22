<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $c$ be the initial call price. Write the risk-neutral [probabilities](../../../../../../probability.md) of stock prices $5,3,2$ as $q_5,q_3,q_2$. The stock's [martingale](../../../../../../martingale-split.md) equation and the normalization give $q_2=2q_5$ and $q_3=1-3q_5$. The call pays only in the first state, so its [martingale](../../../../../../martingale-split.md) equation is $q_5=c$. Thus

$$
(q_5,q_3,q_2)=(c,1-3c,2c).
$$

All three objective [probabilities](../../../../../../probability.md) are positive. This defines an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) precisely when $0<c<1/3$, and part (iii) proves that every such price excludes [arbitrage](../../../../../../arbitrage.md).

To prove necessity without appealing to an existence theorem, consider the other prices explicitly. If $c\leq0$, buy one call and hold $-c$ units of cash. Its initial value is zero and terminal value is $(S_1-4)^+-c$, nonnegative and positive with positive [probability](../../../../../../probability.md). If $c\geq1/3$, take holdings $(h_B,h_S,h_C)=(c-1,1/3,-1)$. The initial value is $c-1+1-c=0$ and terminal values at $5,3,2$ are $(c-1/3,c,c-1/3)$. They are nonnegative and the middle-state value is strictly positive. This includes the endpoint $c=1/3$. Consequently

$$
\boxed{\text{the arbitrage-free call prices are exactly }c\in(0,1/3).}
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
