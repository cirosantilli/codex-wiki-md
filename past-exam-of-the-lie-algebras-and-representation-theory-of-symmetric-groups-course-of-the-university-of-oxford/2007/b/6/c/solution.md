<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First prove preservation of the row and column inequalities for distinct ordered labels. If $b>c_l$, [row insertion](../../../../../row-insertion.md) appends it to the first row, and the inequalities remain valid. Otherwise let $j$ be the first position with $c_j>b$. Replace $c_j$ by $b$ and insert the bumped $c_j$ in the second row. Its first larger entry is some $d_k$ with $k\le j$, because $d_j>c_j$. Replace $d_k$ by $c_j$ and put the bumped $d_k$ in the new third-row cell.

The first-larger-entry choices preserve strict row order. At column $k$, if $k<j$ the first-row entry is $c_k<c_j$, while if $k=j$ it is the new $b<c_j$. At column $j$ when $k<j$, the unchanged lower entry satisfies $d_j>c_j>b$. Every other old column keeps its previous inequalities. The new third-row entry is larger than the second-row first entry: for $k=1$ this is $d_1>c_j$, while for $k>1$ it follows from $d_k>d_1$. Thus the new shape $(l,l,1)$ is a [Young diagram](../../../../../young-diagram.md) with strictly increasing rows and columns. This proves the insertion assertion for the ordered-label convention.

There is a numbering qualification in the literal standard convention of part (a). If $T$ uses exactly $1,\ldots,2l$, an arbitrary missing natural number $b$ need not be $2l+1$. For example, inserting six into rows $(1,2);(3,4)$ produces $(1,2,6);(3,4)$, which has the order inequalities but not the labels $1,\ldots,5$. Thus **standardness with consecutive labels requires $b=2l+1$, or increasing relabelling afterward**. The printed wording is retained in the private transcription; [row insertion](../../../../../row-insertion.md) itself preserves the needed order structure.

## ↑ Ancestors (13)

1. [C](../c.md)
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
