<h1 id="s/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Begin with $u=v=0$ and the printed matching $\{(1,1),(3,2),(5,3)\}$. Grow an alternating [tree](../../../../../tree-graph-theory-split.md) from unmatched row two. Its tight [edge](../../../../../edge-of-a-graph.md) reaches column two, whose matched row is three. Thus the reached row set is $S=\{2,3\}$ and the reached column set is $T=\{2\}$. Among unreached columns the reduced costs are $(6,5,4,4)$ from row two and $(3,4,2,3)$ from row three, so their minimum is two.

Increase $u_2,u_3$ by two and decrease $v_2$ by two. The new tight [edge](../../../../../edge-of-a-graph.md) $(3,4)$ reaches an unmatched column. Augment along $2\to2\to3\to4$, replacing $(3,2)$ by $(2,2),(3,4)$. The matching becomes $\{(1,1),(2,2),(3,4),(5,3)\}$.

Now grow from unmatched row four. [Edge](../../../../../edge-of-a-graph.md) $(4,1)$ reaches matched row one, and [edge](../../../../../edge-of-a-graph.md) $(1,5)$ reaches unmatched column five. Augment along $4\to1\to1\to5$, replacing $(1,1)$ by $(4,1),(1,5)$. This yields

$$
\boxed{\{(1,5),(2,2),(3,4),(4,1),(5,3)\},\qquad\text{cost }2.}
$$

No further potential update is needed. The final potentials are $u=(0,2,2,0,0)$ and $v=(0,-2,0,0,0)$. Their reduced-cost [matrix](../../../../../matrix.md) is

$$
(c_{ij}-u_i-v_j)=
\begin{pmatrix}0&2&2&1&0\\4&0&3&2&2\\1&0&2&0&1\\0&5&1&2&1\\3&3&0&0&2\end{pmatrix}.
$$

Every entry is nonnegative and every chosen entry is zero. The dual sum is $\sum u_i+\sum v_j=2$, so part (a) certifies optimality.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [S](../../../s.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
