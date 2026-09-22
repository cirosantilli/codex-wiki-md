# Adaptive step-size controller

↑ **Parent:** [Error control for ODE solvers](error-control-for-ode-solvers-split.md)

If a scaled [local error estimator](local-error-estimator.md) behaves as $E\propto h^r$ with approximately unchanged error scale, the displayed update targets a fixed local level. A safety factor $0<\eta<1$ aims below the acceptance boundary. For an [embedded Runge-Kutta pair](embedded-runge-kutta-pair.md) with [order of a numerical method](order-of-a-numerical-method.md) $p$ for the accepted output and $p-1$ for the companion formula, the difference generally has $r=p$; for the actual unscaled [local truncation error](local-truncation-error.md) of an order-$p$ formula, $r=p+1$. The exponent belongs to the quantity being controlled. Dividing the defect by $h$ changes that exponent. This follows by solving $E(h_{\rm new})\approx E(h)(h_{\rm new}/h)^r$ for the next step.[§6.5.1, equations (6.5.1)–(6.5.4): estimator order and step prediction](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

Rejecting a trial means retrying from the same accepted time and state, with a smaller step. Advancing time or retaining the rejected output would change the [initial value problem](initial-value-problem.md) being approximated. Minimum and maximum change factors prevent extreme updates; a zero estimate requires finite capped growth. After acceptance, cap the next step at the remaining interval length. Detect a step that cannot advance time in [floating-point arithmetic](floating-point-arithmetic-split.md), and report failure rather than an endless retry. An [adaptive step-size controller](adaptive-step-size-controller.md) can use earlier estimates to smooth step sequences, but the memoryless rule here is sufficient to explain acceptance and rejection.[§6.5.1, Algorithm 6.5.1; §6.5.3, rk23 implementation and About the code: retain state on rejection, safety factor, growth cap, final-step cap, nonadvancing-time check](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

## ↑ Ancestors (6)

1. [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Adaptive Euler-Heun integration of exponential growth](adaptive-euler-heun-integration-of-exponential-growth.md)
- [Adaptive Euler step doubling for exponential decay](adaptive-euler-step-doubling-for-exponential-decay.md)
- [Adaptive step-size controller](adaptive-step-size-controller.md)
- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/6/solution.md)
