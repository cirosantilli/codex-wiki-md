<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $d_1>d_2$, buy $1/100$ of stock 1 and sell $1/100$ of stock 2. Initial cost is zero; the one-period payoff is $u_1-u_2>0$ in the up state and $d_1-d_2>0$ in the down state. This is an [arbitrage](../../../../../arbitrage.md). If terminal rather than time-one arbitrage is required, reinvest the positive receipts in either positive-price stock.

For $d_1<d_2$, define the one-period [Arrow state prices](../../../../../arrow-debreu-state-price.md)

$$
\pi_u=\frac{d_2-d_1}{u_1d_2-u_2d_1},\qquad
\pi_d=\frac{u_1-u_2}{u_1d_2-u_2d_1}.
$$

The denominator is positive because $u_1/u_2>1>d_1/d_2$. Both state prices are strictly positive and satisfy $\pi_u u_i+\pi_d d_i=1$ for $i=1,2$. Thus every portfolio's present value equals the positive state-price-weighted value of its two future payoffs.

Use the same strictly positive pricing rule at every node of the two-period tree. A nonnegative terminal payoff that is positive in at least one state has strictly positive price by backward induction, so a zero-cost [self-financing strategy](../../../../../self-financing-portfolio.md) cannot generate an arbitrage. Therefore **the market is arbitrage free when $d_1<d_2$**, despite having no initially supplied bond. This is a [two-stock binomial market without a supplied bond](../../../../../two-stock-binomial-market-without-a-supplied-bond.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
