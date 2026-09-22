<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume a positive barrier $B\le K<S_0$. Under the zero-rate risk-neutral [Black-Scholes model](../../../../../../black-scholes-model.md), $X_t=\log(S_t/B)$ starts at $x=\log(S_0/B)>0$ and is [Brownian motion](../../../../../../brownian-motion-split.md) with variance rate $\sigma^2$ and drift $\mu=-\sigma^2/2$. The drifted transition density killed at zero is

$$
p^{\rm kill}(t,x,y)=p_\mu(t,y-x)
-e^{-2\mu x/\sigma^2}p_\mu(t,y+x),\qquad y>0.
$$

To see the factor, multiply the zero-drift reflected Gaussian difference by $\exp[\mu(y-x)/\sigma^2-\mu^2t/(2\sigma^2)]$; its second term is the ordinary drifted Gaussian from starting point $-x$ times $e^{-2\mu x/\sigma^2}$.

Integrate the payoff $(Be^y-K)_+$ against this density. The first term is $C(S_0,K)$. Since $K\ge B$, the payoff is zero for $y\le0$, so the second integral may be extended to all real $y$ and equals the ordinary call price from reflected spot $Be^{-x}=B^2/S_0$. The reflection weight is $e^x=S_0/B$. Thus the [down-and-out European call](../../../../../../down-and-out-european-call.md) value is

$$
\boxed{C(S_0,K)-\frac{S_0}{B}C(B^2/S_0,K)}.
$$

This assumes [continuous](../../../../../../continuous-function.md) monitoring and knock-out on first hitting, with no rebate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
