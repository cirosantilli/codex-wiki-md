# Banking stock dividends versus reinvesting them

↑ **Parent:** [Continuous dividend yield](continuous-dividend-yield.md)

For a stock with constant [continuous dividend yield](continuous-dividend-yield.md) $\delta$, holding one fixed share and depositing each dividend in a bank account at rate $r$ gives the displayed wealth process. Since $dA_t=rA_tdt+\delta S_tdt$, this is a [self-financing portfolio](self-financing-portfolio.md): its only cash inflow to the bank is the dividend earned by its stock holding. A claim paying $nX_T$ is replicated by $n$ copies and costs $nX_t$, including the known accrued-dividend balance at time $t$.

A different claim paying only $nS_T$ costs $nS_te^{-\delta(T-t)}$ in the [Black-Scholes model](black-scholes-model.md) with dividends. It is replicated by $ne^{-\delta(T-t)}$ shares with dividends reinvested in new shares: the share count grows at rate $\delta$ and reaches $n$ at expiry. Thus banking dividends and reinvesting them produce distinct terminal payoffs and distinct current values, even though both strategies are self-financing.

## ↑ Ancestors (7)

1. [Continuous dividend yield](continuous-dividend-yield.md)
2. [Stock](stock.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2011/b/6/b/solution.md)
