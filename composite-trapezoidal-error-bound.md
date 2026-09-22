# Composite trapezoidal error bound

↑ **Parent:** [Composite trapezoidal rule](composite-trapezoidal-rule.md)

If $f$ is twice continuously differentiable on $[a,b]$, take a uniform bound $|f''|\leq M$. On one panel $[u,v]$, two [integrations by parts](integration-by-parts.md) give the signed [quadrature error](quadrature-error.md)

$$
\frac{v-u}{2}(f(u)+f(v))-\int_u^v f(t)\,dt=\frac12\int_u^v(t-u)(v-t)f''(t)\,dt.
$$

The nonnegative kernel has integral $(v-u)^3/6$, so the absolute error is at most $M(v-u)^3/12$. Summing $n$ equal panels proves the displayed bound. The maximum exists on the closed interval; a supremum or any known uniform bound also suffices. The estimate certifies a sufficient panel count, which need not be the least count achieving a particular actual error.

## ↑ Ancestors (10)

1. [Composite trapezoidal rule](composite-trapezoidal-rule.md)
2. [Trapezoidal rule](trapezoidal-rule.md)
3. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
4. [Runge-Kutta method](runge-kutta-method-split.md)
5. [One-step method](one-step-method.md)
6. [Numerical analysis](numerical-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/4/a/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/discrete-mathematics-continuous-mathematics-and-probability/6/f/solution.md)
