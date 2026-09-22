# Exact finite difference solution for constant second derivative

↑ **Parent:** [Central finite difference](central-finite-difference.md)

On a uniform mesh $x_n=a+nh$, the centered second [finite difference](finite-difference-split.md) is exact for every quadratic [polynomial](polynomial-split.md). In particular, for $y''=c$ with endpoint [boundary conditions](boundary-condition.md), the unique discrete solution equals the exact quadratic solution at every mesh point. Subtracting consecutive first differences reduces the equation to $d_{n+1}-d_n=ch^2$, so $y_n=\tfrac12ch^2n(n-1)+d_1n+y_0$. The second endpoint determines $d_1$. Uniqueness follows because any difference of two discrete solutions has zero second [finite difference](finite-difference-split.md), hence is linear in the mesh index and vanishes at both endpoints. Exact nodal values in this example do not imply that a general [finite difference method](finite-difference-method.md) is exact for other [ordinary differential equations](ordinary-differential-equation.md).

## ↑ Ancestors (8)

1. [Central finite difference](central-finite-difference.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/4/c/ii/solution.md)
