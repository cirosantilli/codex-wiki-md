# Sharp one-panel trapezoidal error bound

↑ **Parent:** [Trapezoidal rule](trapezoidal-rule.md)

For $f\in C^2[a,b]$ with $a<b$, the [trapezoidal rule](trapezoidal-rule.md) satisfies the displayed bound, and the constant $1/12$ is best possible. The [polynomial interpolation error](polynomial-interpolation-error.md) for the endpoint [linear interpolant](linear-interpolant.md) satisfies $|f(x)-p(x)|\leq\tfrac12 M(x-a)(b-x)$, where $M=\max|f''|$. Integrating this inequality and using the [triangle inequality for an integral](integral-triangle-inequality.md) proves the bound because $\int_a^b(x-a)(b-x)\,dx=(b-a)^3/6$. Equality holds for $f(x)=(x-a)^2$: the exact [integral](integral-split.md) is $(b-a)^3/3$, its [trapezoidal rule](trapezoidal-rule.md) estimate is $(b-a)^3/2$, and $M=2$.

## ↑ Ancestors (9)

1. [Trapezoidal rule](trapezoidal-rule.md)
2. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
3. [Runge-Kutta method](runge-kutta-method-split.md)
4. [One-step method](one-step-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2015/1/b/i/solution.md)
