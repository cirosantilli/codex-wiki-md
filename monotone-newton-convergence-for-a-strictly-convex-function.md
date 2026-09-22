# Monotone Newton convergence for a strictly convex function

↑ **Parent:** [Newton root-finding iteration](newton-root-finding-iteration.md)

Let $f\in C^2([a,b])$ have $f',f''>0$ and $f(a)<0<f(b)$. Its unique root $r$ lies in $(a,b)$. Starting [Newton root-finding iteration](newton-root-finding-iteration.md) at $b$, strict convexity puts the tangent root strictly between $r$ and the current iterate, so the iterates decrease to $r$. Taylor expansion about the current iterate gives $e_{n+1}=f''(\xi_n)e_n^2/[2f'(x_n)]$, where $e_n=x_n-r$ and $\xi_n\in(r,x_n)$. Continuity proves the displayed positive asymptotic constant and [quadratic convergence](quadratic-convergence.md).

## ↑ Ancestors (6)

1. [Newton root-finding iteration](newton-root-finding-iteration.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/11d/ii/solution.md)
