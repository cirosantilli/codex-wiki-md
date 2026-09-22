# Adaptive step-size controller

↑ **Parent:** [Error control for ODE solvers](error-control-for-ode-solvers.md)

If a scaled [local error estimator](local-error-estimator.md) behaves as $E\propto h^r$, the displayed update targets a fixed local level. A safety factor $\eta<1$, minimum/maximum change factors and rejected-step rollback improve robustness. A zero estimate needs finite capped growth. For an embedded $p/(p-1)$ pair, usually $r=p$; for a true order-$p$ exact-start defect, $r=p+1$. Controllers using previous estimates can smooth step sequences. The [GSL ODE documentation](https://www.gnu.org/software/gsl/doc/html/ode-initval.html) illustrates component error scaling, safety factors and growth limits in an actual solver; controller-specific exponents depend on how the solver defines its error estimate.

## ↑ Ancestors (6)

1. [Error control for ODE solvers](error-control-for-ode-solvers.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Error control for ODE solvers](error-control-for-ode-solvers.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/6/solution.md)
