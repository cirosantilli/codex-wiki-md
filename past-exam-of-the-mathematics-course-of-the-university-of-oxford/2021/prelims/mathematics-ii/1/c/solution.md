<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) states that every [bounded sequence](../../../../../../bounded-sequence.md) of [real numbers](../../../../../../real-number.md) has a [convergent subsequence](../../../../../../convergent-subsequence.md). It is enough to select infinitely many terms of the [tangent](../../../../../../tangent.md) [sequence](../../../../../../sequence.md) that stay uniformly bounded.

For each positive [integer](../../../../../../integer-split.md) $k$, choose $n_k=\lfloor k\pi+1/2\rfloor$, using the [floor function](../../../../../../floor-function.md). Then $|n_k-k\pi|\leq1/2$. Moreover $n_{k+1}-n_k\geq\pi-1>0$, so these are strictly increasing indices. By the period and [monotonicity](../../../../../../monotonic-function.md) of the [tangent](../../../../../../tangent.md) on $(-\pi/2,\pi/2)$,

$$
|\tan n_k|=|\tan(n_k-k\pi)|\leq\tan(1/2).
$$

Thus $(\tan n_k)$ is a [bounded subsequence](../../../../../../bounded-subsequence.md). Applying the [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) to it gives a [convergent subsequence](../../../../../../convergent-subsequence.md), which is also a [subsequence](../../../../../../subsequence.md) of the original [sequence](../../../../../../sequence.md). **Such a [convergent subsequence](../../../../../../convergent-subsequence.md) therefore exists.**

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
