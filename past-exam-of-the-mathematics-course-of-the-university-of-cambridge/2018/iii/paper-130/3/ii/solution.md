<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the isolating sets from the preceding part and make the finite disjointification

$$
B_n=A_n\setminus\bigcup_{j<n}A_j.
$$

For $j<n$, $A_j\notin U_n$, so $A_j^c\in U_n$. Therefore

$$
B_n=A_n\cap\bigcap_{j<n}A_j^c\in U_n
$$

by finite-intersection closure of the [ultrafilter](../../../../../../ultrafilter.md). If $m\ne n$, $B_n\subseteq A_n$ and $A_n\notin U_m$ imply $B_n\notin U_m$. Also $B_n$ avoids every earlier $A_j$, hence every earlier $B_j$. Thus

$$
\boxed{B_n\cap B_m=\varnothing\ (n\ne m),\qquad B_n\in U_m\Longleftrightarrow m=n.}
$$

Only finite intersections were used; no countable-intersection closure of an [ultrafilter](../../../../../../ultrafilter.md) is being assumed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
