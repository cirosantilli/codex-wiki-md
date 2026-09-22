<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Every assignment determines a unique [set partition](../../../../../../../set-partition.md) into its nonempty colour classes. If there are $k$ such [blocks of a set partition](../../../../../../../block-of-a-set-partition.md), there are $A(n,k)$ choices for that [set partition](../../../../../../../set-partition.md). For each fixed choice, assign distinct colours to the $k$ [blocks of a set partition](../../../../../../../block-of-a-set-partition.md) in

$$
(x)_k=x(x-1)\cdots(x-k+1)
$$

ways. Although the [blocks of a set partition](../../../../../../../block-of-a-set-partition.md) are unlabelled, they are distinguishable by their elements: ordering them temporarily, for instance by their least elements, counts each assignment exactly once. The [falling factorial](../../../../../../../falling-factorial.md) is zero when $k>x$, as it should be. Summing over the possible numbers of used colours proves

$$
\boxed{x^n=\sum_{k=1}^n A(n,k)(x)_k.}
$$

Here $A(n,k)$ is the [Stirling number of the second kind](../../../../../../../stirling-numbers-of-the-second-kind.md). Both sides are [polynomials](../../../../../../../polynomial-split.md) in $x$ and agree at infinitely many integers $x>2$, so the identity also holds for every real $x$, including $0,1,2$. This extension will justify substituting the [random variable](../../../../../../../random-variable-split.md) $X$ in part (iii).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
