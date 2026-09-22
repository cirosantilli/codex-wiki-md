<h1 id="14b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $n\geq1$, let $p_L,p_R$ be the [interpolation polynomials](../../../../../../interpolation-polynomial.md) of degree at most $n-1$ on nodes $x_0,\ldots,x_{n-1}$ and $x_1,\ldots,x_n$, respectively. The polynomial

$$
p(x)=\frac{(x-x_0)p_R(x)-(x-x_n)p_L(x)}{x_n-x_0}
$$

has degree at most $n$. At $x_0$ it equals $p_L(x_0)$; at $x_n$ it equals $p_R(x_n)$. At each common node both interpolants equal $f$, and the displayed weights sum to one, so $p$ also equals $f$ there. Thus it is the full interpolant by uniqueness.

Its coefficient of $x^n$ is the difference of the leading coefficients of $p_R,p_L$ divided by $x_n-x_0$. By the definition of a [divided difference](../../../../../../divided-difference.md),

$$
\boxed{f[x_0,\ldots,x_n]=\frac{f[x_1,\ldots,x_n]-f[x_0,\ldots,x_{n-1}]}{x_n-x_0}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14B](../../14b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
