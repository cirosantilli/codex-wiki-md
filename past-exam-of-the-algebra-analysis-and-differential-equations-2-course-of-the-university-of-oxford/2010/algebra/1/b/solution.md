<h1 id="algebra/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $S^b=0$. Use the increasing chain of [vector subspaces](../../../../../vector-subspace.md)

$$
0=\ker S^0\subseteq\ker S\subseteq\ker S^2\subseteq\cdots\subseteq\ker S^b=V.
$$

Choose a [basis](../../../../../basis.md) successively, extending a [basis](../../../../../basis.md) of each [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) to one of the next [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md). If a [basis](../../../../../basis.md) [vector](../../../../../vector.md) first enters at level $j$, its [image](../../../../../image-of-a-function.md) under $S$ belongs to $\ker S^{j-1}$, spanned entirely by earlier [basis](../../../../../basis.md) vectors. Thus every [matrix](../../../../../matrix.md) column has nonzero entries only above its diagonal: the [matrix](../../../../../matrix.md) is [strictly upper triangular](../../../../../strictly-upper-triangular-matrix.md).

Conversely, for such a [matrix](../../../../../matrix.md) and its ordered [basis](../../../../../basis.md) $e_1,\ldots,e_n$, one has $S\langle e_1,\ldots,e_j\rangle\subseteq\langle e_1,\ldots,e_{j-1}\rangle$. Iterating $n$ times kills every [vector](../../../../../vector.md). Hence $\boxed{S^n=0}$, establishing both directions without assuming a Jordan form.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [Algebra](../../../algebra.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
