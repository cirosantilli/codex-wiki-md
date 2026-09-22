<h1 id="9g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $x=0$, the generated subspace is zero and invariant. Otherwise, let $r$ be the first index for which $x,Tx,\ldots,T^rx$ are [linearly dependent](../../../../../../linear-dependence.md). Such an index exists with $1\leq r\leq n$, since there are $n+1$ vectors. The preceding vectors are independent, so the coefficient of $T^rx$ in this first relation cannot vanish. Hence

$$
T^rx\in\operatorname{span}\{x,Tx,\ldots,T^{r-1}x\}.
$$

The [linear operator](../../../../../../linear-operator.md) $T$ sends each of the first $r-1$ generators to the next and sends the last into their [span](../../../../../../linear-span.md). This proves that their span is an [invariant subspace](../../../../../../invariant-subspace.md). Every later iterate lies in the same subspace by induction, so it equals the span of the first $n$ iterates. Therefore **the indicated subspace is $T$-invariant**. This proof of a [cyclic subspace](../../../../../../cyclic-subspace.md) uses only finite [dimension](../../../../../../dimension-vector-space.md) and [linear dependence](../../../../../../linear-dependence.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [9G](../../9g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
