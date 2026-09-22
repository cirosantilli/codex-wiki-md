# Energy identity

↑ **Parent:** [Energy method](energy-method.md)

An energy identity is an exact balance obtained by differentiating a chosen functional along a [solution of a differential equation](solution-of-a-differential-equation.md). The functional often is a squared [L2 norm](l2-norm.md), $D$ collects dissipative terms, and $F$ collects forcing or reaction terms. Dropping nonnegative terms gives an [energy estimate](energy-estimate.md).

For $u_t=u_{xx}+g$ on $(0,1)$ with $u_x(0,t)=\alpha u(0,t)$ and $u(1,t)=0$, [integration by parts](integration-by-parts.md) proves

$$
\frac12\frac d{dt}\int_0^1u^2\,dx+\int_0^1u_x^2\,dx+\alpha u(0,t)^2=\int_0^1ug\,dx.
$$

The boundary term is $[u u_x]_0^1=-\alpha u(0,t)^2$; the minus sign at the left endpoint is essential. For $\alpha\geq0$ it contributes dissipation. If $ug\leq a(t)u^2$ and the initial data vanish, the [Gronwall inequality](gronwall-inequality.md) forces $u\equiv0$.

## ↑ Ancestors (6)

1. [Energy method](energy-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford/2009/b/6/solution.md)
- [Solution](past-exam-of-the-differential-equations-1-course-of-the-university-of-oxford/2023/3/b/i/solution.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/1/a/solution.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/1/b/solution.md)
