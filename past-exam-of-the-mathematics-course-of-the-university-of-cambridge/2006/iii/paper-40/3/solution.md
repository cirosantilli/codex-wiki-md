<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume, as in the Bayesian model, that the unknown drift $\alpha$ is independent of the driving [Brownian motion](../../../../../brownian-motion-split.md), with known positive prior precision $\tau_0$. Recover the observed signal from the positive [stock](../../../../../stock.md) price:

$$
Y_t=\frac1\sigma\log(S_t/S_0)+\frac\sigma2t=\alpha t+W_t.
$$

For a fixed time $t$, the centered observed path $Y_s-(s/t)Y_t$ is a [Brownian bridge](../../../../../brownian-bridge.md) independent of $(\alpha,Y_t)$: it is independent of the prior and has zero covariance with $W_t$ in their joint [Gaussian](../../../../../normal-distribution.md) law. Thus the whole observed history has the same posterior information about $\alpha$ as its endpoint. This proves [Brownian endpoint sufficiency for a constant drift](../../../../../brownian-endpoint-sufficiency-for-a-constant-drift.md) rather than assuming it.

The likelihood of that endpoint, as a function of $\alpha$, is proportional to $\exp(\alpha Y_t-\alpha^2t/2)$. Multiplying by the [normal distribution](../../../../../normal-distribution.md) prior and completing the square gives the [Gaussian Brownian drift filter](../../../../../gaussian-brownian-drift-filter.md)

$$
\boxed{\alpha\mid\mathcal F_t^S\sim N(\widehat\alpha_t,\tau_t^{-1}),\qquad
\tau_t=\tau_0+t,\qquad \widehat\alpha_t=\frac{\tau_0\widehat\alpha_0+Y_t}{\tau_0+t}.}
$$

Define the observed [innovation process](../../../../../innovation-process.md) $\widehat W_t=Y_t-\int_0^t\widehat\alpha_sds$. It is a continuous observed-filtration [martingale](../../../../../martingale-split.md): for $s<u$, independence of future noise and the [tower property of conditional expectation](../../../../../law-of-total-expectation.md) give $\mathbb E[\alpha-\widehat\alpha_u\mid\mathcal F_s^S]=0$, so the conditional mean of its increment vanishes. Its [quadratic variation](../../../../../quadratic-variation.md) is $t$, since subtracting the finite-variation drift from $Y$ does not change quadratic variation. The [Lévy characterization of Brownian motion](../../../../../levy-characterization-of-brownian-motion.md) makes $\widehat W$ an observed-filtration [Brownian motion](../../../../../brownian-motion-split.md). Differentiating the posterior mean gives

$$
\boxed{d\widehat\alpha_t=\tau_t^{-1}(dY_t-\widehat\alpha_tdt)=\tau_t^{-1}d\widehat W_t.}
$$

Conversely, the last equation determines $\widehat\alpha$ from $\widehat W$ with deterministic coefficients and known initial value, and $Y=\widehat W+\int\widehat\alpha\,dt$. Thus the observed and innovation [filtrations](../../../../../filtration-probability-theory.md) coincide, supplying the natural Brownian information needed for replication. Consequently the observed stock dynamics are $dS_t/S_t=\sigma d\widehat W_t+\sigma\widehat\alpha_tdt$. Its observed [market price of risk](../../../../../market-price-of-risk.md) is $\kappa_t=\widehat\alpha_t-r/\sigma$, and its normalized [state-price density](../../../../../state-price-density.md) solves

$$
d\zeta_t=-\zeta_t(rdt+\kappa_td\widehat W_t),\qquad
\zeta_t=\exp\left(-rt-\int_0^t\kappa_sd\widehat W_s-\frac12\int_0^t\kappa_s^2ds\right).
$$

The posterior mean is unbounded, so bounded-coefficient [Novikov condition](../../../../../novikov-s-condition.md) reasoning from Question 2 is not available automatically. A direct finite-horizon argument supplies true pricing. Relative to driftless [Wiener measure](../../../../../wiener-measure.md) for $Y$, the Bayesian mixture has observation density

$$
L_t(Y_t)=\sqrt{\frac{\tau_0}{\tau_0+t}}\exp\left(\frac{(\tau_0\widehat\alpha_0+Y_t)^2}{2(\tau_0+t)}-\frac{\tau_0\widehat\alpha_0^2}{2}\right).
$$

A law with observation drift $k=r/\sigma$ instead has density $e^{kY_t-k^2t/2}$. Therefore

$$
\boxed{D_t=\frac{e^{kY_t-k^2t/2}}{L_t(Y_t)},\qquad \zeta_t=e^{-rt}D_t.}
$$

This is the [finite-horizon pricing density for Gaussian drift learning](../../../../../finite-horizon-pricing-density-for-gaussian-drift-learning.md). The ratio changes the physical observed law into a genuine probability law, hence has mean one. Indeed, differentiation of the explicit likelihood, using $dY_t=d\widehat W_t+\widehat\alpha_tdt$, gives

$$
d\log L_t=\widehat\alpha_t\,dY_t-\frac12\widehat\alpha_t^2dt,\qquad
d\log D_t=(k-\widehat\alpha_t)d\widehat W_t-\frac12(\widehat\alpha_t-k)^2dt.
$$

The [Itô formula](../../../../../ito-s-lemma.md) therefore gives $dD_t=-D_t\kappa_td\widehat W_t$, agreeing with the stochastic exponential above. Under this pricing law the stock drift is $\sigma k=r$.

For [logarithmic utility](../../../../../logarithmic-utility.md), terminal marginal utility is $1/w_T$. The [state-price budget constraint](../../../../../state-price-budget-constraint.md) and the marginal condition imply $w_T^*=1/(y\zeta_T)$ and $1/y=w_0$. Since $\zeta_Tw_T^*=w_0$ is constant, its conditional-expectation pricing process is constant as well. Thus the entire optimal wealth process is

$$
\boxed{w_t^*=\frac{w_0}{\zeta_t}.}
$$

Indeed, for any other nonnegative admissible terminal wealth $X$, the elementary inequality $\log(X/w_T^*)\leq X/w_T^*-1$ gives

$$
\mathbb E\log(X/w_T^*)\leq\mathbb E[\zeta_TX/w_0]-1\leq0.
$$

This directly verifies optimality. Expected candidate log wealth is finite because $\mathbb E\widehat\alpha_t^2=\widehat\alpha_0^2+\tau_0^{-1}-(\tau_0+t)^{-1}$ and its time integral is finite on every fixed horizon. Applying the [Itô formula](../../../../../ito-s-lemma.md) to $1/\zeta$ gives

$$
\frac{dw_t^*}{w_t^*}=(r+\kappa_t^2)dt+\kappa_td\widehat W_t.
$$

The observed [self-financing portfolio](../../../../../self-financing-portfolio.md) with risky dollar fraction $\pi_t$ has diffusion coefficient $\pi_t\sigma$. Matching the coefficients proves the [log-optimal investment with Gaussian drift learning](../../../../../log-optimal-investment-with-gaussian-drift-learning.md) rule

$$
\boxed{\pi_t^*=\frac{\kappa_t}{\sigma}=\frac{\sigma\widehat\alpha_t-r}{\sigma^2},\qquad\theta_t^*=\pi_t^*w_t^*.}
$$

The remaining dollars are held in the [bank account](../../../../../bank-account.md); the fraction may be negative or exceed one because the question imposes neither short-sale nor borrowing restrictions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
