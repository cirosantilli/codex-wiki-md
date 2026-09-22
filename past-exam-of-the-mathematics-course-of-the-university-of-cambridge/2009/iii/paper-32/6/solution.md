<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A unit-face-value [zero-coupon bond](../../../../../zero-coupon-bond.md) pays one unit of currency at its maturity $T$ and makes no earlier payments. Write its time-$t$ price as $P(t,T)$, with $P(T,T)=1$. The [instantaneous forward rate](../../../../../instantaneous-forward-rate.md) is related to the bond price by

$$
\boxed{f_t(T)=-\partial_T\log P(t,T),\qquad P(t,T)=\exp\left(-\int_t^T f_t(u)du\right).}
$$

The [short rate](../../../../../short-rate.md) is $r_t=f_t(t)$, and the money-market account is $B_t=\exp(\int_0^tr_sds)$.

Apply [Itô formula](../../../../../ito-s-lemma.md) to $f_t(T)=F(T-t,r_t)$, holding maturity fixed:

$$
df_t(T)=\left(-F_\theta+a(r_t)F_r+\frac12b(r_t)^2F_{rr}\right)dt+b(r_t)F_r\,dW_t.
$$

The supplied equation identifies its volatility and drift as

$$
\sigma_t(T)=b(r_t)F_r(T-t,r_t),\qquad\alpha_t(T)=\sigma_t(T)\int_t^T\sigma_t(u)du.
$$

This is exactly the one-factor [Heath-Jarrow-Morton model](../../../../../heath-jarrow-morton-model.md) drift restriction with zero market price of risk. The initial condition also verifies $f_t(t)=F(0,r_t)=r_t$.

To verify absence of [arbitrage](../../../../../arbitrage.md) directly, without merely naming the drift restriction, put

$$
G(\theta,r)=\int_0^\theta F(s,r)ds,\qquad\Sigma_t(T)=b(r_t)G_r(T-t,r_t).
$$

Integrate the equation in its first variable. Since $F(0,r)=r$ and

$$
\int_0^\theta F_r(s,r)\left(\int_0^sF_r(u,r)du\right)ds=\frac12G_r(\theta,r)^2,
$$

we obtain

$$
F(\theta,r)-r=a(r)G_r+\frac12b(r)^2G_{rr}-\frac12b(r)^2G_r^2.
$$

The bond price from the forward curve is $P(t,T)=e^{-G(T-t,r_t)}$. Its logarithm therefore satisfies

$$
d\log P(t,T)=\left(F-aG_r-\frac12b^2G_{rr}\right)dt-bG_r\,dW_t
=\left(r_t-\frac12\Sigma_t(T)^2\right)dt-\Sigma_t(T)dW_t.
$$

A second application of [Itô formula](../../../../../ito-s-lemma.md) gives

$$
\boxed{\frac{dP(t,T)}{P(t,T)}=r_tdt-\Sigma_t(T)dW_t,\qquad\frac{d(P(t,T)/B_t)}{P(t,T)/B_t}=-\Sigma_t(T)dW_t.}
$$

Thus every discounted bond price is a positive [local martingale](../../../../../local-martingale.md) under the original measure. The sufficient no-arbitrage theorem is: if a common equivalent probability measure makes all discounted traded prices [local martingales](../../../../../local-martingale.md), then there is no [arbitrage](../../../../../arbitrage.md) using [self-financing strategies](../../../../../self-financing-portfolio.md) whose discounted wealth has a deterministic lower bound. Its proof is the [supermartingale](../../../../../supermartingale.md) bound on such wealth. Apply it to any finite collection of bond maturities, using the original measure itself. This establishes **no admissible [arbitrage](../../../../../arbitrage.md)** in the bond market, on horizons where the stated [short rate](../../../../../short-rate.md) model and smooth forward curve are defined. It is the [Forward-rate equation for a Markov short-rate diffusion](../../../../../forward-rate-equation-for-a-markov-short-rate-diffusion.md) construction.

For the constant-coefficient case, substitute $F(\theta,r)=A(\theta)r+B(\theta)$. The initial condition requires $A(0)=1$ and $B(0)=0$. Since $F_r=A$ and $F_{rr}=0$, the equation becomes

$$
A'(\theta)r+B'(\theta)=a_0A(\theta)-b_0^2A(\theta)\int_0^\theta A(s)ds.
$$

The right-hand side does not depend on $r$, so $A'=0$ and $A=1$. It follows that $B'=a_0-b_0^2\theta$, giving

$$
\boxed{A(\theta)=1,\qquad B(\theta)=a_0\theta-\frac12b_0^2\theta^2,\qquad f_t(T)=r_t+a_0(T-t)-\frac12b_0^2(T-t)^2.}
$$

The corresponding [zero-coupon bond](../../../../../zero-coupon-bond.md) price is

$$
\boxed{P(t,T)=\exp\left(-(T-t)r_t-\frac{a_0}2(T-t)^2+\frac{b_0^2}6(T-t)^3\right).}
$$

It has discounted volatility $-b_0(T-t)$, which is deterministic and square-integrable on finite horizons. Its discounted price is consequently a true [martingale](../../../../../martingale-split.md), so the no-arbitrage conclusion follows again. This is the [Gaussian short-rate model with constant coefficients](../../../../../gaussian-short-rate-model-with-constant-coefficients.md).

As a separate check of the signs, conditional on $\mathcal F_t$,

$$
\int_t^T r_sds=(T-t)r_t+\frac{a_0}2(T-t)^2+b_0\int_t^T(W_s-W_t)ds.
$$

The final integral is centered Gaussian with variance $(T-t)^3/3$, obtained by integrating $\operatorname{Cov}(W_s-W_t,W_u-W_t)=\min(s-t,u-t)$. Its negative exponential expectation gives exactly the positive $b_0^2(T-t)^3/6$ term in the bond-price exponent above.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
