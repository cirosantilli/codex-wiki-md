<h1 id="27k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the [Black-Scholes model](../../../../../../black-scholes-model.md), absence of arbitrage and completeness give the price as the discounted expectation under the [risk-neutral measure](../../../../../../risk-neutral-measure.md). Under that measure,

$$
\log S_T=\log S_0+(r-\sigma^2/2)T+\sigma\sqrt T\,Z,\qquad Z\sim N(0,1).
$$

The physical drift $\mu$ therefore does not enter the option price. Put

$$
d_2=\frac{\log(S_0/K)+(r-\sigma^2/2)T}{\sigma\sqrt T},\qquad d_1=d_2+\sigma\sqrt T.
$$

For the standard [normal distribution](../../../../../../normal-distribution.md) function $\Phi$, $\mathbb P(S_T>K)=\Phi(d_2)$. Completing the square in the Gaussian density also gives $\mathbb E[S_T1_{\{S_T>K\}}]=S_0e^{rT}\Phi(d_1)$. Expanding the call payoff into these two truncated moments yields

$$
\boxed{C_0=S_0\Phi(d_1)-Ke^{-rT}\Phi(d_2).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [27K](../../27k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
