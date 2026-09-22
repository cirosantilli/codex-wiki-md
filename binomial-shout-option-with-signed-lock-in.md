# Binomial shout option with signed lock-in

↑ **Parent:** [American option](american-option.md)

A holder may choose a shout time $\tau$ and receive $\max(S_T-S_\tau,0)+S_\tau-K=\max(S_T,S_\tau)-K$, or choose no shout and receive $(S_T-K)^+$. The lock-in term is signed, so shouting below strike can create a negative payoff. Backward induction must compare this actual contract with waiting. For $S_0=100$, multipliers $1.1,0.9$, bank growth $1.05$, strike 101 and two periods, the optimal policy waits at zero, shouts after the first up move, and never shouts after the first down move. The risk-neutral price is $575/49$. Claim payoffs at a recombined stock node can differ according to earlier shout history.

## ↑ Ancestors (6)

1. [American option](american-option.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2008/b/8/d/solution.md)
