# Linear stochastic differential equation

↑ **Parent:** [Stochastic differential equation](stochastic-differential-equation.md)

A [stochastic differential equation](stochastic-differential-equation.md) with drift and diffusion coefficients affine in its state. In the constant-coefficient additive-noise case $dX_t=(aX_t+b)dt+\sigma dW_t$, multiplying by $e^{-at}$ gives

$$
X_t=e^{at}\left(X_0+b\int_0^t e^{-au}\,du+\sigma\int_0^t e^{-au}\,dW_u\right).
$$

Consequently its conditional [distribution](distribution-mathematical-analysis.md) is [normal](normal-distribution.md), with mean $e^{a\tau}x+b(e^{a\tau}-1)/a$ and variance $\sigma^2(e^{2a\tau}-1)/(2a)$ when $a\ne0$. For $a=0$, these become $x+b\tau$ and $\sigma^2\tau$. Additive noise permits negative states; it differs from [geometric Brownian motion](geometric-brownian-motion.md).

## ↑ Ancestors (8)

1. [Stochastic differential equation](stochastic-differential-equation.md)
2. [Stochastic calculus](stochastic-calculus-split.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Linear drift change of measure](linear-drift-change-of-measure.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2017/1/a/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2021/1/b/solution.md)
