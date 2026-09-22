<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Applying the recurrence in source item order gives the complete table

$$
\begin{array}{c|rrrrrrrr}
j\backslash b&0&1&2&3&4&5&6&7\\\hline
0&0&0&0&0&0&0&0&0\\
1&0&0&15&15&15&15&15&15\\
2&0&0&15&18&18&33&33&33\\
3&0&0&15&18&21&33&36&39\\
4&0&0&15&18&21&33&36&40
\end{array}
$$

At $(4,7)$ inclusion wins, since $25+D(3,2)=40>D(3,7)=39$. Thus $x_4=1$ and the residual capacity is two. Items three and two are too heavy for it, and item one exactly fits. Consequently

$$
\boxed{x^*=(1,0,0,1),\qquad p^Tx^*=40.}
$$

Its weight is $2+5=7$. The recurrence proves that no binary selection with capacity seven has greater profit.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
