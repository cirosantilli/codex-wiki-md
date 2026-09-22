<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $T=t_0$, $B_t=e^{-\rho(T-t)}$, and let $V_t=f(S_t,t)$ with $f(x,t)=xg(x,t)+B_th(x,t)$. The [portfolio](../../../../../investment-portfolio.md) holds $g(S_t,t)$ shares of [stock](../../../../../stock.md) and $h(S_t,t)$ units of the [zero-coupon bond](../../../../../zero-coupon-bond.md). It is [self-financing](../../../../../self-financing-portfolio.md) when all changes of holdings are funded within it, which is the gain identity

$$
dV_t=g(S_t,t)\,dS_t+h(S_t,t)\,dB_t.
$$

Under the physical [probability measure](../../../../../probability-measure.md), write $dS_t=\mu S_tdt+\sigma S_tdW_t$, where $\sigma>0$ and $dB_t=\rho B_tdt$. The [Itô formula](../../../../../ito-s-lemma.md) gives

$$
df(S_t,t)=\left(f_t+\mu S_tf_x+\frac12\sigma^2S_t^2f_{xx}\right)dt
+\sigma S_tf_x\,dW_t.
$$

Matching the [Brownian motion](../../../../../brownian-motion-split.md) coefficients forces $f_x=g$. Since $f_x=g+xg_x+B_th_x$, this is precisely

$$
xg_x+B_th_x=0.
$$

Differentiating $f_x=g$ gives $f_{xx}=g_x$. Since $f_t=xg_t+\rho B_th+B_th_t$, matching the [drift](../../../../../drift-coefficient.md) coefficients now gives

$$
xg_t+B_th_t+\frac12\sigma^2x^2g_x=0.
$$

These are the [self-financing conditions for smooth stock and bond holdings](../../../../../self-financing-conditions-for-smooth-stock-and-bond-holdings.md). Conversely, substituting both identities into the [Itô formula](../../../../../ito-s-lemma.md) gives the gain identity, so they are sufficient as well. Smoothness and the positive [lognormal distribution](../../../../../log-normal-distribution.md) density of $S_t$ extend the identities along the price process to every $x>0$, with boundary times obtained by continuity.

The [portfolio with constant stock value in bond units](../../../../../portfolio-with-constant-stock-value-in-bond-units.md) must have $xg(x,t)=\theta B_t$, so $g(x,t)=\theta B_t/x$. The first condition then gives $h_x=\theta/x$, hence

$$
h(x,t)=\theta\log(x/S_0)+c(t).
$$

The second condition reduces to $c'(t)=\theta(\sigma^2/2-\rho)$. Initial [portfolio wealth](../../../../../portfolio-wealth.md) requires $h(S_0,0)=w_0/B_0-\theta=w_0e^{\rho T}-\theta$. Therefore the holdings are

$$
\boxed{g(x,t)=\frac{\theta e^{-\rho(T-t)}}x,\qquad
h(x,t)=w_0e^{\rho T}-\theta+\theta\log(x/S_0)+\theta(\sigma^2/2-\rho)t.}
$$

The corresponding [portfolio wealth](../../../../../portfolio-wealth.md) is

$$
\boxed{V_t=e^{-\rho(T-t)}\left[w_0e^{\rho T}+\theta\log(S_t/S_0)+\theta(\sigma^2/2-\rho)t\right].}
$$

Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), $\log(S_t/S_0)=(\rho-\sigma^2/2)t+\sigma W_t^Q$, so its value in [zero-coupon bond](../../../../../zero-coupon-bond.md) units is $V_t/B_t=w_0e^{\rho T}+\theta\sigma W_t^Q$. This also verifies the [self-financing](../../../../../self-financing-portfolio.md) gain equation after using the bond as [numéraire](../../../../../numeraire.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
