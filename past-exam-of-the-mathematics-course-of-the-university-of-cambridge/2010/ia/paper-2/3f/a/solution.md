<h1 id="3f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $m\geq2$, $f''(x)=m(m-1)x^{m-2}\geq0$ on $[0,\infty)$, so $f$ is a [convex function](../../../../../../convex-function.md); for $m=1$ it is linear and also convex. The equally weighted [random variable](../../../../../../random-variable-split.md) has [expected value](../../../../../../expected-value.md) $EX=N^{-1}\sum_i x_i=1/N$. Applying [Jensen's inequality](../../../../../../jensen-s-inequality.md) gives

$$
\frac1N\sum_{i=1}^N f(x_i)=Ef(X)\geq f(EX)=f(1/N).
$$

Multiplying by $N$ proves

$$
\boxed{\sum_{i=1}^N x_i^m\geq N^{1-m}.}
$$

For $m>1$ equality requires all $x_i=1/N$, by strict convexity; for $m=1$ equality holds for every admissible vector.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3F](../../3f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
