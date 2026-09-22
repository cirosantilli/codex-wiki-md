# Collocation endpoint superconvergence by quadrature orthogonality

↑ **Parent:** [Collocation order theorem](collocation-order-theorem.md)

For $s$ collocation nodes, the residual of the collocation polynomial vanishes at each node and contains the factor $\omega(\tau)=\prod_i(\tau-c_i)$. Quadrature exactness through degree $q-1$ implies $\int_0^1\omega(\tau)p(\tau)d\tau=0$ for every polynomial of degree at most $q-s-1$. Expand the smooth vector-field interpolation error and the derivative of the exact flow in powers of the step. Every endpoint-error term of degree below $q$ has this vanishing weighted moment, so the endpoint local error is $O(h^{q+1})$, although the interior stage accuracy is generally only $s$. A step Lipschitz estimate and [discrete Gronwall inequality](discrete-gronwall-inequality.md) then give global order $q$. Gaussian nodes attain $q=2s$, while the first nonexact quadrature moment bounds the order from above.

## ↑ Ancestors (9)

1. [Collocation order theorem](collocation-order-theorem.md)
2. [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)
3. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
4. [Runge-Kutta method](runge-kutta-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/6/solution.md)
