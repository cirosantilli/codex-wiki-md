<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Compute twice the four opposite face areas and their weighted vertex average:

$$
\begin{aligned}
w_A&\leftarrow\|(C-B)\times(D-B)\|,\\
w_B&\leftarrow\|(C-A)\times(D-A)\|,\\
w_C&\leftarrow\|(B-A)\times(D-A)\|,\\
w_D&\leftarrow\|(B-A)\times(C-A)\|,\\
w&\leftarrow w_A+w_B+w_C+w_D,\\
I&\leftarrow(w_AA+w_BB+w_CC+w_DD)/w.
\end{aligned}
$$

These positive weights make $I$ an interior [convex combination](../../../../../../convex-combination.md). To verify the [incenter of a tetrahedron](../../../../../../incenter-of-a-tetrahedron.md), put $\Delta=|(B-A)\cdot((C-A)\times(D-A))|$. The altitude from $A$ to its opposite face is $\Delta/w_A$. Signed distance to that face is affine and vanishes at the other three vertices, so $I$ has distance $(w_A/w)(\Delta/w_A)=\Delta/w$. The same argument works for every face. Hence

$$
\boxed{I\text{ is the incentre},\qquad r_{\rm in}=\Delta/w.}
$$

The sphere of radius $r_{\rm in}$ centered at $I$ is tangent to all four faces. Equality of the four distances conversely forces these face-area weights, proving uniqueness.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
