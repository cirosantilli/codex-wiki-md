<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a$ be the single entry in the second row of $P$. It lies in $\{2,\ldots,n\}$; the first row is all the other entries in increasing order. Consider the [adjacent transposition](../../../../adjacent-transposition.md) $\sigma=(a-1,a)$, whose word is

$$
1,2,\ldots,a-2,\ a,\ a-1,\ a+1,\ldots,n.
$$

The first $a-1$ entries append in increasing order to the first row. At insertion time $a$, the value $a-1$ bumps $a$ into the second row, creating its only cell. Every later entry appends to the first row. Thus the insertion tableau has second-row entry $a$ and all other entries in the first row, precisely $P$.

The recording tableau also has second-row entry $a$, the time of the unique bump, and all other time labels in increasing first-row order. It too is $P$. Bijectivity of the correspondence therefore gives

$$
\boxed{\operatorname{RSK}^{-1}(P,P)=(a-1,a).}
$$

This includes $n=2,a=2$. It identifies the actual [permutation](../../../../permutation.md) without needing a general theorem about [involutions](../../../../involution.md).

This is [RSK of an adjacent transposition](../../../../rsk-of-an-adjacent-transposition.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the representation Theory of Symmetric Groups course of the University of Oxford](../../../split.md)
5. [Representation Theory of Symmetric Groups course of the University of Oxford](../../../../representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
