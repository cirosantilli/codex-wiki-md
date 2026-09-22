# Error control for ODE solvers

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

Error control selects discretization parameters and checks approximations against requested accuracy. [Local error estimators](local-error-estimator.md), [absolute and relative error tolerances](absolute-and-relative-error-tolerances.md) and an [adaptive step-size controller](adaptive-step-size-controller.md) provide practical local control. Propagation of defects determines the [global error](global-discretization-error.md), while stiffness, [roundoff error](round-off-error.md) and algebraic-solve accuracy impose additional limits.

For an [ordinary differential equation](ordinary-differential-equation.md), the practical loop is to propose a step, form a [local error estimator](local-error-estimator.md), scale it by [absolute and relative error tolerances](absolute-and-relative-error-tolerances.md), and accept or retry before choosing the next step. An [embedded Runge-Kutta pair](embedded-runge-kutta-pair.md) supplies two endpoints from shared [Runge-Kutta stages](runge-kutta-stage.md), making this extra accuracy check inexpensive. The [Euler-Heun embedded pair](euler-heun-embedded-pair.md) below exposes the distinction between the accepted formula's [order of a numerical method](order-of-a-numerical-method.md) and the estimator's step exponent; its [Adaptive Euler-Heun integration of exponential growth](adaptive-euler-heun-integration-of-exponential-growth.md) shows accepted local tests alongside accumulated [global error](global-discretization-error.md).

**Table of contents**

- [Adaptive step-size controller](adaptive-step-size-controller.md)
- [Absolute and relative error tolerances](absolute-and-relative-error-tolerances.md)
- [Local error estimator](local-error-estimator.md)
  - [Predictor-corrector error estimation](predictor-corrector-error-estimation.md)
  - [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
    - [Euler-Heun embedded pair](euler-heun-embedded-pair.md)
      - [Adaptive Euler-Heun integration of exponential growth](adaptive-euler-heun-integration-of-exponential-growth.md)
  - [Step-doubling error estimation](step-doubling-error-estimation.md)
- [Adaptive Euler step doubling for exponential decay](adaptive-euler-step-doubling-for-exponential-decay.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
