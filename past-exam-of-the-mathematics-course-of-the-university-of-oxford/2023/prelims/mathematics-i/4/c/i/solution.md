<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Write $r=(r_1,\ldots,r_n)^T$. The [linear map](../../../../../../../linear-map.md) represented by $A$ has the form

$$
Ax=(r^Tx)e_i.
$$

The [image of a linear map](../../../../../../../image-of-a-linear-map.md) here is contained in the one-dimensional [linear span](../../../../../../../linear-span.md) of $e_i$, so its [matrix rank](../../../../../../../matrix-rank.md) is at most one. The [rank-nullity theorem](../../../../../../../rank-nullity-theorem.md) yields

$$
\boxed{\dim\ker A=n-\operatorname{rank}A\ge n-1.}
$$

Thus the solution space of $Ax=0$, namely the zero [eigenspace](../../../../../../../eigenspace.md) when zero is an [eigenvalue](../../../../../../../eigenvalue.md), contains at least $n-1$ [linearly independent vectors](../../../../../../../linear-independence.md). If $r=0$ its [dimension](../../../../../../../dimension-vector-space.md) is $n$; otherwise it is $n-1$. When $n=1$ the asserted lower bound is zero, even if zero is not an [eigenvalue](../../../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [c](../../c.md)
3. [4](../../../4.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
