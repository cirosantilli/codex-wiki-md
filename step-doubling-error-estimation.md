# Step-doubling error estimation

↑ **Parent:** [Local error estimator](local-error-estimator.md)

For an order-$p$ one-step method with leading numerical error $Ch^{p+1}$, two half steps have leading error $Ch^{p+1}/2^p$. The displayed difference estimates exact minus the finer approximation. Adding it implements [Richardson extrapolation](richardson-extrapolation.md). It requires a common starting value, the smooth local expansion, and accuracy of all algebraic solves; it can fail across a nonsmooth event.

## ↑ Ancestors (7)

1. [Local error estimator](local-error-estimator.md)
2. [Error control for ODE solvers](error-control-for-ode-solvers.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Local error estimator](local-error-estimator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/6/solution.md)
- [Richardson extrapolation](richardson-extrapolation.md)
