# Error control for ODE solvers

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

Error control selects discretization parameters and checks approximations against requested accuracy. [Local error estimators](local-error-estimator.md), [absolute and relative error tolerances](absolute-and-relative-error-tolerances.md) and an [adaptive step-size controller](adaptive-step-size-controller.md) provide practical local control. Propagation of defects determines the [global error](global-discretization-error.md), while stiffness, [roundoff error](round-off-error.md) and algebraic-solve accuracy impose additional limits.

**Table of contents**

- [Adaptive step-size controller](adaptive-step-size-controller.md)
- [Absolute and relative error tolerances](absolute-and-relative-error-tolerances.md)
- [Local error estimator](local-error-estimator.md)
  - [Predictor-corrector error estimation](predictor-corrector-error-estimation.md)
  - [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
  - [Step-doubling error estimation](step-doubling-error-estimation.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
