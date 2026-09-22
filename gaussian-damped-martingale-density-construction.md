# Gaussian-damped martingale density construction

↑ **Parent:** [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)

For a finite-dimensional discounted gain [random vector](random-vector.md) $X$, absence of [arbitrage](arbitrage.md) means $h\cdot X\geq0$ almost surely only when $h\cdot X=0$ almost surely. Let $N=\{h:h\cdot X=0\text{ almost surely}\}$ and minimize $F(h)=\mathbb E e^{-|X|^2-h\cdot X}$ on the [orthogonal complement](orthogonal-complement.md) $N^\perp$. The Gaussian damping makes $F$ finite and differentiable without physical integrability assumptions on $X$. Every nonzero direction in $N^\perp$ has negative gains on an event of positive [probability](probability.md); compactness of directions proves [coercivity](coercive-function.md). At a minimizer, differentiation gives $\mathbb E[Xe^{-|X|^2-h_*\cdot X}]=0$. Normalizing the positive weight produces an [equivalent martingale measure](risk-neutral-measure.md) with integrable gains. This is a constructive one-period proof of the [fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md) even on an infinite [probability space](probability-space.md).

## ↑ Ancestors (6)

1. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/1/solution.md)
