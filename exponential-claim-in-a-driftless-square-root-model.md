# Exponential claim in a driftless square-root model

↑ **Parent:** [Local volatility model](local-volatility-model.md)

In the zero-interest [local volatility model](local-volatility-model.md) $dS_t=\sqrt{S_t}\,dW_t^Q$, the [risk-neutral pricing](risk-neutral-pricing.md) value of the [European contingent claim](european-contingent-claim.md) $e^{vS_T}$, for $v>0$ and $v(T-t)<2$, is

$$
V(t,S_t)=\exp\left(\frac{vS_t}{1-v(T-t)/2}\right).
$$

The [compound Poisson transition law of a driftless square-root diffusion](compound-poisson-transition-law-of-a-driftless-square-root-diffusion.md) proves finiteness and this conditional-expectation formula. Alternatively, substituting $V(t,S)=e^{a(t)S+b(t)}$ into the [pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md) gives $a'+a^2/2=0$ and $b'=0$, with terminal values $a(T)=v,b(T)=0$. Hence $a(t)=v/[1-v(T-t)/2]$ and $b(t)=0$. The conditional-expectation calculation verifies that this formal solution is the price of the unbounded claim. The [delta hedge](delta-hedge.md) holds $a(t)V$ stocks and $(1-a(t)S_t)V/B_t$ bank units.

## ↑ Ancestors (7)

1. [Local volatility model](local-volatility-model.md)
2. [Local volatility](local-volatility.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/5/iii/solution.md)
