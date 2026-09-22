<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $P_{s,t}>0$ denote the time-$s$ price of a [zero-coupon bond](../../../../../zero-coupon-bond.md) paying one at maturity $t$, with $P_{t,t}=1$. Information available at $s$ is the [sigma-algebra](../../../../../sigma-algebra.md) $\mathcal F_s$ in the market [filtration](../../../../../filtration-probability-theory.md). For a curve differentiable in maturity, the [instantaneous forward rate](../../../../../instantaneous-forward-rate.md) and its diagonal [short rate](../../../../../short-rate.md) are

$$
f(s,t)=-\partial_t\log P_{s,t},\qquad R_s=f(s,s),\qquad
P_{s,t}=\exp\left(-\int_s^tf(s,u)du\right).
$$

The last identity follows by integrating the maturity derivative and using $P_{s,s}=1$. The [continuous-time bank account](../../../../../continuous-time-bank-account.md) reinvesting at the [short rate](../../../../../short-rate.md) is $B_s=\exp(\int_0^sR_udu)$, and its reciprocal is the [discount factor](../../../../../discount-factor.md). Modelling forward rates means specifying a random maturity-indexed curve with an evolution consistent with the same pricing measure for every bond. The expectation below is under that money-market [risk-neutral measure](../../../../../risk-neutral-measure.md), not an unspecified physical measure.

For fixed maturity $t$, if $P_{s,t}/B_s$ is a true [martingale](../../../../../martingale-split.md) on $0\leq s\leq t$, its terminal value is $1/B_t$. Consequently

$$
\frac{P_{s,t}}{B_s}=\mathbb E_Q[B_t^{-1}\mid\mathcal F_s],\qquad
\boxed{P_{s,t}=\mathbb E_Q\left[e^{-\int_s^tR_udu}\mid\mathcal F_s\right].}
$$

Conversely, this representation gives $P_{s,t}/B_s=\mathbb E_Q[B_t^{-1}\mid\mathcal F_s]$, a [conditional-expectation martingale](../../../../../conditional-expectation-martingale.md) by the tower property. For example, for $r<s$, conditioning the right side on $\mathcal F_r$ returns $\mathbb E_Q[B_t^{-1}\mid\mathcal F_r]$. These claims assume $\mathbb E_QB_t^{-1}<\infty$. A positive discounted [local martingale](../../../../../local-martingale.md) alone need not equal the conditional expectation of its terminal value, so the word “martingale” cannot be weakened without an extra integrability argument.

In the [Vasicek model](../../../../../vasicek-model.md), the [Brownian motion](../../../../../brownian-motion-split.md) $W$ and coefficients in $dR_s=\alpha(\beta-R_s)ds+\sigma dW_s$ must be understood under this pricing measure. Multiplying by $e^{\alpha s}$ and integrating gives, conditionally on $\mathcal F_s$,

$$
R_u=\beta+(R_s-\beta)e^{-\alpha(u-s)}+\sigma\int_s^ue^{-\alpha(u-v)}dW_v,\qquad u\geq s.
$$

Assume first $\alpha\ne0$, and put $\tau=t-s$ and $B(\tau)=(1-e^{-\alpha\tau})/\alpha$. Integrating the explicit solution over $s\leq u\leq t$ yields

$$
\int_s^tR_udu=R_sB(\tau)+\beta\{\tau-B(\tau)\}+\sigma\int_s^tB(t-v)dW_v.
$$

The interchange of the stochastic integrals is justified by their deterministic square-integrable kernels on the finite triangular domain; equivalently approximate the kernels by step functions, interchange finite sums, and pass to the limit using the [Itô isometry](../../../../../ito-isometry.md). The last integral conditionally has a centered [normal distribution](../../../../../normal-distribution.md) independent of $\mathcal F_s$, with variance

$$
\sigma^2J(\tau),\qquad
J(\tau)=\int_0^\tau B(v)^2dv
=\frac1{\alpha^2}\left[\tau-2B(\tau)+\frac{1-e^{-2\alpha\tau}}{2\alpha}\right].
$$

A deterministic Brownian integral is Gaussian because its step approximations are sums of independent normal increments; their variances converge by the [Itô isometry](../../../../../ito-isometry.md). Completing the square in the [normal density](../../../../../normal-density.md) proves $\mathbb E e^{-Y}=e^{-m+v/2}$ for a normal variable of mean $m$ and variance $v$. Hence the [zero-coupon bond](../../../../../zero-coupon-bond.md) price is exponential-affine:

$$
\boxed{P_{s,t}=e^{a_{s,t}-b_{s,t}R_s},\quad b_{s,t}=B(\tau),\quad a_{s,t}=-\beta\{\tau-B(\tau)\}+\frac{\sigma^2}{2}J(\tau).}
$$

An equivalent familiar form is

$$
a_{s,t}=\left(\beta-\frac{\sigma^2}{2\alpha^2}\right)(B(\tau)-\tau)-\frac{\sigma^2}{4\alpha}B(\tau)^2.
$$

At $t=s$, both coefficients are zero and the bond value is one. These formulas are valid for negative as well as positive nonzero $\alpha$ on finite horizons, though a genuinely mean-reverting [Vasicek model](../../../../../vasicek-model.md) has $\alpha>0$. For $\alpha=0$, direct integration gives $B(\tau)=\tau$, $J(\tau)=\tau^3/3$ and

$$
\boxed{b_{s,t}=\tau,\qquad a_{s,t}=\sigma^2\tau^3/6.}
$$

All the exponential moments used above are finite, so the prices defined by the conditional expectation do give true discounted [martingales](../../../../../martingale-split.md).

To fit an initial bond curve, let its observed prices $p_0(t)$ be positive, satisfy $p_0(0)=1$, and have a sufficiently smooth [instantaneous forward rate](../../../../../instantaneous-forward-rate.md) $f_0(t)=-d\log p_0(t)/dt$. Set $R_0=f_0(0)$; this compatibility is forced by the infinitesimal-maturity bond price. Replace $\beta$ by a deterministic [function](../../../../../function-split.md) $\theta(t)$, with $\alpha\ne0$, so that

$$
dR_t=\alpha\{\theta(t)-R_t\}dt+\sigma dW_t.
$$

Its mean $m(t)=\mathbb E_QR_t$ satisfies $m'=\alpha(\theta-m)$, $m(0)=R_0$. The variance of the integrated rate remains $\sigma^2J(t)$, since changing deterministic drift does not change the centered Gaussian process. Therefore

$$
-\log P_{0,t}=\int_0^tm(u)du-\frac{\sigma^2}{2}J(t),\qquad
-\partial_t\log P_{0,t}=m(t)-\frac{\sigma^2}{2}B(t)^2.
$$

The required mean is consequently $m(t)=f_0(t)+\sigma^2B(t)^2/2$. Solve its mean equation for $\theta$:

$$
\theta(t)=m(t)+\frac{m'(t)}{\alpha}
=f_0(t)+\frac{f_0'(t)}{\alpha}+\frac{\sigma^2}{2}B(t)^2+\frac{\sigma^2}{\alpha}B(t)e^{-\alpha t}.
$$

Combining the last two terms gives the explicit [Hull-White model](../../../../../hull-white-model.md) calibration in the question's parameter convention:

$$
\boxed{\theta(t)=f_0(t)+\frac{f_0'(t)}{\alpha}+\frac{\sigma^2}{2\alpha^2}(1-e^{-2\alpha t}).}
$$

With $R_0=f_0(0)$, the specified mean solves the same [linear differential equation](../../../../../linear-differential-equation.md) and initial condition as the model mean, so it is the actual mean. The resulting model forward curve equals $f_0$; integrating and using $P_{0,0}=p_0(0)=1$ proves $P_{0,t}=p_0(t)$ for every maturity. If the drift is instead written $\widetilde\theta(t)-\alpha R_t$, its calibration parameter is $\widetilde\theta=\alpha\theta$, not $\theta$ itself.

The printed allowance of arbitrary constants needs a qualification for this final claim. If $\alpha=0$, replacing $\beta$ by $\theta(t)$ changes no coefficient at all: $R_t=R_0+\sigma W_t$ regardless of $\theta$. Its initial curve is fixed at $P_{0,t}=\exp(-R_0t+\sigma^2t^3/6)$. With $\sigma\ne0$, the compatible smooth observed curve $p_0(t)=e^{-R_0t}$ is already a counterexample to the unconditional fitting claim. Thus **arbitrary compatible smooth positive initial curves can be fitted by the stated replacement when $\alpha\ne0$; it cannot fit arbitrary curves when $\alpha=0$**. In that degenerate case one can instead introduce an independent deterministic drift $k(t)$ in $dR_t=k(t)dt+\sigma dW_t$, choosing $k(t)=f_0'(t)+\sigma^2t$ to recover the desired initial curve. Likewise an externally fixed $R_0\ne f_0(0)$ is incompatible with exact fitting, and an arbitrary nonsmooth set of prices need not define the differentiable forward curve assumed in the model.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
