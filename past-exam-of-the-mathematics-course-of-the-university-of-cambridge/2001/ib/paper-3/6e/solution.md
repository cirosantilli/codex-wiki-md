<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

Write $\omega(t)=\prod_{i=0}^n(t-x_i)$. If $x$ is an [interpolation node](../../../../../interpolation-node.md), the [polynomial interpolation error](../../../../../polynomial-interpolation-error.md) is zero. Otherwise set

$$
K=\frac{f(x)-p(x)}{\omega(x)},\qquad F(t)=f(t)-p(t)-K\omega(t).
$$

The function $F$ has $n+2$ distinct [zeros](../../../../../zero-of-a-function.md): the $n+1$ interpolation nodes and $x$. Repeated [Rolle's theorem](../../../../../rolle-theorem.md) therefore gives a point $\xi$ strictly between the smallest and largest of these points with $F^{(n+1)}(\xi)=0$. Since $p^{(n+1)}=0$ and $\omega^{(n+1)}=(n+1)!$, this yields the [polynomial interpolation error](../../../../../polynomial-interpolation-error.md)

$$
\boxed{f(x)-p(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}\prod_{i=0}^n(x-x_i).}
$$

All differentiations are justified by $f\in C^{n+1}[a,b]$. At an interpolation node the same displayed equality holds with any $\xi\in[a,b]$, because the product is zero.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
