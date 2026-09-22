# Milstein method

↑ **Parent:** [Euler-Maruyama method](euler-maruyama-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Milstein_method)

For a scalar [stochastic differential equation](stochastic-differential-equation.md), the Milstein method adds the quadratic-variation correction

$$
X_{n+1}=X_n+a(X_n)\Delta t+\sigma(X_n)\Delta W_n
+\frac12\sigma(X_n)\sigma'(X_n)
\left((\Delta W_n)^2-\Delta t\right).
$$

Under standard smoothness assumptions it has [strong order of convergence](strong-convergence-of-a-stochastic-numerical-method.md) one and [weak order of convergence](weak-convergence-of-a-stochastic-numerical-method.md) one.

## ↑ Ancestors (9)

1. [Euler-Maruyama method](euler-maruyama-method.md)
2. [Stochastic differential equation](stochastic-differential-equation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-356/2/b/solution.md)
