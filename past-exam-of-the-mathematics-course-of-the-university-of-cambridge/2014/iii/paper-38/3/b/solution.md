<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The terminal density is strictly positive and has [expectation](../../../../../../expected-value.md) one under the usual deterministic initial bond-price convention. Its density process is

$$
Z_t=\mathbb E^{\mathbb Q}\left[\frac{D_T}{P(0,T)}\,\middle|\,\mathcal F_t\right]
=\frac{D_tP(t,T)}{P(0,T)}.
$$

For $0\leq s\leq t\leq T$, the [Bayes formula for conditional expectation](../../../../../../bayes-formula-for-conditional-expectation.md) under a change of measure gives

$$
\begin{aligned}
\mathbb E^{\mathbb Q_T}\left[\frac{B_t}{P(t,T)}\,\middle|\,\mathcal F_s\right]
&=\frac1{Z_s}\mathbb E^{\mathbb Q}\left[Z_t\frac{B_t}{P(t,T)}\,\middle|\,\mathcal F_s\right]\\
&=\frac1{Z_sP(0,T)}=\frac{B_s}{P(s,T)}.
\end{aligned}
$$

The same calculation at $s=0$ gives the finite [expectation](../../../../../../expected-value.md) $1/P(0,T)$, so this is a true [martingale](../../../../../../martingale-split.md), not just a formal conditional identity. Thus **the [continuous-time bank account](../../../../../../continuous-time-bank-account.md) measured in units of the maturity-$T$ bond is a $\mathbb Q_T$-[martingale](../../../../../../martingale-split.md)**. This is the [forward measure](../../../../../../forward-measure.md) change of [numéraire](../../../../../../numeraire.md). If the initial bond price were random rather than given, [integrability](../../../../../../integrability.md) of its reciprocal would need to be included for this true-martingale assertion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
