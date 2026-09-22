# Explicit Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](runge-kutta-method-split.md)

An explicit Runge-Kutta method has $a_{ij}=0$ whenever $j\geq i$. Its stage [matrix](matrix.md) is strictly lower triangular: compute each [Runge-Kutta stage](runge-kutta-stage.md) using already known slopes, starting with $Y_1=y_n$. In contrast, an [implicit Runge-Kutta method](implicit-runge-kutta-method.md) requires solving coupled stage equations, whose existence is addressed by [stage solvability of an implicit Runge-Kutta method](stage-solvability-of-an-implicit-runge-kutta-method.md).

**Table of contents**

- [Heun's method](heun-s-method.md)

## ↑ Ancestors (7)

1. [Runge-Kutta method](runge-kutta-method-split.md)
2. [One-step method](one-step-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Butcher tableau](butcher-tableau.md)
