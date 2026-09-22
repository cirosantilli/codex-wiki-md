# Mean-square fundamental theorem of calculus

↑ **Parent:** [Mean-square derivative of a Gaussian process](mean-square-derivative-of-a-gaussian-process.md)

If an [L2 space](l2-space-is-a-hilbert-space.md)-valued map $X$ has a continuous mean-square derivative $Y$, then its increments equal the [Bochner integral](bochner-integral.md) of $Y$. To see this, for each partition interval $[t_j,t_{j+1}]$, continuous linear observations and the scalar mean-value bound give $\|X(t_{j+1})-X(t_j)-(t_{j+1}-t_j)Y(t_j)\|_2\leq(t_{j+1}-t_j)\sup_{u\in[t_j,t_{j+1}]}\|Y(u)-Y(t_j)\|_2$. Sum these errors. Uniform continuity of $Y$ makes the total error tend to zero as the mesh tends to zero, while the [Riemann sums](riemann-sum.md) converge to the [Bochner integral](bochner-integral.md). This proves the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) in [L2 space](l2-space-is-a-hilbert-space.md). If a [Gaussian process](gaussian-process.md) derivative also has a [continuous modification](continuous-modification.md), its anchored path integral $X(s)+\int_s^t\widetilde Y(u)\,du$ therefore produces a differentiable [modification of a stochastic process](modification-of-a-stochastic-process.md) of the original [Gaussian process](gaussian-process.md).

## ↑ Ancestors (8)

1. [Mean-square derivative of a Gaussian process](mean-square-derivative-of-a-gaussian-process.md)
2. [Gaussian process](gaussian-process.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Differentiable modification of a stationary Gaussian process](differentiable-modification-of-a-stationary-gaussian-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217/2/solution.md)
