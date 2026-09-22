# Local error estimator

↑ **Parent:** [Error control for ODE solvers](error-control-for-ode-solvers.md)

A local error estimator approximates a numerical step's defect from the exact solution starting at the same input. Differences between formulas estimate error only after their asymptotic orders and constants are accounted for. [Step-doubling error estimation](step-doubling-error-estimation.md), an [embedded Runge-Kutta pair](embedded-runge-kutta-pair.md) and [predictor-corrector error estimation](predictor-corrector-error-estimation.md) are common constructions. They do not by themselves bound accumulated [global error](global-discretization-error.md).

Let $\Phi_h(t_n,y_n)$ be the exact endpoint of the [ordinary differential equation](ordinary-differential-equation.md) started at the numerical value $y_n$, and let $Y_{n+1}$ be the candidate numerical endpoint. The signed local defect being estimated is $\ell_{n+1}=\Phi_h(t_n,y_n)-Y_{n+1}$. In contrast, actual [global error](global-discretization-error.md) compares $Y_{n+1}$ with the solution of the original [initial value problem](initial-value-problem.md), including all previous steps. The [local truncation error](local-truncation-error.md) convention inserts original exact data instead. These starting-value distinctions matter even when the same formula is used for every step. A practical [local error estimator](local-error-estimator.md) also relies on a smooth [Taylor expansion](taylor-expansion.md); a small difference can reflect accidental cancellation rather than a rigorous upper bound.

**Table of contents**

- [Predictor-corrector error estimation](predictor-corrector-error-estimation.md)
- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Step-doubling error estimation](step-doubling-error-estimation.md)

## ↑ Ancestors (6)

1. [Error control for ODE solvers](error-control-for-ode-solvers.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Adaptive Euler step doubling for exponential decay](adaptive-euler-step-doubling-for-exponential-decay.md)
- [Adaptive step-size controller](adaptive-step-size-controller.md)
- [Error control for ODE solvers](error-control-for-ode-solvers.md)
- [Local error estimator](local-error-estimator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/6/solution.md)
