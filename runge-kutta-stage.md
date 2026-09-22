# Runge-Kutta stage

↑ **Parent:** [Runge-Kutta method](runge-kutta-method-split.md)

A Runge-Kutta stage consists of a trial state $Y_i$ at the time node $t_n+c_i h$ and the corresponding [vector field](vector-field.md) evaluation $k_i$. In the slope convention, $Y_i=y_n+h\sum_ja_{ij}k_j$. Stages belong to the construction of one [Runge-Kutta method](runge-kutta-method-split.md) step; they need not have the same accuracy as its final output. Stage states can leave the physically allowed region even when the endpoint lies inside it, so $f$ must be defined at every stage used.

## ↑ Ancestors (7)

1. [Runge-Kutta method](runge-kutta-method-split.md)
2. [One-step method](one-step-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Butcher tableau](butcher-tableau.md)
- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
- [Euler-Heun embedded pair](euler-heun-embedded-pair.md)
- [Explicit Runge-Kutta method](explicit-runge-kutta-method.md)
- [Heun's method](heun-s-method.md)
- [Runge-Kutta method](runge-kutta-method-split.md)
