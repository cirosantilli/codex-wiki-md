# Pointwise positivity does not ensure weak existence

↑ **Parent:** [Weak solution of a stochastic differential equation](weak-solution-of-a-stochastic-differential-equation.md)

There need not be a [weak solution of a stochastic differential equation](weak-solution-of-a-stochastic-differential-equation.md) $dX_t=\sqrt{2\theta(X_t)}dB_t$, $X_0=0$, even when $\theta$ is a bounded [Borel measurable function](borel-measurable-function.md) strictly positive everywhere. For the displayed example, any solution would be a [continuous local martingale](continuous-local-martingale.md) with $[X]_t=2\int_0^t\theta(X_s)ds\leq2t$, hence a [square-integrable](square-integrable-function.md) [martingale](martingale-split.md). The [occupation-times formula](occupation-times-formula.md) applied to $\mathbf1_{\{0\}}$ gives $0=\int_0^t\mathbf1_{\{X_s=0\}}d[X]_s=2\int_0^t\mathbf1_{\{X_s=0\}}ds$. Since $\theta(x)\leq x^2$ away from zero, $\mathbb EX_t^2\leq2\int_0^t\mathbb EX_s^2ds$. The [Gronwall inequality](gronwall-inequality.md) makes $X\equiv0$, a contradiction. Thus a [diffusion amplitude](diffusion-amplitude.md) positive at a single problematic point cannot repair arbitrarily slow neighbouring motion. A local positive lower bound, as in the [Brownian time change for a variable diffusion speed](brownian-time-change-for-a-variable-diffusion-speed.md), rules out this example.

## ↑ Ancestors (9)

1. [Weak solution of a stochastic differential equation](weak-solution-of-a-stochastic-differential-equation.md)
2. [Stochastic differential equation](stochastic-differential-equation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Brownian time change for a variable diffusion speed](brownian-time-change-for-a-variable-diffusion-speed.md)
- [Solution](past-exam-of-the-stochastic-differential-equations-course-of-the-university-of-oxford/2025/1/b/i/solution.md)
