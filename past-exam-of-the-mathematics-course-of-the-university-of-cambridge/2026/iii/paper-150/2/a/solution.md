<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $f$ is a [multiplicative function](../../../../../../multiplicative-function.md) with $|f(n)|\leq1$, then for $\Re s>1$ its [Dirichlet series](../../../../../../dirichlet-series.md) has the [Euler product](../../../../../../euler-product.md)

$$
\sum_{n=1}^{\infty}\frac{f(n)}{n^s}
=\prod_p\left(1+\frac{f(p)}{p^s}+\frac{f(p^2)}{p^{2s}}+\cdots\right).
$$

Indeed, expanding the product over a finite set of primes and using [unique prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md) gives the sum over integers having no other prime factors. Moreover,

$$
\sum_{n\geq1}\left|\frac{f(n)}{n^s}\right|
\leq\sum_{n\geq1}n^{-\Re s}<\infty,
$$

so [absolute convergence](../../../../../../absolute-convergence.md) permits rearrangement and passage to the limit over all primes. This proves the formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
