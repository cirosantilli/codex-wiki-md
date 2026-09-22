<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $a=P(A_1)=P(A_2)$. The complements are [decreasing events](../../../../../../decreasing-event.md). The [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) for a [product measure](../../../../../../product-measure.md) gives

$$
P(A_1^c\cap A_2^c)\ge P(A_1^c)P(A_2^c)=(1-a)^2.
$$

The same correlation inequality for two [decreasing events](../../../../../../decreasing-event.md) follows from that for their increasing complements, since their [covariance](../../../../../../covariance.md) is unchanged. Thus

$$
1-P(A_1\cup A_2)\ge(1-a)^2.
$$

Both $1-a$ and the square root are nonnegative, so rearranging gives the [square-root bound for increasing events](../../../../../../square-root-bound-for-increasing-events.md):

$$
\boxed{P(A_1)\ge1-\sqrt{1-P(A_1\cup A_2)}.}
$$

No independence between the events themselves is asserted; independence is the coordinate property of the underlying [product measure](../../../../../../product-measure.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
