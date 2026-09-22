<h1 id="p/p4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Proceed column by column. At stage $j=1,\ldots,n-2$, consider the entries below the diagonal in column $j$, indexed $j+1,\ldots,n$. If this tail is nonzero, part (c) provides a [Householder matrix](../../../../../householder-transformation.md) sending it to a multiple of its first coordinate vector. Embed this [matrix](../../../../../matrix.md) as an [orthogonal](../../../../../orthogonal-vectors.md) [matrix](../../../../../matrix.md) acting identically on coordinates $1,\ldots,j$, and apply the similarity transformation $A\mapsto Q_j^TAQ_j$. The tail's entries below row $j+1$ become zero. Symmetry is preserved, so the corresponding entries in row $j$ vanish too. If the tail is already zero, use the [identity](../../../../../identity-element.md) transformation.

Earlier reduced columns remain unchanged in their required zero positions: all their entries in the newly mixed tail coordinates were already zero, and the first $j$ coordinates are fixed. Thus each stage preserves the previous zeros while creating the next ones. After $n-2$ stages, all entries at distance greater than one from the diagonal vanish. With the product $Q=Q_1\cdots Q_{n-2}$ one has $Q^TQ=I$ and

$$
\boxed{Q^TAQ\text{ is symmetric tridiagonal}.}
$$

This constructive reduction uses only reflections on successive trailing subspaces.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
