# Absolute and relative error tolerances

↑ **Parent:** [Error control for ODE solvers](error-control-for-ode-solvers-split.md)

Absolute tolerances provide a nonzero error scale near zero, while relative tolerances follow component magnitude. A max-norm test $\max_i|\widehat e_i|/s_i\leq1$ controls every scaled estimated component locally. A root-mean-square test has a different componentwise implication. Neither test automatically certifies the complete trajectory's [global error](global-discretization-error.md).

Write $Y_i$ for the candidate accepted component and require $s_i>0$. The [absolute and relative error tolerances](absolute-and-relative-error-tolerances.md) scale in the title produces the dimensionless [maximum norm](supremum-norm.md) test

$$
E=\max_{1\leq i\leq m}\frac{|\widehat e_i|}{{\rm atol}_i+{\rm rtol}_i\max(|y_i|,|Y_i|)}\leq1.
$$

Absolute tolerances have the same units as the corresponding solution components; relative tolerances are dimensionless. Choose separate absolute scales for components measured in different units or with different significant magnitudes. Near zero, a purely relative test can demand a zero allowable error; a positive absolute scale avoids that difficulty. The crossover is $\max(|y_i|,|Y_i|)\approx{\rm atol}_i/{\rm rtol}_i$ when ${\rm rtol}_i>0$. Official solver documentation specifies the analogous blend ${\rm atol}+{\rm rtol}|y|$ and allows component-specific absolute tolerances; the old/new maximum above is the convention used in this example.[solve\_ivp, rtol and atol parameters: local error estimates, additive scaling and component-specific atol](scipy-1-16-2-documentation/scipy-integrate-solve-ivp.md)

A [root mean square](root-mean-square.md) version replaces the [maximum norm](supremum-norm.md) by $E_{\rm rms}=\sqrt{m^{-1}\sum_i(|\widehat e_i|/s_i)^2}$. It permits one scaled component as large as $\sqrt m$ when all others vanish, so passing that test does not mean every component is at most one. State the aggregation rule along with the [absolute and relative error tolerances](absolute-and-relative-error-tolerances.md). Neither rule is a bound on actual [global error](global-discretization-error.md).

## ↑ Ancestors (6)

1. [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Absolute and relative error tolerances](absolute-and-relative-error-tolerances.md)
- [Adaptive Euler-Heun integration of exponential growth](adaptive-euler-heun-integration-of-exponential-growth.md)
- [Adaptive Euler step doubling for exponential decay](adaptive-euler-step-doubling-for-exponential-decay.md)
- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Error control for ODE solvers](error-control-for-ode-solvers-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/6/solution.md)
