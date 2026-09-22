<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Risk-neutral valuation gives

$$
V_0=e^{-rT}\mathbb E_Q[S_T^p].
$$

Since $W_T^Q\sim N(0,T)$,

$$
\mathbb E_Q[S_T^p]
=S_0^p
\exp\left[p\left(r-\frac12\sigma^2\right)T
+\frac12p^2\sigma^2T\right].
$$

Hence the [Power payoff in the Black-Scholes model](../../../../../../power-payoff-in-the-black-scholes-model.md) has price

$$
\boxed{
V_0=S_0^p
\exp\left(\left((p-1)r+\frac12p(p-1)\sigma^2\right)T\right)
}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
