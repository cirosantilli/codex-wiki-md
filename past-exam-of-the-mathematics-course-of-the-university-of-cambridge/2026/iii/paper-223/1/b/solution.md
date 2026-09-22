<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let replacement tolerance mean the greatest number of observations that can be replaced while the estimator remains bounded. For $n=2m$, a sample with $m$ zeros and $m$ copies of $a$ is within $m$ replacements of both the all-zero sample and its translate by $a$. If an equivariant estimator tolerated $m$ replacements, it would remain within bounded distance of both $T(0^n)$ and $T(0^n)+a$, which is impossible as $a\to\infty$. Thus at most $m-1$ replacements are tolerable.

For $n=2m+1$, a sample with $m$ zeros and $m+1$ copies of $a$ is obtained from the all-zero sample by $m+1$ replacements and from the all-$a$ sample by $m$ replacements. Translation equivariance again forces breakdown by $m+1$ replacements. In both cases the finite-sample [replacement breakdown point](../../../../../../replacement-breakdown-point.md) is at most

$$
\boxed{\frac1n\left\lfloor\frac{n-1}{2}\right\rfloor.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
