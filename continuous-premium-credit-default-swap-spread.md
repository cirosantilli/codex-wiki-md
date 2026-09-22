# Continuous-premium credit-default swap spread

↑ **Parent:** [Credit default swap](credit-default-swap.md)

Assume deterministic [discount factors](discount-factor.md), deterministic risk-neutral [default intensity](default-intensity.md) $\lambda$, fixed fractional recovery $\mathcal R$, and continuous premium until [default](credit-default.md) or maturity. Survival is $G(t)=\exp(-\int_0^t\lambda(u)du)$. Expected discounted protection is $N(1-\mathcal R)\int B\lambda G$, while premium is $Ns\int BG$. Equating them gives the par spread. Constant intensity gives $s=(1-\mathcal R)\lambda$. Discrete premiums, [default](credit-default.md) accrual, stochastic recovery and counterparty losses require changing the corresponding cash-flow [expectations](expected-value.md).

## ↑ Ancestors (8)

1. [Credit default swap](credit-default-swap.md)
2. [Credit derivative](credit-derivative.md)
3. [Financial asset](financial-asset.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32/5/solution.md)
