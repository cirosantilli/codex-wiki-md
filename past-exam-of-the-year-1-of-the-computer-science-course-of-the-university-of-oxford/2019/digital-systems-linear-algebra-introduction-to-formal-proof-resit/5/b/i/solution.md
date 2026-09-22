<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $r$ independent columns of $A$ that form a [basis](../../../../../../basis.md) of its [column space](../../../../../../column-space.md), and put them in $B\in\mathbb R^{m\times r}$. For each column $a_j$ of $A$, let $c_j$ be its coordinate [vector](../../../../../../vector.md) in that basis; put these coordinate [vectors](../../../../../../vector.md) in $C\in\mathbb R^{r\times n}$. The column equations $a_j=Bc_j$ give **$A=BC$**.

By construction $B$ has [full column rank](../../../../../../full-column-rank.md) $r$. The columns of $C$ corresponding to the selected basis columns are the standard [vectors](../../../../../../vector.md) of $\mathbb R^r$, so $C$ has [full row rank](../../../../../../full-row-rank.md) $r$. This proves the requested [rank factorization](../../../../../../rank-factorization.md). When $r=0$, $A=0$ and the corresponding empty-column and empty-row factors have the required shapes and rank zero.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof resit](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
