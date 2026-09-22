# Black-Scholes equation with constant cash storage costs

↑ **Parent:** [Black-Scholes equation](black-scholes-equation.md)

If holding one unit of a commodity costs a constant cash amount $\delta\,dt$ for storage, its gain is $dS-\delta\,dt$. A delta hedge long a derivative and short $V_S$ commodity units has riskless drift $V_t+\tfrac12\sigma^2S^2V_{SS}+\delta V_S$ and value $V-SV_S$. Equating the drift to the bank return gives the displayed [Black-Scholes equation](black-scholes-equation.md). This is an additive cash carry term, unlike a proportional dividend or storage yield.

The corresponding pricing diffusion is $d\widehat S=(r\widehat S+\delta)dt+\sigma\widehat S\,dW$. A fixed-strike forward has value $S+\delta(1-e^{-r\tau})/r-Ke^{-r\tau}$, and [put-call parity](put-call-parity.md) gives that same value for a matching call minus put. Replication buys the commodity and a bank reserve equal to the present value of its future storage payments. For $r=0$, the reserve is $\delta\tau$.

## ↑ Ancestors (7)

1. [Black-Scholes equation](black-scholes-equation.md)
2. [Black-Scholes model](black-scholes-model.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2010/b/6/a/solution.md)
