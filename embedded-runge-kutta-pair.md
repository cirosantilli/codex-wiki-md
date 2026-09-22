# Embedded Runge-Kutta pair

↑ **Parent:** [Local error estimator](local-error-estimator.md)

Two [Runge-Kutta methods](runge-kutta-method.md) share a stage matrix and nodes but use different output weights. An order-$p$ and order-$q$ pair with $q<p$ gives an output difference generally of order $h^{q+1}$, estimating the lower-order defect. Shared stage evaluations reduce the cost. The [adaptive step-size controller](adaptive-step-size-controller.md) exponent must reflect this estimator order, rather than blindly the higher reported solution order.

## ↑ Ancestors (7)

1. [Local error estimator](local-error-estimator.md)
2. [Error control for ODE solvers](error-control-for-ode-solvers.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Local error estimator](local-error-estimator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/6/solution.md)
