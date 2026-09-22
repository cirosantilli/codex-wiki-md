# Concave Newton iteration from below

↑ **Parent:** [Newton root-finding iteration](newton-root-finding-iteration.md)

Suppose $f\in C^2([a,r])$, $f(r)=0$, $f'\ge m>0$ and $-K\le f''<0$. Starting at $x_0\in[a,r)$, the [Newton root-finding iteration](newton-root-finding-iteration.md) remains below $r$ and increases strictly to it. To prove this, assume $x_n<r$. Strict increase of $f$ gives $f(x_n)<0$, so the Newton step is positive. [Taylor's theorem](taylor-s-theorem.md) between $x_n$ and $r$ gives, with $e_n=x_n-r$,

$$
e_{n+1}=\frac{f''(\xi_n)}{2f'(x_n)}e_n^2.
$$

Its coefficient is negative and at least $-K/(2m)$, proving both the stated error bound and $x_n<x_{n+1}<r$. [Mathematical induction](mathematical-induction.md) establishes the invariant. The increasing bounded iterates have a [limit](limit-of-a-function.md) $L\le r$; continuity in $x_{n+1}-x_n=-f(x_n)/f'(x_n)$ forces $f(L)=0$, hence $L=r$. The error bound supplies local [quadratic convergence](quadratic-convergence.md).

## ↑ Ancestors (6)

1. [Newton root-finding iteration](newton-root-finding-iteration.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/6/e/solution.md)
