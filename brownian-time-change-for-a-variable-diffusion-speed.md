# Brownian time change for a variable diffusion speed

↑ **Parent:** [Martingale problem](martingale-problem.md)

Let $\theta:\mathbb R^d\to(0,\Theta]$ be a [Borel measurable function](borel-measurable-function.md) bounded away from zero on every compact set. If $B$ is standard $d$-dimensional [Brownian motion](brownian-motion-split.md), the displayed clock is finite on compact intervals, continuous, strictly increasing, and unbounded. Its inverse $\tau_t=A^{-1}(t)$ is a Brownian [stopping time](stopping-time.md), with $\tau_t\leq2\Theta t$. The [optional sampling theorem](optional-sampling-theorem-for-a-supermartingale.md) and the change of variables $d\tau_t=2\theta(B_{\tau_t})dt$ show that $X_t=B_{\tau_t}$ solves the [martingale problem](martingale-problem.md) for $\mathcal L=\theta\Delta$ on [test functions](test-function.md) $C_c^\infty(\mathbb R^d)$. The [filtration](filtration-probability-theory.md) is $\mathcal F^B_{\tau_t}$. These are true [martingales](martingale-split.md): on a finite new-time horizon the sampling times have a deterministic bound. Continuous strictly positive $\theta$ satisfies the compact-set lower bound. Pointwise positivity alone does not; [pointwise positivity does not ensure weak existence](pointwise-positivity-does-not-ensure-weak-existence.md) gives a counterexample.

## ↑ Ancestors (9)

1. [Martingale problem](martingale-problem.md)
2. [Stochastic differential equation](stochastic-differential-equation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-stochastic-differential-equations-course-of-the-university-of-oxford/2025/1/b/i/solution.md)
- [Pointwise positivity does not ensure weak existence](pointwise-positivity-does-not-ensure-weak-existence.md)
