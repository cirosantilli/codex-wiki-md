<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $v>0$ and $m>0$, let $\Phi$ and $\phi$ be the [standard normal distribution function](../../../../../standard-normal-distribution-function.md) and density, and put

$$
d_1=\frac{-\log m+v/2}{\sqrt v},\qquad d_2=\frac{-\log m-v/2}{\sqrt v}=d_1-\sqrt v.
$$

The exercise event is $Z>(\log m+v/2)/\sqrt v=-d_2$. Complete the square in the first truncated expectation:

$$
\begin{aligned}
\mathbb E[e^{-v/2+\sqrt vZ}\mathbf1_{\{Z>-d_2\}}]
&=\int_{-d_2}^\infty e^{-v/2+\sqrt vz}\phi(z)dz\\
&=\int_{-d_2}^\infty\phi(z-\sqrt v)dz=\Phi(d_1).
\end{aligned}
$$

The probability of exercise is $\Phi(d_2)$. Hence the [normalized Black-Scholes call function](../../../../../normalized-black-scholes-call-function.md) is

$$
\boxed{F(v,m)=\Phi(d_1)-m\Phi(d_2).}
$$

At $v=0$ it is $(1-m)^+$. If $m\le0$, the positive underlying always exceeds $m$, so $F(v,m)=1-m$; the reciprocal identity below is understood on its natural domain $m>0$.

For the reciprocal strike, $d_1(v,1/m)=-d_2(v,m)$ and $d_2(v,1/m)=-d_1(v,m)$. Thus

$$
\begin{aligned}
1-m+mF(v,1/m)
&=1-m+m\Phi(-d_2)-\Phi(-d_1)\\
&=1-m+m(1-\Phi(d_2))-(1-\Phi(d_1))\\
&=\Phi(d_1)-m\Phi(d_2)=F(v,m).
\end{aligned}
$$

Therefore

$$
\boxed{F(v,m)=1-m+mF(v,1/m),\qquad v\ge0,\ m>0.}
$$

The $v=0$ case follows either by continuity or by checking the two positive parts directly.

For the [stock](../../../../../stock.md) model, the original probability measure is already risk-neutral: $e^{-rt}S_t=S_0e^{\sigma W_t-\sigma^2t/2}$ is a true [martingale](../../../../../martingale-split.md). Write $\tau=T-t$. Conditional on $\mathcal F_t$, the [stock](../../../../../stock.md) at maturity is

$$
S_T=S_te^{r\tau}\exp\left(-\frac12\sigma^2\tau+\sigma\sqrt\tau Z\right),
$$

with $Z$ independent of current information and [standard normal distribution](../../../../../standard-normal-distribution.md). Therefore

$$
\mathbb E[e^{-r\tau}(S_T-K)^+\mid\mathcal F_t]=S_tF\left(\sigma^2\tau,\frac{Ke^{-r\tau}}{S_t}\right)=C_t(T,K).
$$

Equivalently,

$$
e^{-rt}C_t=\mathbb E[e^{-rT}(S_T-K)^+\mid\mathcal F_t],
$$

which is a true [martingale](../../../../../martingale-split.md), since the payoff is integrable. The sufficient direction of the [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md) says that an equivalent measure making all discounted traded prices [local martingales](../../../../../local-martingale.md) excludes [arbitrage](../../../../../arbitrage.md) by [admissible trading strategies](../../../../../admissible-trading-strategy.md). The original measure works simultaneously for the [bank account](../../../../../bank-account.md), [stock](../../../../../stock.md) and call. Thus **the call-augmented market has no [arbitrage](../../../../../arbitrage.md)**.

For the put, hold one call, short one share, and hold $Ke^{-rT}$ units of the [bank account](../../../../../bank-account.md). This [self-financing portfolio](../../../../../self-financing-portfolio.md) has current value $C_t-S_t+Ke^{-r\tau}$ and terminal payoff

$$
(S_T-K)^+-S_T+K=(K-S_T)^+.
$$

Its discounted value is also the [conditional expectation](../../../../../conditional-expectation.md) of that payoff. Thus the [put-call parity](../../../../../put-call-parity.md) price

$$
\boxed{P_t=Ke^{-r\tau}-S_t+C_t}
$$

adds another discounted [martingale](../../../../../martingale-split.md) to the same market, proving **no [arbitrage](../../../../../arbitrage.md) with both call and put included**.

Now put $m=Ke^{-r\tau}/S_t$. The reciprocal identity gives

$$
P_t=S_t(F(\sigma^2\tau,m)-1+m)=S_tmF(\sigma^2\tau,1/m).
$$

The resulting [Put-call symmetry in the Black-Scholes model](../../../../../put-call-symmetry-in-the-black-scholes-model.md) is

$$
\boxed{P_t(T,K)=Ke^{-r(T-t)}F\left((T-t)\sigma^2,\frac{S_te^{r(T-t)}}K\right).}
$$

**The final formula printed in the PDF has two errors:** its discount-rate symbol is undefined, and the reciprocal argument has the wrong sign in the interest-rate exponential. Both are resolved by the displayed calculation. Even replacing the undefined symbol by $r$ leaves an incorrect expression with $e^{-r\tau}$ inside $F$. For $\tau>0$, $r>0$ and $\sigma>0$, $F(v,m)$ is strictly decreasing in $m$, because $\partial_mF=-\mathbb P(e^{-v/2+\sqrt vZ}>m)<0$. The printed argument is smaller than the reciprocal argument and hence gives a strictly larger put price. Thus the literal printed symmetry cannot be established; the boxed expression is the corrected identity.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
