# Gaussian exponential martingale with deterministic variance

↑ **Parent:** [Gaussian process](gaussian-process.md)

Let $X_0=0$ and let $X$ be a centered [Gaussian process](gaussian-process.md) whose increments are independent of the past [filtration](filtration-probability-theory.md), with deterministic variance $v(t)$. Its displayed exponential is a positive [martingale](martingale-split.md). Indeed, $X_t-X_s$ is a centered [Gaussian random variable](gaussian-random-variable.md) with variance $v(t)-v(s)$, so the [Gaussian moment-generating function](moment-generating-function-of-a-normal-distribution.md) gives

$$
\mathbb E[M_t\mid\mathcal F_s]=M_s\mathbb E\exp(X_t-X_s-(v(t)-v(s))/2)=M_s.
$$

The sign-reversed process has the same variance and the same conclusion. Continuity of paths is unnecessary for this conditional-expectation argument.

## ↑ Ancestors (7)

1. [Gaussian process](gaussian-process.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gaussian forward-rate covariance drift restriction](gaussian-forward-rate-covariance-drift-restriction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/6/solution.md)
