<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $T=t_0$, $\Delta=T-t$ and assume the payoff has sufficient integrability for [risk-neutral valuation](../../../../../risk-neutral-pricing.md). Under the [risk-neutral measure](../../../../../risk-neutral-measure.md) $Q$, the [Black-Scholes model](../../../../../black-scholes-model.md) has $dS_u=\rho S_u\,du+\sigma S_u\,dW_u^Q$, so conditionally on $S_t=x$,

$$
S_T=x\exp\left((\rho-\sigma^2/2)\Delta+\sigma\sqrt\Delta\,Z\right),\qquad Z\sim N(0,1).
$$

Absence of [arbitrage](../../../../../arbitrage.md) gives the time-$t$ price

$$
\boxed{V(x,t)=e^{-\rho\Delta}\mathbb E\left[f\left(xe^{(\rho-\sigma^2/2)\Delta+\sigma\sqrt\Delta Z}\right)\right].}
$$

For a regular payoff this is the solution of the [Black-Scholes equation](../../../../../black-scholes-equation.md) with terminal value $f$, and the [delta hedge](../../../../../delta-hedge.md) $g=V_x$ replicates it. Suitable limits or conditional-expectation representations extend the price formula beyond smooth terminal payoffs.

For the [logarithmic stock payoff](../../../../../logarithmic-stock-payoff.md), put $Y=(\rho-\sigma^2/2)\Delta+\sigma\sqrt\Delta Z$. Its [Gaussian moment-generating function](../../../../../moment-generating-function-of-a-normal-distribution.md) is $\mathbb Ee^Y=e^{\rho\Delta}$, while differentiating that moment gives $\mathbb E[Ye^Y]=(\rho+\sigma^2/2)\Delta e^{\rho\Delta}$. Therefore

$$
\boxed{V(x,t)=x\left[\log x+(\rho+\sigma^2/2)\Delta\right].}
$$

The [option delta](../../../../../option-delta.md) is $\log x+1+(\rho+\sigma^2/2)\Delta$, and the second [stock](../../../../../stock.md) derivative is $1/x$. The [Black-Scholes equation](../../../../../black-scholes-equation.md) can also be checked directly from $V_t=-x(\rho+\sigma^2/2)$.

For general convex $f$, let $Y_+=\exp((\rho-\sigma^2/2)\Delta+\sigma\sqrt\Delta Z)>0$. For $0\leq\lambda\leq1$, convexity gives

$$
f((\lambda x+(1-\lambda)y)Y_+)\leq\lambda f(xY_+)+(1-\lambda)f(yY_+).
$$

Taking the positive discounted expectation proves that $V(\cdot,t)$ is convex. Its derivative, where defined, is therefore nondecreasing, proving that the [stock](../../../../../stock.md) holding in the [delta hedge](../../../../../delta-hedge.md) rises weakly with the [stock](../../../../../stock.md) price. For twice differentiable $f$, differentiation gives $V_{xx}=e^{-\rho\Delta}\mathbb E[Y_+^2f''(xY_+)]\geq0$. For a merely convex payoff, Gaussian smoothing at $t<T$ and the usual growth assumptions give the same conclusion; one-sided derivatives are monotone even without smoothing. Strict increase is not implied by convexity alone: an affine payoff has constant [option delta](../../../../../option-delta.md).

For the [random constant Gaussian interest-rate mixture](../../../../../random-constant-gaussian-interest-rate-mixture.md), represent the rate as $\rho=\rho_0+\tau Y$, with $Y,Z$ independent standard normal variables. This independence simply represents averaging the constant-rate price function over its Gaussian parameter. Completing the square in $Y$ yields the identity

$$
\mathbb E[e^{-\tau TY}F(Y)]=e^{\tau^2T^2/2}\mathbb E[F(Y-\tau T)].
$$

Apply it inside the time-zero price formula:

$$
\begin{aligned}
\mathbb Ep(\rho,\sigma)
={}&e^{-\rho_0T+\tau^2T^2/2}\mathbb E\left[f\left(S_0e^{(\rho_0-\sigma^2/2-\tau^2T)T+\tau TY+\sigma\sqrt T Z}\right)\right].
\end{aligned}
$$

The combined normal term has variance $\tau^2T^2+\sigma^2T$. Define $\rho_* =\rho_0-\tau^2T/2$ and $\sigma_*^2=\sigma^2+\tau^2T$. Then the discount factor is $e^{-\rho_*T}$, and the log-price mean is $(\rho_*-\sigma_*^2/2)T$. Thus the expectation is exactly the constant-parameter [Black-Scholes model](../../../../../black-scholes-model.md) price with those parameters:

$$
\boxed{\mathbb Ep(\rho,\sigma)=p\left(\rho_0-\frac{\tau^2T}{2},\sqrt{\sigma^2+\tau^2T}\right).}
$$

The argument applies to nonnegative payoffs by [Tonelli theorem](../../../../../tonelli-theorem.md), and to signed payoffs whenever absolute integrability justifies the expectations. It averages constant-rate prices; it does not assume a stochastic short-rate process.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
