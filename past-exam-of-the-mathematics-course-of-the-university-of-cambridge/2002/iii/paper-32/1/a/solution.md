<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat each column as the payoff from one unit of initial investment, so the cost of holdings $h=(h_1,h_2,h_3)^t$ is $h_1+h_2+h_3$. The first asset weakly dominates the third at the same price, and so does the second. Long the first and short the third gives zero initial cost and terminal payoff $(0,0,2)^t$. Long the second and short the third gives payoff $(2,0,0)^t$, also at zero cost. These are [arbitrages](../../../../../../arbitrage.md) provided the displayed states have positive [probability](../../../../../../probability.md). Combining them gives the zero-cost position $(1,1,-2)^t$ with payoff $(2,0,2)^t$.

More generally, imposing zero cost means $h_3=-h_1-h_2$, and its payoff is $(2h_2,0,2h_1)^t$. Thus every $h_1,h_2\ge0$ with at least one positive gives a [pure-investment arbitrage](../../../../../../pure-investment-arbitrage.md). **The market is not arbitrage-free.**

There is nevertheless no [arbitrage](../../../../../../arbitrage.md) of the other requested kind, with every future net cash flow identically zero. Indeed the middle-state payoff is $2(h_1+h_2+h_3)$, so a zero terminal payoff already forces zero initial cost. The other two states then force $h_1=h_2=0$, hence $h_3=0$. Equivalently, the return matrix has [determinant](../../../../../../determinant.md) $8$ and is invertible. Therefore

$$
\boxed{\text{Zero-cost positive future payoffs exist; a positive receipt now with zero future payoff does not.}}
$$

The unique vector pricing the three unit-investment payoffs is $(0,\tfrac12,0)^t$. It is nonnegative but not strictly positive. This illustrates why [nonnegative state prices need not exclude arbitrage](../../../../../../nonnegative-state-prices-need-not-exclude-arbitrage.md): strictly positive state prices would assign positive cost to either of the nonzero nonnegative payoffs above.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
