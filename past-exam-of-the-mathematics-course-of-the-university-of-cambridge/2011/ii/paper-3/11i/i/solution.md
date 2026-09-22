<h1 id="11i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $\sigma=\operatorname{Re}s>1$, the [Dirichlet series](../../../../../../dirichlet-series.md) $\zeta(s)=\sum_{n\geq1}n^{-s}$ is absolutely convergent. A finite product over primes $p\leq P$ can be expanded into absolutely convergent [geometric series](../../../../../../geometric-series.md). By [unique prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md),

$$
\prod_{p\leq P}(1-p^{-s})^{-1}=\sum_{\substack{n\geq1\\\text{all prime factors of }n\leq P}}n^{-s}.
$$

The omitted integers are all greater than $P$, so the difference from $\zeta(s)$ has modulus at most $\sum_{n>P}n^{-\sigma}\to0$. Thus

$$
\boxed{\zeta(s)=\prod_p(1-p^{-s})^{-1}\qquad(\operatorname{Re}s>1).}
$$

This defines the infinite [Euler product](../../../../../../euler-product.md) as the limit of finite products. Its absolute convergence also follows from $\sum_p p^{-\sigma}<\infty$, with $\log(1-p^{-s})^{-1}=p^{-s}+O(p^{-2\sigma})$ for sufficiently large $p$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11I](../../11i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
