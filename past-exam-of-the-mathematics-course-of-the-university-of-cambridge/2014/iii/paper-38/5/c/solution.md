<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate the [Gaussian](../../../../../../normal-distribution.md) price with respect to $s$. The terms involving derivatives of $d$ cancel because $\phi'(d)=-d\phi(d)$ and $s-Ke^{-r\tau}=\nu d$. Thus the [delta hedge](../../../../../../delta-hedge.md) is

$$
\boxed{\pi_t=C_s(t,S_t)=\Phi\left(\frac{S_t-Ke^{-r(T-t)}}{
\sigma\sqrt{(1-e^{-2r(T-t)})/(2r)}}\right).}
$$

For every $t<T$, $\nu>0$ and $S_t$ is finite, so $0<\pi_t<1$. At maturity its limiting value is the payoff derivative $\mathbf1_{\{S_T>K\}}$ except at the kink, an event of probability zero under the equivalent [Gaussian](../../../../../../normal-distribution.md) law. Consequently **the [stock](../../../../../../stock.md) holding is always nonnegative and never exceeds one**. The initial drift $\mu$ does not enter this hedge; it is removed by the change to the [risk-neutral measure](../../../../../../risk-neutral-measure.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
