# Contractivity of split Crank-Nicolson diffusion

↑ **Parent:** [Crank-Nicolson method](crank-nicolson-method.md)

For symmetric negative semidefinite matrices $A,B$, each factor $C_A(h)=(I-hA/2)^{-1}(I+hA/2)$ has norm at most one, since its eigenvalues are $(1+h\lambda/2)/(1-h\lambda/2)$ with $\lambda\le0$. The same holds for $B$, so their ordered product is a contraction for every $h\ge0$, whether or not $A,B$ commute. This proves unconditional discrete [L2 norm](l2-norm.md) stability of the split [Crank-Nicolson method](crank-nicolson-method.md) for directional diffusion. Its splitting error remains first order in general, because the product's quadratic defect is $h^2[A,B]/2$.

## ↑ Ancestors (8)

1. [Crank-Nicolson method](crank-nicolson-method.md)
2. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
3. [Runge-Kutta method](runge-kutta-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/5/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/7/solution.md)
