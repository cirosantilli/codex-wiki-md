<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $T=t_0$, $\tau=T-t$, $x=S_t>0$, and $\sigma>0$. Use a dividend-free [Black-Scholes model](../../../../../black-scholes-model.md) with constant [interest rate](../../../../../interest-rate.md) $\rho$. The terminal payoff is assumed independent of the parameters being varied. In addition to twice differentiability, impose enough [integrability](../../../../../integrability.md) to differentiate the pricing formula; for example, $f,f',f''$ of polynomial growth suffice. Twice differentiability alone is not enough: the smooth payoff $f(x)=e^{x^2}$ has infinite [expectation](../../../../../expected-value.md) under every nondegenerate [lognormal distribution](../../../../../log-normal-distribution.md).

Under the [risk-neutral measure](../../../../../risk-neutral-measure.md) $Q$, future [stock](../../../../../stock.md) values conditional on $S_t=x$ have the form

$$
S_T=xM,\qquad M=\exp\left((\rho-\sigma^2/2)\tau+\sigma\sqrt\tau Z\right),\qquad Z\sim N(0,1).
$$

[Claim replication](../../../../../claim-replication.md), or equivalently the [martingale](../../../../../martingale-split.md) property of discounted value in the [complete market](../../../../../complete-market.md), gives

$$
\boxed{p(x,t)=e^{-\rho\tau}\mathbb E[f(xM)]
=\frac{e^{-\rho\tau}}{\sqrt{2\pi}}\int_{\mathbb R}f\left(xe^{(\rho-\sigma^2/2)\tau+\sigma\sqrt\tau z}\right)e^{-z^2/2}\,dz.}
$$

The [replicating strategy](../../../../../replicating-strategy.md) holds the [option delta](../../../../../option-delta.md) $p_x$ shares and bank-account value $\beta=p-xp_x$. No physical [drift](../../../../../drift-coefficient.md) parameter appears: the [Girsanov theorem](../../../../../girsanov-theorem.md) replaces the physical [drift](../../../../../drift-coefficient.md) by $\rho$ under the pricing measure, and the replication argument cancels it directly. The [risk-neutral pricing](../../../../../risk-neutral-pricing.md) operator is linear in the payoff and preserves pointwise payoff inequalities.

Here is a verification of the [Black-Scholes equation](../../../../../black-scholes-equation.md) using the integral itself. Differentiation in spot gives

$$
p_x=e^{-\rho\tau}\mathbb E[Mf'(xM)],\qquad
p_{xx}=e^{-\rho\tau}\mathbb E[M^2f''(xM)].
$$

Differentiating with respect to $\tau$ gives

$$
p_\tau=-\rho p+e^{-\rho\tau}\mathbb E\left[S_Tf'(S_T)
\left(\rho-\frac{\sigma^2}{2}+\frac{\sigma Z}{2\sqrt\tau}\right)\right].
$$

For $G(Z)=S_Tf'(S_T)$, the [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) identity $\mathbb E[ZG]=\mathbb E[G']$ yields

$$
\mathbb E[Z S_Tf'(S_T)]
=\sigma\sqrt\tau\,\mathbb E[S_Tf'(S_T)+S_T^2f''(S_T)].
$$

Substitution cancels the $-\sigma^2/2$ term and proves

$$
p_\tau=-\rho p+\rho xp_x+\tfrac12\sigma^2x^2p_{xx}.
$$

Since $p_t=-p_\tau$, this is precisely the [Black-Scholes equation](../../../../../black-scholes-equation.md). As $\tau\downarrow0$, $M\to1$ and growth control permits passage to the limit, giving $p(x,T)=f(x)$. The [delta hedge](../../../../../delta-hedge.md) then supplies the admissible replicating gains under the same regularity assumptions.

The [Black-Scholes parameter sensitivities](../../../../../black-scholes-parameter-sensitivities.md) describe the dependence on the model parameters without assuming a particular payoff. If $f$ is increasing, then $p_x\geq0$. If $f$ is [convex](../../../../../convex-function.md), then $p_{xx}\geq0$, so its price is [convex](../../../../../convex-function.md) in spot. The [option gamma](../../../../../option-gamma.md) $p_{xx}$ measures the response of the [option delta](../../../../../option-delta.md) to spot changes.

For the [interest rate](../../../../../interest-rate.md), the distribution of the future [stock](../../../../../stock.md) also changes with $\rho$, so looking only at discounting gives the wrong general answer. Differentiation gives the [option rho](../../../../../option-rho.md)

$$
\boxed{p_\rho=-\tau p+\tau e^{-\rho\tau}\mathbb E[S_Tf'(S_T)]
=\tau(xp_x-p)=-\tau\beta.}
$$

Thus a short bank-account position gives positive rate sensitivity, while a positive bank-account position gives negative rate sensitivity. For a cash payoff the result is negative; for the payoff $f(x)=x$ it is zero.

For [spot volatility](../../../../../spot-volatility.md), differentiate the lognormal multiplier and then use [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md):

$$
\begin{aligned}
p_\sigma&=e^{-\rho\tau}\mathbb E[S_Tf'(S_T)(\sqrt\tau Z-\sigma\tau)]\\
&=\sigma\tau e^{-\rho\tau}\mathbb E[S_T^2f''(S_T)]
=\boxed{\sigma\tau x^2p_{xx}}.
\end{aligned}
$$

Consequently a [convex](../../../../../convex-function.md) payoff has nonnegative [option vega](../../../../../option-vega.md). This monotonicity can also be understood by a mean-preserving increase of dispersion in the discounted [stock](../../../../../stock.md). Strict positivity requires nonzero curvature seen with positive probability; an affine payoff has zero [option vega](../../../../../option-vega.md).

Time enters through the remaining maturity $\tau$. Holding spot fixed, the [Black-Scholes equation](../../../../../black-scholes-equation.md) gives

$$
\boxed{p_t=\rho\beta-\tfrac12\sigma^2x^2p_{xx},\qquad p_T=-p_t.}
$$

Under the conventional assumption $\rho\geq0$, a [convex](../../../../../convex-function.md) payoff and a short bond position $\beta<0$ imply $p_t\leq0$. The inequality is strict if $\rho>0$, or if $p_{xx}>0$ with positive volatility. Thus the price at fixed [stock](../../../../../stock.md) value is nonincreasing in calendar time, and nondecreasing in maturity, under these hypotheses. It is not a claim that the realized stochastic price path decreases: that path still has Brownian exposure $\sigma S_tp_x\,dW_t^Q$.

The printed conclusion needs the nonnegative-rate qualification; it is false for arbitrary negative rates. For $K>0$, the twice-differentiable [convex](../../../../../convex-function.md) payoff $f(x)=x-K$ has

$$
p=x-Ke^{-\rho\tau},\qquad\beta=-Ke^{-\rho\tau}<0,\qquad
p_t=-\rho Ke^{-\rho\tau}>0\quad\text{if }\rho<0.
$$

This is an exact counterexample, not a failure of the pricing formula. Also, with $\rho=0$ and an affine payoff, “decreasing” can only mean nonincreasing. Without payoff monotonicity or the specified bond-position sign, neither the spot nor rate nor time sensitivity has a universal sign. Any additional payoff parameter, such as a strike, is differentiated through $f$; pointwise payoff ordering, rather than a generic parameter rule, determines its price effect.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
