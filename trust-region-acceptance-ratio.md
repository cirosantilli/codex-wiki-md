# Trust-region acceptance ratio

↑ **Parent:** [Trust region](trust-region.md)

For positive predicted decrease, the [trust-region acceptance ratio](trust-region-acceptance-ratio.md) compares the actual decrease with the model decrease. A ratio near one supports the local model; a negative ratio means the trial increased the [objective function](objective-function.md). A typical algorithm rejects and shrinks the [trust region](trust-region.md) when $\rho_k<\eta_1$, accepts it when $\rho_k\geq\eta_1$, and enlarges the radius after a very successful boundary step with $\rho_k>\eta_2$, where $0<\eta_1<\eta_2<1$.

## ↑ Ancestors (5)

1. [Trust region](trust-region.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/2/a/ii/solution.md)
- [Trust region](trust-region.md)
- [Trust-region acceptance ratio](trust-region-acceptance-ratio.md)
- [Trust-region method](trust-region-method.md)
