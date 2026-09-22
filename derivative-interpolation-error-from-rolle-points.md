# Derivative interpolation error from Rolle points

↑ **Parent:** [Polynomial interpolation error](polynomial-interpolation-error.md)

Let $f\in C^{n+1}[a,b]$, $n\geq1$, and let $p_n$ be its [Lagrange interpolation polynomial](lagrange-polynomial.md) at ordered distinct [interpolation nodes](interpolation-node.md) $x_0<\cdots<x_n$. Since $f-p_n$ vanishes at every [interpolation node](interpolation-node.md), [Rolle's theorem](rolle-theorem.md) supplies distinct $\eta_i\in(x_{i-1},x_i)$ where $f'(\eta_i)=p_n'(\eta_i)$. The [polynomial](polynomial-split.md) $p_n'$ has [polynomial degree](degree-of-a-polynomial.md) at most $n-1$, so it is the [interpolation polynomial](interpolation-polynomial.md) for $f'$ at these $n$ new [interpolation nodes](interpolation-node.md). Its [polynomial interpolation error](polynomial-interpolation-error.md) is the displayed formula, with $\xi\in(a,b)$ depending on $x$.

Consequently $|f'(x)-p_n'(x)|\leq M\prod_i|x-\eta_i|/n!\leq M(b-a)^n/n!$, where $M=\max|f^{(n+1)}|$. The existence of the [interpolation nodes](interpolation-node.md) is enough for this bound; their explicit locations generally depend on $f$. This proof avoids differentiating an unspecified intermediate point in the original [polynomial interpolation error](polynomial-interpolation-error.md) formula.

## ↑ Ancestors (5)

1. [Polynomial interpolation error](polynomial-interpolation-error.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2015/2/c/i/solution.md)
