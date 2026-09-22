<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

On a finite horizon $[0,T]$, let $W$ be a standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md) and let $\theta$ be a [predictable process](../../../../../predictable-process.md) with $\int_0^T|\theta_s|^2ds<\infty$ almost surely. Suppose the [stochastic exponential](../../../../../doleans-dade-exponential.md)

$$
Z_t=\exp\left(-\int_0^t\theta_s\cdot dW_s-\frac12\int_0^t|\theta_s|^2ds\right)
$$

is a true [martingale](../../../../../martingale-split.md) with $\mathbb EZ_T=1$. The [Novikov condition](../../../../../novikov-s-condition.md) $\mathbb E\exp(\frac12\int_0^T|\theta_s|^2ds)<\infty$ is a sufficient condition. The [Girsanov theorem](../../../../../girsanov-theorem.md) says that under $dQ=Z_TdP$,

$$
\boxed{W_t^Q=W_t+\int_0^t\theta_sds\text{ is standard Brownian motion}.}
$$

Because $Z_T>0$, the two measures are equivalent on the terminal sigma-algebra.

For the proof sketch, [Itô formula](../../../../../ito-s-lemma.md) gives $dZ_t=-Z_t\theta_t\cdot dW_t$. Apply the product rule to $Z_tW_t^{Q,i}$. Its finite-variation term $Z_t\theta_t^i dt$ is cancelled by $d[Z,W^i]_t=-Z_t\theta_t^i dt$. After localization the product is a [martingale](../../../../../martingale-split.md) under $P$, and the conditional change-of-measure formula makes $W^{Q,i}$ a [local martingale](../../../../../local-martingale.md) under $Q$. Adding finite variation leaves its covariations unchanged: $[W^{Q,i},W^{Q,j}]_t=\delta_{ij}t$. The [Lévy characterization of multidimensional Brownian motion](../../../../../levy-characterization-of-multidimensional-brownian-motion.md) completes the proof. Localization is essential if the integrands are not bounded; the true-martingale hypothesis on $Z$ permits the final measure change.

For the deal, write $T=t_0$ and use constant [interest rate](../../../../../interest-rate.md) $\rho$, volatility $\sigma>0$ and no [stock](../../../../../stock.md) dividends. Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), the [Black-Scholes model](../../../../../black-scholes-model.md) is

$$
S_t=S_0\exp\left((\rho-\tfrac12\sigma^2)t+\sigma W_t^Q\right).
$$

For example this follows from the preceding theorem with $\theta=(\mu-\rho)/\sigma$ when the physical [stock](../../../../../stock.md) drift is $\mu$. The delivered shares have terminal cash value $S_T\max(r,c/A)$, so its initial value is

$$
V_0=e^{-\rho T}\mathbb E_Q\left[S_T\max(r,c/A)\right].
$$

The factor $S_T$ must be included: the deal is a [stock](../../../../../stock.md) delivery, not a cash payment of the random number of shares.

Use the [stock-numeraire measure in the Black-Scholes model](../../../../../stock-numeraire-measure-in-the-black-scholes-model.md), whose density is

$$
\frac{dQ^S}{dQ}=\frac{e^{-\rho T}S_T}{S_0}=\exp\left(\sigma W_T^Q-\tfrac12\sigma^2T\right).
$$

The [Girsanov theorem](../../../../../girsanov-theorem.md) gives $W_t^S=W_t^Q-\sigma t$ as [Brownian motion](../../../../../brownian-motion-split.md) under $Q^S$. Therefore

$$
\log A=\log S_0+(\rho+\tfrac12\sigma^2)\bar t+\frac\sigma n\sum_{i=1}^nW_{t_i}^S,\qquad\bar t=\frac1n\sum_{i=1}^nt_i.
$$

The [discrete geometric average under the stock-numeraire measure](../../../../../discrete-geometric-average-under-the-stock-numeraire-measure.md) has normally distributed logarithm with

$$
m=\log S_0+(\rho+\tfrac12\sigma^2)\bar t,\qquad v=\frac{\sigma^2}{n^2}\sum_{i,j=1}^n\min(t_i,t_j)=\frac{\sigma^2}{n^2}\sum_{i=1}^n(2i-1)t_i.
$$

The last identity uses the printed descending order of sampling times. Each $t_i$ is the minimum in exactly $2i-1$ ordered pairs. In particular $v>0$.

Assume the ordinary positive deal parameters $r,c>0$ and put $k=\log(c/r)$, $d=(m-k)/\sqrt v$. The [change of numeraire](../../../../../change-of-numeraire.md) gives $V_0=S_0\mathbb E_{Q^S}\max(r,ce^{-Y})$, where $Y=\log A$. Split the integral at $k$. Completing the square in $e^{-y}$ times the [normal probability density](../../../../../normal-density.md) gives

$$
\mathbb P(Y\ge k)=\Phi(d),\qquad\mathbb E[e^{-Y}\mathbf1_{Y<k}]=e^{-m+v/2}\Phi\left(\frac{k-m+v}{\sqrt v}\right).
$$

Thus the [stock-delivery option with a geometric average](../../../../../stock-delivery-option-with-a-geometric-average.md) has value

$$
\boxed{V_0=S_0\left[r\Phi(d)+ce^{-m+v/2}\Phi(-d+\sqrt v)\right].}
$$

Here $\Phi$ is the standard [normal distribution](../../../../../normal-distribution.md) function. Delivery time $T$ does not enter separately once the sampling dates are fixed: the [stock](../../../../../stock.md) numeraire cancels the final [stock](../../../../../stock.md) factor and discounting. As a check, for one sample at $T$, the payment is $\max(rS_T,c)$ and the formula becomes the value of $r$ shares plus a put on their terminal value. If $c=0$ the value is $rS_0$; if $r=0$ the value is $cS_0e^{-m+v/2}$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
