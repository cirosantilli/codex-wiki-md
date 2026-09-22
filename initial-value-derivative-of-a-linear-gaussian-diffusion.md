# Initial-value derivative of a linear Gaussian diffusion

↑ **Parent:** [Strong solution of a stochastic differential equation](strong-solution-of-a-stochastic-differential-equation.md)

For $dX=\mu(t)Xdt+\sigma(t)dB$ with deterministic coefficients, $X(t,x)=a(t)[x+\int_0^ta(s)^{-1}\sigma(s)dB_s]$, where $a(t)=\exp(\int_0^t\mu)$. The random part does not depend on the initial value. For $f\in C_b^1$, the [mean value theorem](mean-value-theorem.md) bounds the initial-value difference quotient by $a(t)\|f'\|_\infty$, and [dominated convergence theorem](dominated-convergence-theorem.md) gives the displayed [derivative](derivative.md). The transition law is normal with mean $a(t)x$ and variance $\int_0^t\exp(2\int_s^t\mu)\sigma(s)^2ds$.

## ↑ Ancestors (9)

1. [Strong solution of a stochastic differential equation](strong-solution-of-a-stochastic-differential-equation.md)
2. [Stochastic differential equation](stochastic-differential-equation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
