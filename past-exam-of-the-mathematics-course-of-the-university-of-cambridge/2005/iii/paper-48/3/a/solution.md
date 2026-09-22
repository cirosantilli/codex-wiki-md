<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\widehat\sigma(x,t)=\sigma(e^x,t)$, $a(x,t)=\widehat\sigma^2/2$ and $b(x,t)=r-\widehat\sigma^2/2$. The chain rule gives $SV_S=V_x$ and $S^2V_{SS}=V_{xx}-V_x$. Also $V=e^{-r(T-t)}u$, so $V_t=e^{-r(T-t)}(u_t+ru)$. The killing term cancels, leaving

$$
\boxed{u_t+a(x,t)u_{xx}+b(x,t)u_x=0,\qquad u(x,T)=(e^x-K)^+.}
$$

This is the [explicit log-price scheme for local-volatility pricing](../../../../../../explicit-log-price-scheme-for-local-volatility-pricing.md) equation. Under the [risk-neutral measure](../../../../../../risk-neutral-measure.md), the corresponding log-price [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
\boxed{dx_t=\left(r-\frac12\sigma(e^{x_t},t)^2\right)dt+\sigma(e^{x_t},t)dW_t^Q.}
$$

The logarithmic coordinate removes the [stock](../../../../../../stock.md)-price factors from the diffusion coefficient, but retains the spatial variation of [local volatility](../../../../../../local-volatility.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
