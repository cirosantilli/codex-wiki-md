<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Using the [risk-neutral probability](../../../../risk-neutral-probability.md) $q=2/3$ from part [c](../c.md), the [stock](../../../../stock.md) tree has values $9$ initially, $12,6$ after one step, and $16,8,4$ after two. The [American put option](../../../../american-put-option.md) has terminal [financial payoffs](../../../../contingent-claim-payoff.md) $0,1,5$. Work backwards, comparing the immediate [exercise payoff](../../../../exercise-payoff.md) with its discounted continuation value.

At $S_1=12$, continuation is $(3/10)(2\cdot0+1)=3/10$, exceeding the zero exercise payoff. At $S_1=6$, continuation is $(3/10)(2\cdot1+5)=21/10$, while exercise pays three. Therefore **exercise at the down node $S_1=6$ and continue at $S_1=12$**. The initial exercise payoff is zero and the continuation value is

$$
\boxed{P_0=\frac3{10}\left(2\cdot\frac3{10}+3\right)=\frac{27}{25}=1.08.}
$$

The [Snell envelope](../../../../snell-envelope.md) gives this backwards maximum recursion. For comparison, restricting exercise to expiry would give $81/100$, so early exercise genuinely adds value.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
