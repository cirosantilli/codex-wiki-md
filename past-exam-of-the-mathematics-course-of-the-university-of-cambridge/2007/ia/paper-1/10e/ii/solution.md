<h1 id="10e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $q=\lambda a+(1-\lambda)b$. Since $0<\lambda<1$ and $a<b$, $a<q<b$. Apply the [mean value theorem](../../../../../../mean-value-theorem.md) separately to $[a,q]$ and $[q,b]$. There exist $x\in(a,q)$ and $y\in(q,b)$ such that

$$
\boxed{f(q)=f(a)+(1-\lambda)(b-a)f'(x)
=f(b)-\lambda(b-a)f'(y).}
$$

These are the requested points, and $x<y$. Part (i) makes $f'(x)\leq f'(y)$, so the corresponding secant slopes satisfy

$$
\frac{f(q)-f(a)}{(1-\lambda)(b-a)}
\leq\frac{f(b)-f(q)}{\lambda(b-a)}.
$$

Multiply by the positive denominators and collect $f(q)$ to obtain

$$
\boxed{f(\lambda a+(1-\lambda)b)\leq\lambda f(a)+(1-\lambda)f(b).}
$$

This is precisely the defining chord inequality for a [convex function](../../../../../../convex-function.md). The proof uses only existence and nonnegativity of $f''$, with no additional regularity hypothesis on that derivative.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10E](../../10e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
