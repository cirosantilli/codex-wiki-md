<h1 id="27k/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Expand the payoff as $(S_T-2K+K^2/S_T)1_{\{S_T>K\}}$. The same [risk-neutral measure](../../../../../../risk-neutral-measure.md) applies. For any real $p$, completing the square gives the [truncated lognormal moment](../../../../../../truncated-lognormal-moment.md)

$$
\mathbb E[S_T^p1_{\{S_T>K\}}]=S_0^pe^{prT+p(p-1)\sigma^2T/2}\Phi(d_2+p\sigma\sqrt T).
$$

Using $p=1,0,-1$ and discounting by $e^{-rT}$ gives

$$
\boxed{V_0=S_0\Phi(d_1)-2Ke^{-rT}\Phi(d_2)+\frac{K^2}{S_0}e^{-2rT+\sigma^2T}\Phi(d_2-\sigma\sqrt T).}
$$

The inverse-price moment explains both the extra volatility factor and the shifted normal argument in the last term.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
