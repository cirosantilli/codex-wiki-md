<h1 id="28i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An arbitrage is a portfolio with nonpositive initial cost, nonnegative terminal payoff [almost surely](../../../../../../almost-sure-convergence.md) and a positive payoff with positive [probability](../../../../../../probability.md), allowing unused initial cash to be invested in the riskless asset. Equivalently it is a zero-cost portfolio with those terminal properties. An [equivalent martingale measure](../../../../../../risk-neutral-measure.md) $Q$ has the same [null sets](../../../../../../null-set.md) as the physical [measure](../../../../../../measure.md) and satisfies $E_Q[S_1^i]=(1+r)S_0^i$ for every traded asset, with appropriate integrability.

For an agent with differentiable increasing concave utility and an optimal portfolio, let $W^*$ be its terminal wealth. The [first-order conditions](../../../../../../first-order-optimality-condition.md) for variations in risky holdings are $E[U'(W^*)(S_1^i-(1+r)S_0^i)]=0$. If $U'(W^*)>0$ and integrable, normalize it to the [probability density](../../../../../../probability-density.md) $Z=U'(W^*)/E[U'(W^*)]$. The [first-order conditions](../../../../../../first-order-optimality-condition.md) make $Q$ with $dQ=Z\,dP$ an [equivalent martingale measure](../../../../../../risk-neutral-measure.md). A small additional payoff $H$ then has marginal price

$$
\boxed{p(H)=\frac{E[U'(W^*)H]}{(1+r)E[U'(W^*)]}=\frac{E_QH}{1+r}.}
$$

This follows by setting the [first variation](../../../../../../first-variation.md) of expected utility for buying a small claim at price $p$ equal to zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28I](../../28i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
