# Gauss collocation coefficient construction

↑ **Parent:** [Gauss-Legendre method](gauss-legendre-method.md)

Choose $c_1,\ldots,c_s$ as the [polynomial roots](root-of-a-polynomial.md) of $P_s(2c-1)$ in $(0,1)$, and form the [Lagrange interpolation polynomials](lagrange-polynomial.md) $\ell_j(t)=\prod_{m\ne j}(t-c_m)/(c_j-c_m)$. The [Gauss collocation method](gauss-legendre-method.md) has $a_{ij}=\int_0^{c_i}\ell_j(t)dt$ and $b_j=\int_0^1\ell_j(t)dt$. This gives explicit coefficient formulas after finding [polynomial roots](root-of-a-polynomial.md): if $\ell_j(t)=\sum_rd_{jr}t^r$, these [integrals](integral.md) are $\sum_rd_{jr}c_i^{r+1}/(r+1)$ and $\sum_rd_{jr}/(r+1)$. [Gaussian quadrature](gaussian-quadrature.md) gives order $2s$.

## ↑ Ancestors (9)

1. [Gauss-Legendre method](gauss-legendre-method.md)
2. [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)
3. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
4. [Runge-Kutta method](runge-kutta-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/1/b/solution.md)
