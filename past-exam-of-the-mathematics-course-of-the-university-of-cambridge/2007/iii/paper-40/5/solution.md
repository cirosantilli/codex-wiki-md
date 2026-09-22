<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The resulting [revenue comparison for two uniform private values](../../../../../revenue-comparison-for-two-uniform-private-values.md) is

$$
\boxed{\frac5{12}>\frac{2}{3\sqrt3}>\frac13.}
$$

Thus the optimally reserved ascending auction is best, followed by the optimal [posted price](../../../../../posted-price.md), followed by the ascending auction without a reserve. These values are in the normalized monetary units used for the valuations.

The [revenue equivalence](../../../../../revenue-equivalence.md) theorem for symmetric independent private values applies to mechanisms with the same allocation probabilities at every type and the same expected utility for the lowest type, under the usual incentive and risk-neutrality assumptions. The reserved and unreserved auctions have different allocation rules. Without a reserve, a bidder of valuation $v$ wins with probability $G(v)=v$. With reserve $r$, that probability is zero for $v<r$ and $v$ for $v>r$. In particular the car is withheld when even the highest valuation is below $r$.

The [interim payment identity](../../../../../interim-payment-identity.md) makes the difference explicit. With lowest-type utility zero, the ordinary auction has expected payment $m(v)=v^2/2$. The reserved auction has

$$
m_r(v)=\begin{cases}0,&v<r,\\(v^2+r^2)/2,&v>r.\end{cases}
$$

Summing the two bidders' ex ante payments gives $2\int_r^1m_r(v)\,dv=1/3+r^2-4r^3/3$, exactly the revenue calculated above. Hence there is **no conflict with [revenue equivalence](../../../../../revenue-equivalence.md): its equal-allocation hypothesis does not hold**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
