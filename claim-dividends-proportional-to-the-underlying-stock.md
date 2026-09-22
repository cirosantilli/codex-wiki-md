# Claim dividends proportional to the underlying stock

↑ **Parent:** [Black-Scholes equation with claim dividends](black-scholes-equation-with-claim-dividends.md)

In the [Black-Scholes model](black-scholes-model.md), suppose a [stock](stock.md) pays [continuous dividend yield](continuous-dividend-yield.md) $q$, a claim pays cash flow $f(t)S_tdt$, and its terminal [financial payoff](contingent-claim-payoff.md) is $cS_T$. If the discounted cash-flow integral is finite, its [risk-neutral pricing](risk-neutral-pricing.md) value is the displayed expression. To derive it, substitute $V=S\phi(t)$ into the [Black-Scholes equation with claim dividends](black-scholes-equation-with-claim-dividends.md), including stock drift $(r-q)S$. This gives $\phi'-q\phi=-f$, $\phi(T)=c$, which an [integrating factor](integrating-factor.md) solves. The [interest rate](interest-rate.md) cancels because all payments are proportional to the same [stock](stock.md).

## ↑ Ancestors (8)

1. [Black-Scholes equation with claim dividends](black-scholes-equation-with-claim-dividends.md)
2. [Black-Scholes equation](black-scholes-equation.md)
3. [Black-Scholes model](black-scholes-model.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2008/b/7/d/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2023/1/b/solution.md)
