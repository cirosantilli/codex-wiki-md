<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the maturity $T$ fixed and write $F(t,T)=\exp L(t,x_t)$, where

$$
L(t,x)=ax+(1-a)\widetilde\mu+\frac{\sigma^2}{4\alpha}(1-a^2),\qquad a=e^{-\alpha(T-t)}.
$$

As calendar time increases, $\partial_ta=\alpha a$, so $L_x=a$, $L_{xx}=0$ and $L_t=\alpha a(x-\widetilde\mu)-\sigma^2a^2/2$. Applying the [Itô formula](../../../../ito-s-lemma.md) to $L$ and then to its exponential gives

$$
dL=-\frac12\sigma^2a^2dt+\sigma a\,dZ_t,\qquad \boxed{\frac{dF(t,T)}{F(t,T)}=\sigma e^{-\alpha(T-t)}\,dZ_t}.
$$

The [Itô formula](../../../../ito-s-lemma.md)'s exponential correction cancels the displayed drift of $L$. The zero drift also follows from the [tower property of conditional expectation](../../../../law-of-total-expectation.md): for $t\leq u\leq T$, $\mathbb E_t[F(u,T)]=\mathbb E_t[S_T]=F(t,T)$. In particular $F(T,T)=S_T$, while the quote's instantaneous [spot volatility](../../../../spot-volatility.md) approaches $\sigma$ as expiry approaches.

This is a [martingale](../../../../martingale-split.md) under the same measure used in the stipulated [conditional expectation](../../../../conditional-expectation.md). To interpret it as [futures pricing](../../../../futures-pricing.md), that measure must be a suitable pricing measure. For a non-dividend-paying traded [stock](../../../../stock.md) at a deterministic [interest rate](../../../../interest-rate.md), the absence of [arbitrage](../../../../arbitrage.md) instead gives a [forward contract](../../../../forward-contract.md) delivery price $S_t e^{r(T-t)}$. A physical-measure expectation under the given mean-reverting drift is not automatically that price; the question's expectation convention is sufficient for the calculation above, but not for this additional identification.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
