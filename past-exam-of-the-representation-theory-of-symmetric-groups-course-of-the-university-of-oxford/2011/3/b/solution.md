<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\lambda=(a,b)$ with $a\geq b>0$. If the removed corner is in the first row, it must be its last cell, with $a>b$. Remove that entry and output it as $v$; all remaining row and column inequalities persist, and the shape is $(a-1,b)$.

If the corner is the last cell of the second row, remove its value $c$. In the first row find the rightmost entry $d<c$, replace it by $c$, and output $v=d$. Such an entry exists: the first-row cell above the removed corner has smaller value than $c$. The chosen position is therefore at least column $b$.

The new first-row entry exceeds all entries to its left, while every entry to its right is larger than $c$ by the rightmost-choice rule. After deleting the lower corner, no second-row cell remains below the changed position, since that row now has [length](../../../../length.md) $b-1$. Thus all column inequalities remain valid too. The resulting shape is $(a,b-1)$, omitting a zero part if $b=1$.

$$
\boxed{\operatorname{shape}(P^-)=\lambda\setminus\{x\}.}
$$

The entries remain distinct and increasing along rows and columns, but the missing label is the ejected $v$, not necessarily the original corner value. The resulting tableau is therefore standard on its remaining ordered entry [set](../../../../set-split.md), the generalized-standard convention in the question.

## ↑ Ancestors (12)

1. [B](../b.md)
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
