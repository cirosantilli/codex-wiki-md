<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The two-variable [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) follows from a square:

$$
0\leq(\sqrt a-\sqrt b)^2=a+b-2\sqrt{ab}.
$$

Hence **$2\sqrt{ab}\leq a+b$**, with equality exactly when $a=b$.

For the [series](../../../../../series-mathematics.md), apply that same inequality with $a=a_n$ and $b=n^{-2}$ to obtain

$$
0\leq\frac{\sqrt{a_n}}n\leq\frac12\left(a_n+\frac1{n^2}\right).
$$

The comparison [series](../../../../../series-mathematics.md) converges: its first summand has finite sum by hypothesis, and the inverse-square [series](../../../../../series-mathematics.md) converges, for example by the telescoping estimate $n^{-2}\leq1/[n(n-1)]=1/(n-1)-1/n$ for $n\geq2$. Thus the [comparison test for series](../../../../../comparison-test-for-series.md) proves

$$
\boxed{\sum_{n=1}^\infty\frac{\sqrt{a_n}}n<\infty.}
$$

Equivalently, its positive partial sums are increasing and bounded above by $\tfrac12\sum a_n+\tfrac12\sum n^{-2}$, so the [bounded monotone sequence theorem](../../../../../bounded-monotone-sequence-theorem.md) proves convergence directly. This is the case $p=1$ of [weighted square roots of a summable sequence](../../../../../weighted-square-roots-of-a-summable-sequence.md).

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
