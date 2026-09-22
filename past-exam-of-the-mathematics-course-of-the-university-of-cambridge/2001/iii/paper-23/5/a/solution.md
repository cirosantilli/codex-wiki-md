<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) is defined by $f(t,T)=-\partial_T\log P(t,T)$, with $P(t,t)=1$. Integrating in maturity gives the [zero-coupon bond](../../../../../../zero-coupon-bond.md) price and its diagonal [short rate](../../../../../../short-rate.md):

$$
\boxed{P(t,T)=\exp\left(-\int_t^Tf(t,u)\,du\right),\qquad r_t=f(t,t).}
$$

The solution of the [continuous-time bank account](../../../../../../continuous-time-bank-account.md) equation $dB_t=r_tB_tdt$, $B_0=1$, is $B_t=\exp(\int_0^tr_sds)$; the integration variable is time. Its discounted bond value is

$$
\boxed{Z_t(t,T)=B_t^{-1}P(t,T)
=\exp\left(-\int_0^tr_sds-\int_t^Tf(t,u)\,du\right).}
$$

All these are [adapted processes](../../../../../../adapted-process.md) when the [Heath-Jarrow-Morton model](../../../../../../heath-jarrow-morton-model.md) coefficients are adapted and the integrals exist.

For [market completeness](../../../../../../complete-market.md), stochastic integration over maturity gives

$$
d\log P(t,T)=\left[r_t-\int_t^T\alpha(t,u)\,du\right]dt+\Sigma(t,T)dW_t,\qquad
\Sigma(t,T)=-\int_t^T\sigma(t,u)\,du.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) for the exponential then yields

$$
\frac{dP(t,T)}{P(t,T)}
=\left[r_t-\int_t^T\alpha(t,u)\,du+\frac12\Sigma(t,T)^2\right]dt+\Sigma(t,T)dW_t.
$$

Consequently under a [risk-neutral measure](../../../../../../risk-neutral-measure.md) the no-arbitrage drift restriction is

$$
\int_t^T\alpha^Q(t,u)\,du=\frac12\left(\int_t^T\sigma(t,u)\,du\right)^2,\qquad
\alpha^Q(t,T)=\sigma(t,T)\int_t^T\sigma(t,u)\,du.
$$

The last equality needs sufficient maturity regularity and has a positive sign despite the negative definition of $\Sigma$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
