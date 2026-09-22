<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $L=\exp((r-\frac12\sigma^2)(T-t)+\sigma\sqrt{T-t}\,Z)$. Boundedness of $g'$ and integrability of the [lognormal distribution](../../../../../../log-normal-distribution.md) variable $L$ justify differentiation under the expectation, by dominated convergence:

$$
V_s(t,s)=e^{-r(T-t)}\mathbb E[g'(sL)L].
$$

A differentiable increasing payoff has $g'\geq0$, and $L>0$. Thus the [delta hedge](../../../../../../delta-hedge.md) has

$$
\boxed{\pi_t=e^{-r(T-t)}\mathbb E[g'(S_tL)L]\geq0.}
$$

Moreover $\mathbb EL=e^{r(T-t)}$, so $0\leq\pi_t\leq\|g'\|_\infty$. At maturity the delta is $g'(S_T)\geq0$. The [admissible trading strategy](../../../../../../admissible-trading-strategy.md) already constructed therefore uses nonnegative stock holdings throughout replication. After maturity, liquidate the stock position and retain the proceeds in the bank account, so $\pi_t=0$ for $t>T$ if holdings are to be defined for all times.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
