<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two nonzero proper [invariant subspaces](../../../../../../invariant-subspace.md) are

$$
\boxed{U=\operatorname{span}\{e_3\},\qquad W=\operatorname{span}\{e_1,e_2\}.}
$$

Both are preserved by the [rotation](../../../../../../rotation-mathematics.md). To show there are no others, note that

$$
P=\frac{I+T^2}{2},\qquad P(x,y,z)=(0,0,z)
$$

is the [linear projection](../../../../../../projection-linear-algebra.md) onto $U$, and $I-P$ is the [linear projection](../../../../../../projection-linear-algebra.md) onto $W$. Every [invariant subspace](../../../../../../invariant-subspace.md) $L$ is preserved by $I,T^2$, and hence by both of these [linear projections](../../../../../../projection-linear-algebra.md). Therefore

$$
L=(L\cap U)\oplus(L\cap W).
$$

Because $U$ has [dimension](../../../../../../dimension-vector-space.md) one, $L\cap U$ is either $0$ or $U$. If $L\cap W$ contains a nonzero $v=(a,b,0)$, it also contains $Tv=(-b,a,0)$. These two [vectors](../../../../../../vector.md) are [linearly independent](../../../../../../linear-independence.md), because their two-dimensional [determinant](../../../../../../determinant.md) is $a^2+b^2>0$. They [span](../../../../../../linear-span.md) $W$, so $L\cap W$ is either $0$ or $W$. The only possibilities for $L$ are therefore $0,U,W,V$.

Finally every $(x,y,z)$ has the unique decomposition $(0,0,z)+(x,y,0)$, with one summand in each of $U,W$. Hence

$$
\boxed{V=U\oplus W.}
$$

This also illustrates how [invariant subspaces of a quarter-turn in three dimensions](../../../../../../invariant-subspaces-of-a-quarter-turn-in-three-dimensions.md) can be classified by [linear projections](../../../../../../projection-linear-algebra.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
