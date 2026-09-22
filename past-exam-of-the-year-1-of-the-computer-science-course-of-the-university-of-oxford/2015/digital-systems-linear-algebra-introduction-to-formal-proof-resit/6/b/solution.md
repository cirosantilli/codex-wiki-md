<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Denote the five rows by $r_1,\ldots,r_5$. They satisfy

$$
r_1=r_2+r_4,\qquad r_5=r_2+r_4-r_3.
$$

Thus $r_2,r_3,r_4$ span the [row space](../../../../../row-space.md). They are [linearly independent](../../../../../linear-independence.md): in a [linear combination](../../../../../linear-combination.md) $\alpha r_2+\beta r_3+\gamma r_4=0$, coordinate 1 gives $\alpha=0$, coordinate 2 then gives $\beta=0$, and coordinate 4 gives $\gamma=0$. Therefore

$$
\boxed{\mathcal B_{\rm row}=\{(1,1,0,0),(0,1,1,0),(0,0,1,1)\},\qquad\operatorname{rank}A=3.}
$$

As an alternative [basis](../../../../../basis.md), the nonzero rows of the [reduced row echelon form](../../../../../reduced-row-echelon-form.md) are

$$
\operatorname{rref}(A)=\begin{pmatrix}
1&0&0&1\\0&1&0&-1\\0&0&1&1\\0&0&0&0\\0&0&0&0
\end{pmatrix}.
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
