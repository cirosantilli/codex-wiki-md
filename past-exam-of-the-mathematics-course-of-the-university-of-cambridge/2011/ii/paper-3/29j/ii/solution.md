<h1 id="29j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $G_T=\exp(T^{-1}\int_0^T\log S_u\,du)$, the continuous [Geometric Asian option](../../../../../../geometric-asian-option.md) average. Under the same risk-neutral measure,

$$
\log G_T=\log S_0+\tfrac12(r-\sigma^2/2)T+\frac\sigma T\int_0^TW_u\,du.
$$

The Brownian integral is Gaussian with mean zero and variance

$$
\int_0^T\int_0^T\min(u,v)\,du\,dv=\frac{T^3}{3}.
$$

Thus $\log G_T\sim N(m,v)$, where $m=\log S_0+(r-\sigma^2/2)T/2$ and $v=\sigma^2T/3$. Define

$$
D_2=\frac{m-\log K}{\sqrt v},\qquad D_1=D_2+\sqrt v,\qquad F_G=e^{m+v/2}=S_0e^{rT/2-\sigma^2T/12}.
$$

The truncated [lognormal distribution](../../../../../../log-normal-distribution.md) calculation from (i) gives

$$
\boxed{V_0=e^{-rT}[F_G\Phi(D_1)-K\Phi(D_2)]=S_0e^{-rT/2-\sigma^2T/12}\Phi(D_1)-Ke^{-rT}\Phi(D_2).}
$$

For comparison, a lognormal call written in terms of its mean $F$ and log-variance $v$ is $c(F,v)=F\Phi(d_1)-K\Phi(d_2)$. Differentiation gives $\partial_Fc=\Phi(d_1)>0$ and $\partial_vc=F\varphi(d_1)/(2\sqrt v)>0$, where $\varphi$ is the standard normal density. The terminal stock has $F_S=S_0e^{rT}$ and $v_S=\sigma^2T$, while $v_G=v_S/3$. Therefore

$$
\boxed{V_0<C_0\quad\text{if }r\geq-\sigma^2/6,\ \sigma,T,K>0,}
$$

since this condition gives $F_G\leq F_S$ and the log-variance is strictly smaller. In particular the requested inequality holds for the usual nonnegative interest rate.

The PDF gives no sign restriction on $r$, so its unconditional comparison needs qualification. If $r<-\sigma^2/6$, then $F_G>F_S$, and as $K\downarrow0$ the two prices tend to $e^{-rT}F_G$ and $e^{-rT}F_S$. By continuity, sufficiently small positive strikes reverse the claimed inequality. Also strictness needs nonzero volatility or another source of a strict mean inequality. These qualifications do not affect the pricing formula.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [29J](../../29j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
