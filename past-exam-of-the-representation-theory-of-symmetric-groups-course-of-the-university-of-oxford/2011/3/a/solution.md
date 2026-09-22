<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [permutations](../../../../permutation.md), the [Robinson-Schensted-Knuth correspondence](../../../../robinson-schensted-knuth-correspondence.md), also called the [permutation](../../../../permutation.md) case of [RSK](../../../../robinson-schensted-knuth-correspondence.md), is a [bijection](../../../../bijection.md)

$$
\boxed{S_n\longleftrightarrow\{(P,Q):P,Q\text{ standard tableaux of the same shape }\lambda\vdash n\}.}
$$

Process the word $\sigma(1),\ldots,\sigma(n)$ by [row insertion](../../../../row-insertion.md) to form $P$. To insert a new entry $a$, replace the leftmost entry of the first row larger than $a$ and bump that displaced entry into the next row by the same rule. If a row has no larger entry, append $a$ at its end and stop. Exactly one outer-corner cell is added. Record the current insertion time in that new cell of $Q$.

Rows stay increasing by the choice of the leftmost larger entry. The inequalities between successive bumped entries and the entries above them preserve increasing columns. Successive shapes are [Young diagrams](../../../../young-diagram.md), so the recording labels also increase across rows and down columns. Reverse insertion at the corner labelled $n$ in $Q$ recovers the last input entry; repeating it recovers the full [permutation](../../../../permutation.md), proving bijectivity. The more general [RSK correspondence](../../../../robinson-schensted-knuth-correspondence.md) extends this construction to suitable two-line arrays and [semistandard tableaux](../../../../semistandard-young-tableau.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
