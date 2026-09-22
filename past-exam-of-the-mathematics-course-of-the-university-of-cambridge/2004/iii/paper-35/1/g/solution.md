<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

All three individual risky assets now have negative excess [expected returns](../../../../../../expected-return.md). The [covariance matrix](../../../../../../covariance-matrix.md) and the risky [portfolio opportunity set](../../../../../../portfolio-opportunity-set.md) remain unchanged, but the risk-free point moves above all three individual means. Solving the new tangency equations gives

$$
z=\Sigma^{-1}(-15,-8,-1)^T=\frac1{77}(-283,-41,18)^T,\qquad s=\mathbf1^Tz=-\frac{306}{77}.
$$

The [sign of the normalized tangency portfolio](../../../../../../sign-of-the-normalized-tangency-portfolio.md) now matters. Normalizing to a unit risky budget gives

$$
w_M=\frac1{306}(283,41,-18)^T,\qquad m_M=\frac{3095}{306}<25,
$$

and its [Sharpe ratio](../../../../../../sharpe-ratio.md) is $-\sqrt{4555/77}$. This point touches the lower risky frontier, rather than being an efficient positive-premium [market portfolio](../../../../../../market-portfolio.md).

The positive-premium efficient direction is still $x=cz$, $c>0$. It shorts the first two assets, holds a hedging long position in the third, and has negative total risky investment. Its risk-free investment exceeds its initial wealth: the net proceeds of [short selling](../../../../../../short-finance.md) are lent. Equivalently it takes a negative position in the normalized tangency portfolio. Thus

$$
\boxed{\text{upper efficient slope}=+\sqrt{\frac{4555}{77}},\quad \text{normalized tangency Sharpe ratio}=-\sqrt{\frac{4555}{77}}.}
$$

Negative excess means therefore do not eliminate efficient risky investments when unrestricted [short selling](../../../../../../short-finance.md) is allowed. The second diagram shows both orientations; it would be incorrect to interpret the negative normalized ratio as a negative slope for the upper efficient ray.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
