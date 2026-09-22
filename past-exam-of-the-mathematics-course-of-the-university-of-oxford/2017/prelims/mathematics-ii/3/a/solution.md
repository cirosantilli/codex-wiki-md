<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A real or complex [sequence](../../../../../../sequence.md) $(a_n)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md) if

$$
\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall m,n\geq N:\quad |a_m-a_n|<\varepsilon.
$$

For $z_n=x_n+iy_n$, the [complex modulus](../../../../../../complex-modulus.md) gives

$$
|x_m-x_n|\leq|z_m-z_n|,\qquad |y_m-y_n|\leq|z_m-z_n|.
$$

Thus the same $N$ works for both coordinate [Cauchy sequences](../../../../../../cauchy-sequence.md). Conversely, if both real coordinate [Cauchy sequences](../../../../../../cauchy-sequence.md) converge to $x$ and $y$, then $|z_n-(x+iy)|\leq|x_n-x|+|y_n-y|\to0$. This proves the needed completeness for [complex numbers](../../../../../../complex-number.md) from the assumed [completeness of the real numbers](../../../../../../completeness-of-the-real-numbers.md).

Now suppose $\sum_{n\geq0}|z_n|$ converges. Its real [partial sums](../../../../../../partial-sum.md) form a [Cauchy sequence](../../../../../../cauchy-sequence.md). Given $\varepsilon>0$, sufficiently late tails therefore satisfy $\sum_{k=n+1}^m|z_k|<\varepsilon$. For $s_m=\sum_{k=0}^mz_k$, the [triangle inequality](../../../../../../triangle-inequality.md) yields

$$
|s_m-s_n|\leq\sum_{k=n+1}^m|z_k|<\varepsilon\qquad(m>n\geq N).
$$

The complex [partial sums](../../../../../../partial-sum.md) are a [Cauchy sequence](../../../../../../cauchy-sequence.md), hence converge by the coordinate argument. Therefore **[absolute convergence](../../../../../../absolute-convergence.md) implies convergence** for a complex [series](../../../../../../series-mathematics.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
