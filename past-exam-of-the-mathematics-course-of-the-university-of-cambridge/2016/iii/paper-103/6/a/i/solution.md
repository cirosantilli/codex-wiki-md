<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [near Young tableau](../../../../../../../near-young-tableau.md) is a filling of a [Young diagram](../../../../../../../young-diagram.md) by distinct entries from a totally ordered alphabet, increasing along rows and down columns; the entries need not be $1,\ldots,n$. For [row insertion](../../../../../../../row-insertion.md) of $x$, scan the first row for its leftmost entry larger than $x$. If one exists, replace it by $x$ and insert the displaced entry into the next row by the same rule. Otherwise append $x$ to the row and stop. Continue until a new outer-corner box is appended.

The [Robinson–Schensted correspondence](../../../../../../../robinson-schensted-correspondence.md) inserts the letters $x_1,\ldots,x_n$ of a permutation successively to form $P$. Whenever the $k$th insertion creates a new cell, put $k$ in that cell of a second tableau $Q$. [Row insertion](../../../../../../../row-insertion.md) preserves increasing rows and columns, so $P$ is standard; the sequence of growing diagrams makes $Q$ standard, with the same shape. To reverse the construction, remove the box carrying the largest label in $Q$, and reverse the bumping in $P$: in each row above, exchange the carried entry with the rightmost smaller entry, continuing up to the first row. The final expelled entry is the last letter of the permutation. Repeating recovers the whole permutation, establishing the [bijection](../../../../../../../bijection.md) with pairs of [standard Young tableaux](../../../../../../../standard-young-tableau.md) of a common shape.

For the bumping inequality, each displaced entry is the first entry strictly larger than the incoming one. Thus every step replaces a larger entry with a smaller entry and carries that larger value downwards. Consequently **the bumped values strictly increase**:

$$
\boxed{x<x'<x''<x'''<\cdots}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
