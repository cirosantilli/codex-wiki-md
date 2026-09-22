<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First convert the printed cycle to one-line notation:

$$
\sigma=(3,6,5,2,4,7,8,1).
$$

Apply [row insertion](../../../../../row-insertion.md) to these values, recording the insertion time in each new cell. The successive insertion-tableau row lists are

$$
\begin{array}{c|l}
1&(3)\\
2&(3,6)\\
3&(3,5);(6)\\
4&(2,5);(3);(6)\\
5&(2,4);(3,5);(6)\\
6&(2,4,7);(3,5);(6)\\
7&(2,4,7,8);(3,5);(6)\\
8&(1,4,7,8);(2,5);(3);(6)
\end{array}.
$$

Therefore the [Robinson-Schensted-Knuth correspondence](../../../../../robinson-schensted-knuth-correspondence.md) gives

$$
\boxed{P_\sigma=\begin{array}{rrrr}1&4&7&8\\2&5\\3\\6\end{array},\qquad
Q_\sigma=\begin{array}{rrrr}1&2&6&7\\3&5\\4\\8\end{array}.}
$$

Both have shape $(4,2,1,1)$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
