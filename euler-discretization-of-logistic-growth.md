# Euler discretization of logistic growth

↑ **Parent:** [Logistic differential equation](logistic-differential-equation.md)

The [Forward Euler method](euler-method.md) applied to the [logistic differential equation](logistic-differential-equation.md) $y'=ry(1-ay)$ becomes the [logistic map](logistic-map.md) after $u=a(\lambda-1)y/\lambda$, $\lambda=1+r\Delta t$. The positive [equilibrium point](equilibrium-point-of-a-dynamical-system.md) of the [differential equation](differential-equation-split.md) has perturbations decaying as $e^{-rt}$. Its discrete [fixed-point multiplier](multiplier-of-a-periodic-orbit-of-an-iteration.md) is $1-r\Delta t=2-\lambda$: for $r\Delta t>2$, the discretization has an artificial oscillatory [instability](instability.md), leading initially to alternation on successive steps. This contrasts with the positive perturbation multiplier $e^{-r\Delta t}$ of the exact time-step map.

## ↑ Ancestors (8)

1. [Logistic differential equation](logistic-differential-equation.md)
2. [Nonlinear ordinary differential equation](nonlinear-ordinary-differential-equation.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/6d/solution.md)
