<h1 id="27i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [power option](../../../../../../power-option.md) need not have bounded payoff, but all real powers of a positive lognormal stock have finite moments, so risk-neutral valuation still applies. The [Gaussian](../../../../../../normal-distribution.md) moment-generating identity gives $\mathbb E[e^{n\sigma B_T}]=e^{n^2\sigma^2T/2}$. Therefore

$$
\boxed{V(0,S_0)=S_0^n\exp\left(\left[(n-1)r+\tfrac12n(n-1)\sigma^2\right]T\right).}
$$

For $n=1$ this reduces to $S_0$, and for $n=0$ to the time-zero value $e^{-rT}$ of one unit paid at expiry.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27I](../../27i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
