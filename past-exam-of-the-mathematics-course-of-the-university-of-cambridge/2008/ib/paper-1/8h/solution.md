<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

The [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) for an equality constraint states that if a feasible $x_*$ and a multiplier $\lambda_*$ exist such that $x_*$ globally maximizes $L(x,\lambda_*)=f(x)-\lambda_*\cdot(g(x)-b)$ over the underlying domain, then $x_*$ globally maximizes $f$ over $g(x)=b$. Indeed $L=f$ at every feasible point, so global maximality of $L$ directly compares the feasible objective values. The underlying domain can already impose $x_i\geq0$.

For $0<p<1$, choose $\lambda=p d^{1-p}$. Each function $t^p-\lambda t$ on $t\geq0$ is a [strictly concave function](../../../../../strictly-concave-function.md) and attains its unique maximum at $t=1/d$, since $pt^{p-1}=\lambda$ there. The sum [Lagrangian](../../../../../lagrangian.md) is therefore globally maximized when every $x_i=1/d$, and this point is feasible. For $p=1$ the objective is identically one on the feasible set. For $p>1$, each feasible $x_i$ lies in $[0,1]$, so $x_i^p\leq x_i$, with equality only at $0$ or $1$; equality in the total is attained exactly at a [simplex](../../../../../simplex.md) vertex. Consequently

$$
\boxed{\max\sum_{i=1}^d x_i^p=\begin{cases}d^{1-p},&0<p<1,\\1,&p\geq1.\end{cases}}
$$

For $0<p<1$ the unique maximizer is $(1/d,\ldots,1/d)$; for $p=1$ every feasible point is a maximizer; for $p>1$ the maximizers are exactly the $d$ vertices with one coordinate one and all others zero. When $d=1$ these descriptions coincide.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
