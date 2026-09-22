<h1 id="5/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The first left multiplication swaps rows three and four. The final right multiplication swaps columns three and four, restoring the two diagonal ones to their diagonal positions while exchanging the earlier entries of the two rows. Therefore

$$
ENE=\begin{pmatrix}1&0&0&0\\N_{21}&1&0&0\\N_{41}&N_{42}&1&0\\N_{31}&N_{32}&0&1\end{pmatrix}.
$$

The two specified zeros at positions $(3,4)$ and $(4,3)$ are important. Conjugation by this [permutation matrix](../../../../../../permutation-matrix.md) preserves this restricted lower triangular pattern; it would not preserve lower triangularity for an arbitrary [matrix](../../../../../../matrix.md) with a nonzero $(4,3)$ entry.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
