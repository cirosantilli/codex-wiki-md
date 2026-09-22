<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $T=t_0$, $\tau=T-t$, and let $N$ have the [standard normal distribution](../../../../../standard-normal-distribution.md). For a twice [differentiable](../../../../../differentiable-function.md) payoff with enough growth control for the following [expectations](../../../../../expected-value.md) and derivatives, [risk-neutral pricing](../../../../../risk-neutral-pricing.md) in the dividend-free [Black-Scholes model](../../../../../black-scholes-model.md) gives

$$
\boxed{V(x,t)=e^{-\rho\tau}\mathbb E[f(xM)],\qquad
M=e^{(\rho-\sigma^2/2)\tau+\sigma\sqrt\tau N}.}
$$

The conditional discounted payoff is a [martingale](../../../../../martingale-split.md) under the [risk-neutral measure](../../../../../risk-neutral-measure.md). Applying the [Itô formula](../../../../../ito-s-lemma.md) to $e^{-\rho s}V(S_s,s)$ and setting its [drift](../../../../../drift-coefficient.md) to zero therefore gives the [Black-Scholes equation](../../../../../black-scholes-equation.md)

$$
\boxed{V_t+\frac12\sigma^2x^2V_{xx}+\rho xV_x-\rho V=0,\qquad V(x,T)=f(x).}
$$

The [delta hedge](../../../../../delta-hedge.md) holds $\Delta=V_x$ shares; the remaining bond value is $\beta=V-x\Delta$, or $h=\beta/e^{-\rho(T-t)}$ units of the [zero-coupon bond](../../../../../zero-coupon-bond.md). Substitution in the [Itô formula](../../../../../ito-s-lemma.md) and the displayed equation gives $dV=\Delta\,dS+h\,dB$, proving replication and [self-financing](../../../../../self-financing-portfolio.md).

Differentiating the pricing expectation in the current [stock](../../../../../stock.md) price gives its [option delta](../../../../../option-delta.md) and [option gamma](../../../../../option-gamma.md):

$$
\Delta=e^{-\rho\tau}\mathbb E[f'(xM)M],\qquad
\Gamma=e^{-\rho\tau}\mathbb E[f''(xM)M^2].
$$

Thus a nondecreasing payoff has a nondecreasing price; a nonincreasing payoff has a nonincreasing price. A [convex](../../../../../convex-function.md) payoff has $\Gamma\geq0$, and a [concave](../../../../../concave-function.md) payoff has $\Gamma\leq0$. This is [convexity preservation in Black-Scholes pricing](../../../../../convexity-preservation-in-black-scholes-pricing.md).

The [Black-Scholes parameter sensitivities](../../../../../black-scholes-parameter-sensitivities.md) follow directly from the same expectation. Differentiation in the [interest rate](../../../../../interest-rate.md) gives the [option rho](../../../../../option-rho.md)

$$
\boxed{V_\rho=\tau(x\Delta-V)=-\tau\beta.}
$$

For [spot volatility](../../../../../spot-volatility.md), differentiation first gives

$$
V_\sigma=e^{-\rho\tau}\mathbb E[f'(xM)xM(\sqrt\tau N-\sigma\tau)].
$$

The [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) identity $\mathbb E[N\psi(N)]=\mathbb E[\psi'(N)]$, applied to $\psi(N)=f'(xM)xM$, cancels the term containing $f'$ and gives the [option vega](../../../../../option-vega.md)

$$
\boxed{V_\sigma=\sigma\tau x^2\Gamma.}
$$

Consequently increasing [spot volatility](../../../../../spot-volatility.md) increases a [convex](../../../../../convex-function.md) payoff's value and decreases a [concave](../../../../../concave-function.md) payoff's value, with weak inequalities in affine or degenerate cases. A short bond position gives positive [option rho](../../../../../option-rho.md), while a long bond position gives negative [option rho](../../../../../option-rho.md). The physical [stock](../../../../../stock.md) [drift](../../../../../drift-coefficient.md) $\mu$ does not enter these prices: the [risk-neutral measure](../../../../../risk-neutral-measure.md) replaces it by $\rho$.

The [option theta](../../../../../option-theta.md) is the calendar-time derivative at fixed current [stock](../../../../../stock.md) price. The [Black-Scholes equation](../../../../../black-scholes-equation.md) gives

$$
\boxed{V_t=\rho\beta-\frac12\sigma^2x^2\Gamma.}
$$

For $\rho\geq0$, a [convex](../../../../../convex-function.md) payoff with $\beta<0$ therefore has $V_t\leq0$, while a [concave](../../../../../concave-function.md) payoff with $\beta>0$ has $V_t\geq0$. The signs are strict when $\rho>0$. At $\rho=0$, an affine payoff can give equality. Remaining-maturity sensitivity is $V_T=-V_t$ when the payoff is independent of $T$. All these time comparisons hold at fixed current [stock](../../../../../stock.md) price.

The stated time-monotonicity conclusion needs the nonnegative-rate condition. For example, the [convex](../../../../../convex-function.md) affine payoff $f(x)=x-K$ has

$$
V=x-Ke^{-\rho(T-t)},\qquad \beta=-Ke^{-\rho(T-t)}<0,\qquad
V_t=-\rho Ke^{-\rho(T-t)}>0\quad(\rho<0).
$$

Thus with negative [interest rates](../../../../../interest-rate.md) it provides an explicit counterexample even though the replica is short in bonds.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
