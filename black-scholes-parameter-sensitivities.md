# Black-Scholes parameter sensitivities

↑ **Parent:** [Black-Scholes model](black-scholes-model.md)

For a fixed twice-differentiable terminal payoff with sufficient growth control, differentiate its [lognormal distribution](log-normal-distribution.md) pricing integral. [Gaussian integration by parts](stein-s-lemma-probability.md) gives the displayed identities. Convexity implies $p_{xx}\geq0$, so increasing [spot volatility](spot-volatility.md) cannot lower the price. The [interest rate](interest-rate.md) sensitivity depends on the sign of the cash position $p-xp_x$. Calendar-time sensitivity is $p_t=\rho(p-xp_x)-\tfrac12\sigma^2x^2p_{xx}$. Thus a convex payoff with a negative cash position has a nonincreasing price at fixed spot when $\rho\geq0$. Negative rates invalidate that conclusion: $f(x)=x-K$ gives $p=x-Ke^{-\rho(T-t)}$ and $p_t=-\rho Ke^{-\rho(T-t)}>0$ when $\rho<0$.

**Table of contents**

- [Convexity preservation in Black-Scholes pricing](convexity-preservation-in-black-scholes-pricing.md)
- [Option rho](option-rho.md)
- [Option gamma](option-gamma.md)

## ↑ Ancestors (6)

1. [Black-Scholes model](black-scholes-model.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/5/solution.md)
