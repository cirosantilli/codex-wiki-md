<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $R=e^r$, $u=4/3$ and $d=2/3$. Since both moves have positive physical [probability](../../../../probability.md), the [binomial options pricing model](../../../../binomial-options-pricing-model.md) is free of [arbitrage](../../../../arbitrage.md) exactly when

$$
\boxed{\frac23<e^r<\frac43.}
$$

If $R\leq d$, borrowing the share price and buying one share gives terminal gain $S_t(u-R)$ or $S_t(d-R)$, both nonnegative and at least one positive. If $R\geq u$, shorting one share and investing its proceeds gives the opposite comparison, with gain $S_t(R-u)$ or $S_t(R-d)$. Equality at either endpoint still permits [arbitrage](../../../../arbitrage.md) because the other outcome has positive [probability](../../../../probability.md).

Conversely, strict inequalities give a [risk-neutral probability](../../../../risk-neutral-probability.md) $q=(R-d)/(u-d)\in(0,1)$, for which the discounted share is a [martingale](../../../../martingale-split.md). Any zero-cost [self-financing portfolio](../../../../self-financing-portfolio.md) with nonnegative terminal value has zero discounted [expectation](../../../../expected-value-split.md) under this equivalent positive-probability law and hence cannot have a strictly positive payoff in either state. Applying this argument conditionally at each node proves [no-arbitrage](../../../../no-arbitrage.md) over the tree.

## ↑ Ancestors (12)

1. [A](../a.md)
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
