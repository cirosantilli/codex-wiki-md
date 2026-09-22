# Factorial Picard estimate for a linear stochastic differential equation

↑ **Parent:** [Stochastic differential equation](stochastic-differential-equation.md)

For $dy=\sum_iA^iy\,dB^i$ with constant linear maps, let $K=\sum_i\|A^i\|_{\mathrm{op}}^2$ and let $D_m$ be consecutive [Picard iterate](picard-iterate.md) differences starting from $y^{(0)}=a$. The vector [Itô isometry](ito-isometry.md) gives $\mathbb E|D_m(t)|^2\leq K\int_0^t\mathbb E|D_{m-1}(s)|^2ds$, proving the displayed estimate by induction. The square roots of these factorial bounds are summable on bounded time intervals. The [Doob L2 maximal inequality](doob-l2-maximal-inequality.md) then makes $\sum_m\mathbb E\sup_{t\leq T}|D_m(t)|$ finite. [Tonelli's theorem](tonelli-theorem.md) proves absolute uniform almost-sure convergence of the iterations, in addition to their $L^2$ convergence.

## ↑ Ancestors (8)

1. [Stochastic differential equation](stochastic-differential-equation.md)
2. [Stochastic calculus](stochastic-calculus-split.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford/2010/a/1/c/solution.md)
