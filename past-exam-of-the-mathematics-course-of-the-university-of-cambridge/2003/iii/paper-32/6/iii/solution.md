<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An [interest-rate cap](../../../../../../interest-rate-cap.md) is the sum of [caplets](../../../../../../caplet.md) over successive reset and payment dates. Consider one accrual period $[T,U]$ with year fraction $\delta>0$ and strike $K\geq0$. The reset rate is $L(T;T,U)=[P(T,U)^{-1}-1]/\delta$; the unit-notional payment at $U$ is $\delta(L-K)^+$. At reset its value is

$$
P(T,U)\left(P(T,U)^{-1}-1-\delta K\right)^+=\left(1-(1+\delta K)P(T,U)\right)^+.
$$

Hence the [caplet](../../../../../../caplet.md) is equivalent before reset to $c=1+\delta K$ puts expiring at $T$ on the maturity-$U$ [zero-coupon bond](../../../../../../zero-coupon-bond.md), with strike $K_b=1/c$. This algebra accounts for payment at $U$ rather than incorrectly treating the payment date as $T$.

Under the [T-forward measure](../../../../../../t-forward-measure.md), use the bond-ratio process $F_s=P(s,U)/P(s,T)$, which is a [martingale](../../../../../../martingale-split.md). From the Gaussian HJM dynamics its relative volatility is $-[\Sigma(s,U)-\Sigma(s,T)]$. With deterministic volatilities its logarithm at reset is normal with integrated variance

$$
v^2=\int_t^T\|\Sigma(s,U)-\Sigma(s,T)\|^2ds=\int_t^T\left\|\int_T^U\sigma(s,u)du\right\|^2ds.
$$

For $v>0$, write $d_1=\log(F_t/K_b)/v+v/2$ and $d_2=d_1-v$. A normal integral gives $\mathbb Q^T(F_T<K_b\mid\mathcal F_t)=\Phi(-d_2)$ and $\mathbb E_{Q^T}[F_T\mathbf1_{\{F_T<K_b\}}\mid\mathcal F_t]=F_t\Phi(-d_1)$. Therefore the [Gaussian caplet bond-put formula](../../../../../../gaussian-caplet-bond-put-formula.md) is

$$
\boxed{C_t=P(t,T)\Phi(-d_2)-(1+\delta K)P(t,U)\Phi(-d_1).}
$$

For $v=0$, the value is $\big(P(t,T)-(1+\delta K)P(t,U)\big)^+$. This is also obtained from the [Gaussian bond-option formula](../../../../../../gaussian-bond-option-formula.md) by put-call parity. A cap price is the sum of its caplet prices, multiplied by the notional principal.

In the [Vasicek model](../../../../../../vasicek-model.md), the instantaneous forward-rate volatility is $\sigma(s,u)=\eta e^{-\kappa(u-s)}$. Thus

$$
\boxed{v^2=\frac{\eta^2}{2\kappa^3}(1-e^{-\kappa(U-T)})^2(1-e^{-2\kappa(T-t)}).}
$$

Indeed, $\Sigma(s,U)-\Sigma(s,T)=\eta e^{-\kappa(T-s)}(1-e^{-\kappa(U-T)})/\kappa$, whose squared integral gives this expression without ambiguity. Gaussian short and instantaneous forward rates do not mean the reset floating rate $L$ is Gaussian: the latter is an inverse bond price minus one. The lognormal bond-ratio calculation, under the proper [forward measure](../../../../../../forward-measure.md), is the reason for the normal-CDF pricing formula.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
