<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the hook cycle [partition](../../../../../integer-partition.md) as $\mu=(k,1^{n-k})$, $1\le k\le n$. At the identity, the [representation](../../../../../group-representation.md) [dimension](../../../../../dimension-vector-space.md) is $n-1$: a [standard tableau](../../../../../standard-young-tableau.md) of shape $(2,1^{n-2})$ is determined by the entry in its top-right box, any one of $2,\ldots,n$.

For $2\le k\le n-2$, the only removable [border strip](../../../../../rim-hook.md) of length $k$ is the vertical bottom strip. Its height is $k-1$, and the remaining hook has size $n-k$ and [dimension](../../../../../dimension-vector-space.md) $n-k-1$. A strip of length $n-1$ would leave the top-left box but disconnect the removed top-right box from the removed column, so none exists and the value is zero. For $k=n$, the whole hook is a [border strip](../../../../../rim-hook.md) of height $n-2$ and contributes $(-1)^{n-2}$. These cases combine as

$$
\boxed{\chi^{(2,1^{n-2})}(k,1^{n-k})=\begin{cases}n-1,&k=1,\\(-1)^{k-1}(n-k-1),&2\le k\le n.\end{cases}}
$$

In particular the formula includes zero at $k=n-1$ and the full-cycle sign at $k=n$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
