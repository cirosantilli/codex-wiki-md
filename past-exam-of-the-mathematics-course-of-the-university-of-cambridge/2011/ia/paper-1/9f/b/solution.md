<h1 id="9f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [function](../../../../../../function-split.md) $1/x$ is decreasing and positive. Therefore on $[k,k+1]$ it is at most $1/k$, and the [Riemann integral](../../../../../../riemann-integral.md) gives

$$
\int_k^{k+1}\frac{dx}{x}\le\frac1k.
$$

Summing from $k=1$ to $n-1$ yields

$$
\boxed{\log n=\int_1^n\frac{dx}{x}\le\sum_{k=1}^{n-1}\frac1k.}
$$

For $n=1$ both sides are zero; for $n>1$ the inequality is actually strict. The same [integral test for convergence](../../../../../../integral-test-for-convergence.md) gives $\sum_{k=N}^{n-1}1/k\ge\log(n/N)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
