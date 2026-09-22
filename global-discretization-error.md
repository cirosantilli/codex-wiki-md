# Global discretization error

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

The [global error](global-discretization-error.md) is the difference between the computed and exact solutions after accumulated numerical steps, rather than the [local truncation error](local-truncation-error.md) of a single step started from exact data. An estimate for the [stability of a numerical method](stability-of-a-numerical-method.md) controls how initial errors and local defects accumulate. For a stable order-$p$ time integrator with starting errors $O(h^p)$, local defects $O(h^{p+1})$ accumulated over $O(1/h)$ steps give [global error](global-discretization-error.md) $O(h^p)$ on a fixed time interval.

**Table of contents**

- [Variable-step global ODE error bound](variable-step-global-ode-error-bound.md)
- [Residual bound for global ODE error](residual-bound-for-global-ode-error.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
