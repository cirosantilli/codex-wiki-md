<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $v=t(1-t)$ and $M=\max_i\beta_i$. If $v=0$ the assertion is immediate. Otherwise, suppose

$$
M<\frac{v\log n}{2n}.
$$

Since $v\leq1/4$, this makes $M\leq\log n/(8n)$, so $M$ is sufficiently small to apply the [maximum-influence logarithmic lower bound](../../../../../../maximum-influence-logarithmic-lower-bound.md) once $n$ is large. That bound gives

$$
nM\geq\sum_i\beta_i\geq\frac23v\log(1/M)
\geq\frac23v\left(\log n-\log\log n+\log8\right).
$$

For all sufficiently large $n$, the last quantity exceeds $v\log n/2$, contradicting $nM<v\log n/2$. The choice of sufficiently large $n$ is independent of $t$. Therefore

$$
\boxed{\max_i\beta_i\geq\frac12t(1-t)\frac{\log n}{n}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
