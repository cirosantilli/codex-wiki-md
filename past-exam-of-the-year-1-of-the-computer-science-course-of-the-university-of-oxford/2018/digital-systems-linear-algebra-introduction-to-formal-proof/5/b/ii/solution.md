<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let column $j$ of $A^{-1}$ be $x$, so $Ax=e_j$. Every diagonal entry of the invertible [lower triangular matrix](../../../../../../lower-triangular-matrix.md) $A$ is nonzero, since its [determinant](../../../../../../determinant.md) is the product of those entries. In row one through row $j-1$, the right-hand side is zero. [Forward substitution](../../../../../../forward-substitution.md) first gives $x_1=0$, then $x_2=0$, and successively $x_i=0$ for all $i<j$. These are precisely the entries above the diagonal in column $j$ of $A^{-1}$. Every column satisfies this, proving that **$A^{-1}$ is lower triangular**. This is [triangularity of an inverse matrix](../../../../../../triangularity-of-an-inverse-matrix.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
