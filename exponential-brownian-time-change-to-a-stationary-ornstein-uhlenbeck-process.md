# Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process

↑ **Parent:** [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md)

For $\lambda>0$, set $\mathcal G_t=\mathcal F_{e^{2\lambda t}}$ and $W_t=(2\lambda)^{-1/2}\int_1^{e^{2\lambda t}}u^{-1/2}dB_u$. This is a [Brownian motion](brownian-motion-split.md) in the new [filtration](filtration-probability-theory.md); its independent Gaussian increments have variance equal to elapsed time. The [Itô product rule](ito-product-rule.md) gives $dY=\sqrt{2\lambda}\,dW-\lambda Y\,dt$. Its initial value is $B_1$, independent of future W increments, and its [covariance function](covariance-function.md) is $e^{-\lambda|t-s|}$. Consequently it is a stationary [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md). The quadratic variation of the unscaled time change is $e^{2\lambda t}-1$, not $e^{2\lambda t}$.

## ↑ Ancestors (8)

1. [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md)
2. [Gaussian process](gaussian-process.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30/3/c/solution.md)
