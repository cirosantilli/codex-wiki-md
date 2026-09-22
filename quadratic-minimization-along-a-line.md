# Quadratic minimization along a line

↑ **Parent:** [Quadratic function](quadratic-function.md)

For a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $A$ and a nonzero [vector](vector.md) $p$, minimizing $f(x+\alpha p)$ over $\alpha\in\mathbb R$, where $f(x)=x^TAx/2-b^Tx$, gives the displayed optimizer. Put $r=b-Ax$. Expansion gives $f(x+\alpha p)=f(x)-\alpha p^Tr+\alpha^2p^TAp/2$, a strictly convex [quadratic function](quadratic-function.md) of $\alpha$. At its minimum,

$$
f(x+\alpha_*p)-f(x)=-\frac{(p^Tr)^2}{2p^TAp}.
$$

Strict decrease is therefore equivalent to $p^Tr\ne0$. This is minimization over a full line, so the optimizer can be negative. For an [exact line search](exact-line-search.md) restricted to a nonnegative [step size](step-size.md), the optimizer is instead $\max(0,\alpha_*)$.

## ↑ Ancestors (6)

1. [Quadratic function](quadratic-function.md)
2. [Polynomial](polynomial-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Finite termination of conjugate directions](finite-termination-of-conjugate-directions.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/3/a/solution.md)
