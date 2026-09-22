<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention that insertion returns the insertion tableau $P$ first and the recording tableau $Q$ second. Successive row insertions of $3,4,1,6,7,5,2$ give

$$
\boxed{P=\begin{array}{llll}1&2&5&7\\3&4\\6\end{array},\qquad Q=\begin{array}{llll}1&2&4&5\\3&6\\7\end{array}.}
$$

For example inserting five bumps six to the second row, and the final insertion of two bumps four from the first row and six from the second, creating the third row. The newly created boxes at these steps receive recording labels six and seven respectively.

The deletion input is this pair with the two tableaux interchanged. The symmetry property of [RSK](../../../../../robinson-schensted-knuth-correspondence.md) therefore gives the inverse permutation. One can also reverse-insert the boxes in descending recording-label order. The result is

$$
\boxed{\operatorname{del}=\begin{pmatrix}1&2&3&4&5&6&7\\3&7&1&2&6&4&5\end{pmatrix}.}
$$

Indeed the displayed second row lists the positions of one through seven in the original permutation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
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
