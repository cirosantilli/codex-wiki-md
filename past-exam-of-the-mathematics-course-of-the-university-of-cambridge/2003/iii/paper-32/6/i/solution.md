<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Gaussian](../../../../../../normal-distribution.md) [one-factor short-rate model](../../../../../../one-factor-short-rate-model.md) is most naturally specified under a chosen [risk-neutral measure](../../../../../../risk-neutral-measure.md) $Q$, not by using a physical drift unaltered in a pricing formula. The [Vasicek model](../../../../../../vasicek-model.md) has

$$
dr_t=\kappa(\bar r-r_t)dt+\eta dW_t^Q,\qquad\kappa>0.
$$

Its explicit solution is $r_s=\bar r+(r_t-\bar r)e^{-\kappa(s-t)}+\eta\int_t^s e^{-\kappa(s-u)}dW_u^Q$. It is a [Markov process](../../../../../../markov-process-split.md), and its conditional mean and variance are $\bar r+(r_t-\bar r)e^{-\kappa(s-t)}$ and $\eta^2(1-e^{-2\kappa(s-t)})/(2\kappa)$. Hence all finite-dimensional distributions are Gaussian. The model permits negative rates; Gaussianity does not enforce their positivity.

The unit [zero-coupon bond](../../../../../../zero-coupon-bond.md) price is $P(t,T)=\mathbb E_Q[e^{-\int_t^T r_sds}\mid\mathcal F_t]$. Write $\tau=T-t$ and $B(\tau)=(1-e^{-\kappa\tau})/\kappa$. Stochastic integration of the explicit solution gives

$$
\int_t^T r_sds=\bar r\tau+(r_t-\bar r)B(\tau)+\eta\int_t^T B(T-u)dW_u^Q.
$$

This Gaussian variable has variance $\eta^2\int_0^\tau B(v)^2dv$. Evaluating its exponential moment gives [exponential-affine bond pricing](../../../../../../exponential-affine-bond-pricing.md)

$$
\boxed{P(t,T)=A(\tau)e^{-B(\tau)r_t},\quad\log A(\tau)=\left(\bar r-\frac{\eta^2}{2\kappa^2}\right)(B(\tau)-\tau)-\frac{\eta^2B(\tau)^2}{4\kappa}.}
$$

For example, $\int_0^\tau B(v)^2dv=\kappa^{-2}[\tau-2B(\tau)+(1-e^{-2\kappa\tau})/(2\kappa)]$, which gives the displayed expression by direct simplification. The [term structure of interest rates](../../../../../../yield-curve.md) is therefore analytically tractable, and bond-price changes are driven by the current short rate alone.

The [Hull-White model](../../../../../../hull-white-model.md) replaces the drift by $\alpha(t)-\kappa r_t$ with deterministic $\alpha$. The same calculation gives

$$
P(t,T)=\exp\!\left[-B(T-t)r_t-\int_t^T B(T-u)\alpha(u)du+\frac{\eta^2}{2}\int_t^T B(T-u)^2du\right].
$$

This retains the one-factor Gaussian and Markov structure while allowing an exact initial-curve fit through $\alpha$. If $f_0(t)$ is the initial [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) and $r_0=f_0(0)$, differentiating the bond formula shows that

$$
\alpha(t)=f_0'(t)+\kappa f_0(t)+\frac{\eta^2}{2\kappa}(1-e^{-2\kappa t}).
$$

Thus calibration flexibility is separated from stochastic mean reversion. Time-dependent calibration generally destroys time stationarity even though the state remains Markov. In the time-homogeneous Vasicek case, a stationary initialization is $r_0\sim N(\bar r,\eta^2/(2\kappa))$ independent of future increments; its covariance is $\eta^2e^{-\kappa|t-s|}/(2\kappa)$. A fixed initial short rate does not give a stationary process.

## ↑ Ancestors (11)

1. [I](../i.md)
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
