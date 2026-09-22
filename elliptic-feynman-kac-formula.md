# Elliptic Feynman-Kac formula

↑ **Parent:** [Feynman-Kac formula](feynman-kac-formula.md)

For a bounded domain, a bounded [classical solution](classical-solution.md) with boundary data $g$, nonnegative bounded $V$, bounded $f$ and integrable diffusion exit time $\tau$ satisfies

$$
u(x)=\mathbb E_x\left[e^{-\int_0^\tau V(X_r)dr}g(X_\tau)+\int_0^\tau e^{-\int_0^sV(X_r)dr}f(X_s)ds\right].
$$

Apply the [Itô product rule](ito-product-rule.md) to the discounted stopped solution and add its source integral. The stopped martingale is dominated by $\|u\|_\infty+\|f\|_\infty\tau$, so [dominated convergence](dominated-convergence-theorem.md) permits passage to the exit. For $V=f=0$, this is a boundary-value averaging principle for functions harmonic under $L$.

## ↑ Ancestors (10)

1. [Feynman-Kac formula](feynman-kac-formula.md)
2. [Kolmogorov backward equation](kolmogorov-backward-equation.md)
3. [Stochastic differential equation](stochastic-differential-equation.md)
4. [Stochastic calculus](stochastic-calculus-split.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38/5/solution.md)
