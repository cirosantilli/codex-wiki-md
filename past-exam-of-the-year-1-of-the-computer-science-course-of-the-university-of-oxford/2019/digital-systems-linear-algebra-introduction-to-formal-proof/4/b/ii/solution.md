<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the specified row and column, expand the two [matrix products](../../../../../../matrix-product.md) and reorder only [finite sums](../../../../../../finite-sum.md):

$$
\begin{aligned}
((AB)C)_{ij}
&=\sum_{k=1}^{p}\left(\sum_{\ell=1}^{n}A_{i\ell}B_{\ell k}\right)C_{kj}\\
&=\sum_{\ell=1}^{n}A_{i\ell}\left(\sum_{k=1}^{p}B_{\ell k}C_{kj}\right)
=(A(BC))_{ij}.
\end{aligned}
$$

The middle equality uses [scalar](../../../../../../scalar.md) [associativity](../../../../../../associative-property.md) and [distributivity](../../../../../../distributive-property.md), and the interchange of two [finite sums](../../../../../../finite-sum.md). Together with their equal [dimensions](../../../../../../dimension-vector-space.md), equality of every entry proves **$(AB)C=A(BC)$**.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
