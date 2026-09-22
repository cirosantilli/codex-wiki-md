<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\pi_t$ be the [predictable](../../../../../../predictable-process.md) [stock](../../../../../../stock.md) holding during $(t-1,t]$. Cash has constant price, so [self-financing](../../../../../../self-financing-portfolio.md) gives

$$
X_t-X_{t-1}=\pi_t(S_t-S_{t-1}),\qquad
X_t=\mathbb E[\xi\mid\mathcal F_t].
$$

Put $\mathcal G=\mathcal F_{t-1}$. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) and $\mathcal F_t$-measurability of $S_t$ give

$$
\operatorname{Cov}(\xi,S_t\mid\mathcal G)
=\operatorname{Cov}(X_t,S_t\mid\mathcal G).
$$

Since $X_{t-1}$, $S_{t-1}$ and $\pi_t$ are $\mathcal G$-measurable, substituting the gains identity yields

$$
\operatorname{Cov}(X_t,S_t\mid\mathcal G)
=\pi_t\operatorname{Var}(S_t\mid\mathcal G).
$$

The denominator is positive on every positive-probability parent atom. If it were zero on such an atom, $S_t$ would be constant there, and the [martingale](../../../../../../martingale-split.md) property would force that constant to equal $S_{t-1}$, contradicting the nonzero-increment assumption. Hence

$$
\boxed{\pi_t=\frac{\operatorname{Cov}(\xi,S_t\mid\mathcal F_{t-1})}
{\operatorname{Var}(S_t\mid\mathcal F_{t-1})},\qquad1\leq t\leq T.}
$$

This is [conditional covariance hedge ratio](../../../../../../recovery-of-a-martingale-transform-integrand-by-conditional-covariance.md). It uses attainability; a regression coefficient alone would not replicate a general unattainable payoff. After maturity one may liquidate into cash, so the same formula gives zero for later dates wherever its denominator remains nonzero. On a finite sample space a [martingale](../../../../../../martingale-split.md) cannot have nonzero increments forever; the stated nondegeneracy is naturally a finite-maturity assumption.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
