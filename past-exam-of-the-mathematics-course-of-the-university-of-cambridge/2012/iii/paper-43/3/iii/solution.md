<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Yes: different adapted volatilities can give perfectly correlated terminal prices.** The counterexample in part ii already establishes this with one nonconstant volatility. Both can be nonconstant as well. Put $h(x)=1+\tfrac12\tanh x$ and take

$$
S_t=\mathcal E\left(\int_0^\cdot h(B_u)dB_u\right)_t,\qquad S'_t=\tfrac12(1+S_t),\qquad r=0.
$$

The [Doléans-Dade exponential](../../../../../../doleans-dade-exponential.md) has volatility $h(B_t)$, bounded between $1/2$ and $3/2$. The second stock has volatility $h(B_t)S_t/(1+S_t)$, also bounded and nonconstant. Their squared volatility difference integrates to

$$
\int_0^t\frac{h(B_u)^2}{(1+S_u)^2}\,du>0\quad(t>0).
$$

The [Novikov condition](../../../../../../novikov-s-condition.md) and boundedness give true square-integrable [martingales](../../../../../../martingale-split.md), and the [Itô isometry](../../../../../../ito-isometry.md) gives positive [variance](../../../../../../variance-split.md) for each $t>0$. Yet $S'_t=(1+S_t)/2$ gives correlation one. The mechanism is positive affine dependence, not equality of the multiplicative volatility coefficients; it also explains the failure of the literal part-ii premise.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
