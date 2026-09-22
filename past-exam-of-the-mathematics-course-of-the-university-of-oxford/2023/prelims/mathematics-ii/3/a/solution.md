<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [power series](../../../../../../power-series.md) $\sum a_nz^n$, its [radius of convergence](../../../../../../radius-of-convergence.md) $R\in[0,\infty]$ separates [absolute convergence](../../../../../../absolute-convergence.md) for $|z|<R$ from divergence for $|z|>R$. One may define $R=\sup\{r\geq0:\sum|a_n|r^n<\infty\}$, allowing $R=\infty$.

To justify convergence inside the radius, choose $|z|<r<R$ with $\sum|a_n|r^n<\infty$. In particular $|a_n|r^n\leq M$ for some $M$, so

$$
|a_nz^n|\leq M(|z|/r)^n.
$$

The [comparison test](../../../../../../direct-comparison-test.md) with a [geometric series](../../../../../../geometric-series.md) proves [absolute convergence](../../../../../../absolute-convergence.md). Conversely, convergence at a point of modulus $\rho$ makes $a_nz^n$ bounded there and gives [absolute convergence](../../../../../../absolute-convergence.md) at all smaller moduli by the same estimate. Consequently a convergent point of modulus greater than $R$ would contradict the definition of $R$.

For $0<R<\infty$, the real [domain of convergence](../../../../../../domain-of-convergence.md) is one of $(-R,R)$, $[-R,R)$, $(-R,R]$, or $[-R,R]$. At $R=1$ these are realized respectively by

$$
\sum z^n,\qquad \sum_{n=1}^\infty\frac{z^n}{n},\qquad \sum_{n=1}^\infty\frac{(-1)^nz^n}{n},\qquad \sum_{n=1}^\infty\frac{z^n}{n^2}.
$$

The endpoint assertions follow from the [harmonic series](../../../../../../harmonic-series.md), [alternating series test](../../../../../../alternating-series-test.md), and [p-series](../../../../../../p-series.md). Replacing $z$ by $z/R$ realizes every finite positive radius. The degenerate domain $\{0\}$ occurs for $\sum n!z^n$, while the entire [real line](../../../../../../real-line.md) occurs for $\sum z^n/n!$. Their radii are zero and infinity by the [ratio test](../../../../../../ratio-test.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
