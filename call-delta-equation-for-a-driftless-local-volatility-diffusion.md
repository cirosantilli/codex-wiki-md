# Call delta equation for a driftless local volatility diffusion

↑ **Parent:** [Option delta](option-delta.md)

In the cash-numéraire market $dS_t=a(S_t)dW_t$, let a smooth call value solve $V_t+\tfrac12a^2V_{SS}=0$. Its [delta hedge](delta-hedge.md) is $U=V_S$. Differentiating the pricing equation gives

$$
U_t+aa'U_S+\frac12a^2U_{SS}=0,\qquad U(T,S)=\mathbf1_{\{S\ge K\}},
$$

with the terminal value at the strike understood up to the null probability of the diffusion hitting that exact terminal value. By [Itô formula](ito-s-lemma.md), $dU(t,S_t)=-aa'U_Sdt+aU_SdW_t$, while $dV(t,S_t)=U(t,S_t)dS_t$. Thus holding $U(t,S_t)$ shares and cash $V-SU$ replicates the terminal call. The drift in the [option delta](option-delta.md) equation comes from differentiating the spatially varying diffusion coefficient, not from a drift in the original [stock](stock.md).

**Table of contents**

- [Derivative-weighted call delta martingale](derivative-weighted-call-delta-martingale.md)

## ↑ Ancestors (7)

1. [Option delta](option-delta.md)
2. [Greeks (finance)](greeks-finance.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Derivative-weighted call delta martingale](derivative-weighted-call-delta-martingale.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/4/solution.md)
