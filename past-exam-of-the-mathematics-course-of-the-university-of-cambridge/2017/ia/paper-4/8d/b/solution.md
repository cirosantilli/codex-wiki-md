<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) gives $a_k+1/a_k\ge2$, so $u_n\ge2n\to+\infty$. Hence **$(u_n)$ has no finite limit**.

For the example, take $\boxed{a_k=1+2^{-k}}$. Every term is positive and different from $1$, and

$$
0<a_k-\frac1{a_k}=\frac{2^{-k}(2+2^{-k})}{1+2^{-k}}<2^{1-k}.
$$

The bounding [geometric series](../../../../../../geometric-series.md) converges, so the [comparison test for series](../../../../../../comparison-test-for-series.md) proves that the [partial sums](../../../../../../partial-sum.md) $v_n$ converge.

In general, if $v_n$ converges, the necessary condition for a [convergent series](../../../../../../convergent-series.md) gives $d_k=a_k-1/a_k=v_k-v_{k-1}\to0$. Since $a_k>0$,

$$
a_k+\frac1{a_k}=\sqrt{\left(a_k-\frac1{a_k}\right)^2+4}=\sqrt{d_k^2+4}\longrightarrow2.
$$

Apply the [Cesaro theorem for convergent sequences](../../../../../../cesaro-theorem-for-convergent-sequences.md) to these summands:

$$
\boxed{\frac{u_n}{n}\longrightarrow2.}
$$

Equivalently, $a_k=(d_k+\sqrt{d_k^2+4})/2\to1$. The [series](../../../../../../series-mathematics.md) of the differences may converge while the [series](../../../../../../series-mathematics.md) of the positive sums still diverges linearly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
