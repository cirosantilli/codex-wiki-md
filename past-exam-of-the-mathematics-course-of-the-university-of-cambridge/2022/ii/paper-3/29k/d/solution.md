<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the risk-neutral measure, write

$$
S_t=S_0e^{X_t},
\qquad
X_t=\left(r-\frac12\sigma^2\right)t+\sigma W_t^Q.
$$

Let $M_T=\max_{t\leq T}X_t$ and $m_T=\min_{t\leq T}X_t$. Then

$$
Y_1=S_0e^{M_T},
\qquad
Y_2=S_0e^{pX_T-m_T}.
$$

The time-reversed increment process

$$
\widetilde X_t=X_T-X_{T-t},
\qquad0\leq t\leq T,
$$

has the same finite-dimensional distributions as $X$, because $X$ has stationary independent increments. Moreover,

$$
\max_{t\leq T}\widetilde X_t=X_T-m_T.
$$

Choosing

$$
\boxed{p=1}
$$

therefore makes $Y_2=S_0e^{X_T-m_T}$ equal in distribution to $Y_1$. Their discounted expectations, and hence their time-zero Black--Scholes prices, are equal. This is [Brownian time reversal for fixed-strike lookback extrema](../../../../../../brownian-time-reversal-for-fixed-strike-lookback-extrema.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
