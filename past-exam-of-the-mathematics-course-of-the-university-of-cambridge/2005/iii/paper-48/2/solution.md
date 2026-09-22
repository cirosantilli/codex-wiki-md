<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Substitute the nonzero product $V=f(S)g(t)$ into the [Black-Scholes equation with continuous stock dividends](../../../../../black-scholes-equation-with-continuous-stock-dividends.md) and divide by $fg$ on intervals where it is nonzero. The result is

$$
-\frac{\dot g}{g}+r
=\frac{\tfrac12\sigma^2S^2f''+(r-q)Sf'}{f}.
$$

The left side depends only on time and the right side only on spot, so both equal a constant $\lambda$. Thus

$$
\boxed{\dot g=(r-\lambda)g,\qquad
\tfrac12\sigma^2S^2f''+(r-q)Sf'-\lambda f=0.}
$$

These are the [separated solutions of the Black-Scholes equation](../../../../../separated-solutions-of-the-black-scholes-equation.md). The zero solution is included separately, so division loses no relevant case.

For the unheaded parity request, the terminal difference of the power-call and power-put payoffs is $S_T^\beta-K^\beta$. Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), $S_T=S\exp[(r-q-\sigma^2/2)\tau+\sigma(W_T-W_t)]$, where $\tau=T-t$. The [Gaussian](../../../../../normal-distribution.md) exponential moment gives $\mathbb E_Q[S_T^\beta\mid S_t=S]=S^\beta e^{\lambda_\beta\tau}$ with $\lambda_\beta=\beta(r-q)+\sigma^2\beta(\beta-1)/2$. Discounting the difference proves [power put-call parity](../../../../../power-put-call-parity.md):

$$
\boxed{C_\beta(S,t)-P_\beta(S,t)=S^\beta e^{(\lambda_\beta-r)(T-t)}-K^\beta e^{-r(T-t)}.}
$$

For $\beta=1$ this is the familiar dividend-adjusted [put-call parity](../../../../../put-call-parity.md), $Se^{-q\tau}-Ke^{-r\tau}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
