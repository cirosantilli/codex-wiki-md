<h1 id="b/7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Linearity separates the terminal call payoff from the running payment stream. The first contributes the supplied European call price. Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), $\mathbb E(S_v\mid S_t=s)=se^{r(v-t)}$, so the stream contributes

$$
\mathbb E^{\mathbb Q}\int_t^Te^{-r(v-t)}qS_v\,dv
=qs\int_t^Tdv=qs(T-t).
$$

Consequently

$$
\boxed{V(t,s)=s\Phi(d_1)-Ke^{-r(T-t)}\Phi(d_2)+qs(T-t).}
$$

This is the [claim dividends proportional to the underlying stock](../../../../../claim-dividends-proportional-to-the-underlying-stock.md) identity. The underlying itself is still non-dividend-paying; the cash flow belongs to the derivative.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
