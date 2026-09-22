# Variable-step global ODE error bound

↑ **Parent:** [Global discretization error](global-discretization-error.md)

If a one-step map is Lipschitz with factor at most $1+Lh_n$ and its exact-start defect is at most $Ch_n^{p+1}$, iteration of the error recurrence gives the displayed global bound on a time interval of length $T$. Since $\sum h_n\leq T$, the defect sum is at most $T(\max h_n)^p$. Local tolerance control alone is not a global accuracy certificate: propagation, the number of steps, stiffness, roundoff and nonlinear-solve errors also enter. The [discrete Gronwall inequality](discrete-gronwall-inequality.md) organizes this distinction.

## ↑ Ancestors (6)

1. [Global discretization error](global-discretization-error.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/7/solution.md)
