# Parabolic Feynman-Kac formula with a source

↑ **Parent:** [Feynman-Kac formula](feynman-kac-formula.md)

For a nonexplosive [diffusion process](markov-diffusion.md), bounded source $f$, terminal data $g$ and nonnegative bounded potential $V$, a bounded [classical solution](classical-solution.md) with $u(T,x)=g(x)$ is

$$
u(t,x)=\mathbb E_{t,x}\left[e^{-\int_t^TV(X_r)dr}g(X_T)+\int_t^Te^{-\int_t^sV(X_r)dr}f(s,X_s)ds\right].
$$

The [Itô product rule](ito-product-rule.md) shows that the discounted solution plus its accumulated discounted source is a local martingale. Its deterministic finite-horizon bound upgrades it to a true martingale, giving the formula and uniqueness without a global derivative bound.

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
