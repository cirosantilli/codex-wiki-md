# Delta of a squared positive-part call

↑ **Parent:** [Option delta](option-delta.md)

For [contingent claim payoff](contingent-claim-payoff.md) $(S_T-K)_+^2$ in the non-dividend [Black-Scholes model](black-scholes-model.md), differentiating the discounted [expected value](expected-value-split.md) gives $\Delta=2e^{-r\tau}S^{-1}\mathbb E[(S_T^2-KS_T)\mathbf1_{\{S_T\geq K\}}]$. Completing the square in the Gaussian exponent computes each truncated [lognormal](log-normal-distribution.md) moment and yields the displayed formula, where $d_1=(\log(S/K)+(r+\sigma^2/2)\tau)/(\sigma\sqrt\tau)$. Its terminal limit is $2(S-K)_+$.

## ↑ Ancestors (7)

1. [Option delta](option-delta.md)
2. [Greeks (finance)](greeks-finance.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2007/b/6/d/solution.md)
