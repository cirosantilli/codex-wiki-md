<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The common [short-rate market price of risk](../../../../../../short-rate-market-price-of-risk.md) follows from absence of [arbitrage](../../../../../../arbitrage.md), with the securities driven by the same [Brownian motion](../../../../../../brownian-motion-split.md). Take two traded derivatives $V_1,V_2$ with drifts $m_1,m_2$ and diffusion coefficients $s_1,s_2$. At a given state hold $s_2$ units of the first and $-s_1$ of the second, and place $-s_2V_1+s_1V_2$ in the [bank account](../../../../../../bank-account.md). The portfolio has zero current value and zero diffusion exposure. Its instantaneous excess drift is

$$
s_2(m_1-rV_1)-s_1(m_2-rV_2).
$$

If this were nonzero, selecting its positive orientation and maintaining the local risk-cancelling [self-financing](../../../../../../self-financing-portfolio.md) hedge would generate a gain without risk from zero wealth. Under the usual trading and regularity assumptions this violates absence of [arbitrage](../../../../../../arbitrage.md). Thus the expression vanishes, and at nonzero exposures

$$
\boxed{\frac{m_1-rV_1}{s_1}=\frac{m_2-rV_2}{s_2}=\theta(t,r).}
$$

At zero exposure the correct relation is $m-rV=\theta s=0$, without dividing by zero. This is a condition on traded securities: the physical drift of the nontraded [short rate](../../../../../../short-rate.md) alone does not determine $\theta$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
