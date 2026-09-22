<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use four-variable [Karnaugh maps](../../../../../karnaugh-map.md) with rows $AB=00,01,11,10$ and columns $Cx=00,01,11,10$, both in [Gray code](../../../../../gray-code.md) order. A dash denotes an unused present state. The maps for the three next-state bits are

$$
\begin{array}{c|cccc}
A^+&00&01&11&10\\\hline
00&0&0&0&0\\01&0&0&1&0\\11&-&-&-&-\\10&0&0&-&-
\end{array}\qquad
\begin{array}{c|cccc}
B^+&00&01&11&10\\\hline
00&0&0&1&0\\01&1&1&0&0\\11&-&-&-&-\\10&0&1&-&-
\end{array}\qquad
\begin{array}{c|cccc}
C^+&00&01&11&10\\\hline
00&0&1&0&0\\01&1&0&0&0\\11&-&-&-&-\\10&0&0&-&-
\end{array}.
$$

For $A^+$, join its sole one with the dash directly below it. For $B^+$, use the four-cell groups $Ax$ and $B\bar C$, and the two-cell group $\bar BCx$; the last group wraps between the top and bottom rows. For $C^+$, join the one at row $01$, column $00$ to the dash below it; the one at row $00$, column $01$ is isolated. These [prime implicants](../../../../../prime-implicant.md) give

$$
\boxed{D_A=BCx,\qquad D_B=Ax+B\bar C+\bar BCx,\qquad D_C=B\bar C\bar x+\bar A\bar B\bar Cx.}
$$

Here products mean [Boolean conjunction](../../../../../logical-conjunction.md) and sums mean [Boolean disjunction](../../../../../logical-disjunction.md). The $D$ inputs are the desired next-state bits of the three [D flip-flops](../../../../../d-flip-flop.md). The equations are independent of the unused values except for the explicitly chosen [Karnaugh map](../../../../../karnaugh-map.md) groups.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
