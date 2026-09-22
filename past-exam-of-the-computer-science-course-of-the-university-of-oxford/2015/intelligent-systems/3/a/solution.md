<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use one [variable](../../../../../variable-mathematics.md) $X_{r,c}$ for each cell, with $1\le r,c\le9$. An empty cell has [constraint domain](../../../../../constraint-domain.md) $\{1,\ldots,9\}$; a clue containing $d$ has singleton [constraint domain](../../../../../constraint-domain.md) $\{d\}$. Thus all clues are retained automatically.

For every row $r$ impose $\operatorname{AllDifferent}(X_{r,1},\ldots,X_{r,9})$, and for every column $c$ impose $\operatorname{AllDifferent}(X_{1,c},\ldots,X_{9,c})$. For each $a,b\in\{0,1,2\}$ impose an [all-different constraint](../../../../../all-different-constraint.md) on

$$
\{X_{3a+i,3b+j}:1\le i,j\le3\}.
$$

These are the nine prescribed boxes. There are 27 [all-different constraints](../../../../../all-different-constraint.md) altogether. Nine pairwise distinct values chosen from a [set](../../../../../set-split.md) of nine values must use every value exactly once, so these restrictions are precisely the [Sudoku](../../../../../sudoku.md) requirements. Equivalently, expand each [all-different constraint](../../../../../all-different-constraint.md) into pairwise [binary constraints](../../../../../binary-constraint.md) $X_{r,c}\ne X_{r',c'}$ for cells sharing a row, column, or box.

$$
\boxed{81\text{ variables, clue-restricted domains, and }27\text{ all-different constraints}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
