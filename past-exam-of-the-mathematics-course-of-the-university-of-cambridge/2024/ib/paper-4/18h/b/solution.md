<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $x_k\geq1$, then positivity and the [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) give

$$
x_{k+1}=\frac12\left(x_k+\frac a{x_k}\right)
\geq\sqrt a\geq1.
$$

Thus all iterates remain in $[1,\infty)$.

Consider the strictly convex [function](../../../../../../function-split.md)

$$
f(x)=\frac{x^3}{3}-ax
$$

on $[1,\infty)$. Since $f'(x)=x^2-a$ and $f''(x)=2x$, its Newton minimization step is

$$
x-\frac{f'(x)}{f''(x)}
=\frac12\left(x+\frac ax\right).
$$

Its unique minimizer is $x^*=\sqrt a$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
