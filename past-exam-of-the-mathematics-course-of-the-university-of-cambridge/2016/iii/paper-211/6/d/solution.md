<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the original measure as the [risk-neutral measure](../../../../../../risk-neutral-measure.md) for this zero-interest model, or interpret $S$ as a discounted [stock](../../../../../../stock.md) price. **$\xi_t$ is the arbitrage-free value of the European contingent claim with payoff $g(S_T)$**, and **$\pi_t$ is its option delta and replicating stock holding**. Part (b) supplies the [self-financing portfolio](../../../../../../self-financing-portfolio.md):

$$
\boxed{\text{stock holding }\pi_t=V_S(t,S_t),\qquad
\text{cash holding }\xi_t-\pi_tS_t.}
$$

With the cash asset identically one, its value is $\xi_t$ and its gains satisfy $d\xi_t=\pi_t\,dS_t$, so it exactly replicates $g(S_T)$. This [delta hedge](../../../../../../delta-hedge.md) is admissible since the assumed nonnegative $V$ gives nonnegative wealth. In this continuous-path setting the holdings can be taken [predictable](../../../../../../predictable-process.md).

The auxiliary [change of measure](../../../../../../change-of-measure.md) in part (c) expresses the [option delta](../../../../../../option-delta.md) as an [expectation](../../../../../../expected-value.md) of terminal payoff sensitivity. It changes the [stock](../../../../../../stock.md) drift to $aa'$ and is generally not the original [risk-neutral measure](../../../../../../risk-neutral-measure.md) for the zero-interest stock market. Its role is to value sensitivity under the tilted state dynamics, while the actual [replicating strategy](../../../../../../replicating-strategy.md) trades under the original dynamics. No general claim of [market completeness](../../../../../../complete-market.md) is needed, including when $a$ can vanish.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
