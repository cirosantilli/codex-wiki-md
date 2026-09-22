# Maturity monotonicity of calls with nonnegative strikes

↑ **Parent:** [European call option](european-call-option.md)

If the [bank account](bank-account.md) $B$ is positive and nondecreasing and $S/B$ is a [martingale](martingale-split.md) under an [equivalent martingale measure](risk-neutral-measure.md) $Q$, then for $K\geq0$ the European call price $C(T,K)$ is nondecreasing in $T$. Put $M_t=S_t/B_t$. For $u\geq t$, $K/B_u\leq K/B_t$ and hence $(M_u-K/B_u)^+\geq(M_u-K/B_t)^+$. Conditional convexity gives $\mathbb E_Q[(M_u-K/B_t)^+\mid\mathcal F_t]\geq(M_t-K/B_t)^+$. Taking expectations and multiplying by $B_0$ proves the claim. The result is not generally true for negative strikes: with $S_t=B_t=e^{rt}$ and $r>0$, a negative-strike call costs $1-Ke^{-rT}$, decreasing in maturity.

## ↑ Ancestors (7)

1. [European call option](european-call-option.md)
2. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/2/iii/solution.md)
