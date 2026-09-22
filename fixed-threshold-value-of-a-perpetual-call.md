# Fixed-threshold value of a perpetual call

↑ **Parent:** [Perpetual American call option](perpetual-american-call-option.md)

For the [perpetual American call option](perpetual-american-call-option.md) model and a fixed [exercise threshold](exercise-threshold.md) $B>K$, this is the discounted [expectation](expected-value-split.md) of $B-K$ at its first hit, with zero payoff if the hit never occurs. The stationary [ordinary differential equation](ordinary-differential-equation.md) and boundary conditions $C_B(0)=0$, $C_B(B)=B-K$ prove the formula. At fixed $S<B$, differentiation gives $\partial_BC_B=S^pB^{-p-1}[pK-(p-1)B]$, so the unique maximizing threshold is $pK/(p-1)$. If a larger threshold is imposed, $C_B'(B-)>1$ and its value lies below immediate exercise payoff just below $B$. This is allowed for a committed policy, but violates the exercise lower bound if quoted for an unrestricted [American call option](american-call-option.md).

## ↑ Ancestors (8)

1. [Perpetual American call option](perpetual-american-call-option.md)
2. [American call option](american-call-option.md)
3. [American option](american-option.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2017/3/c/solution.md)
