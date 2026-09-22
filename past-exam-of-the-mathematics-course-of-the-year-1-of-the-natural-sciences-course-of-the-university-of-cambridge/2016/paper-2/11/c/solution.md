<h1 id="11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $D=\mathbf a\cdot(\mathbf b\times\mathbf c)>0$. Since these vectors form a [basis](../../../../../basis.md), write $\mathbf r=\alpha\mathbf a+\beta\mathbf b+\gamma\mathbf c$. The [reciprocal basis](../../../../../reciprocal-basis.md) gives

$$
\alpha=\frac{\mathbf r\cdot(\mathbf b\times\mathbf c)}D,\qquad
\beta=\frac{\mathbf r\cdot(\mathbf c\times\mathbf a)}D,\qquad
\gamma=\frac{\mathbf r\cdot(\mathbf a\times\mathbf b)}D.
$$

A point is in the closed [tetrahedron](../../../../../tetrahedron.md) precisely when it is a [convex combination](../../../../../convex-combination.md) of the four vertices, with weights $1-\alpha-\beta-\gamma,\alpha,\beta,\gamma$. Thus the necessary and sufficient conditions are

$$
\boxed{\begin{gathered}
\mathbf r\cdot(\mathbf b\times\mathbf c)\geq0,\quad
\mathbf r\cdot(\mathbf c\times\mathbf a)\geq0,\quad
\mathbf r\cdot(\mathbf a\times\mathbf b)\geq0,\\
\mathbf r\cdot(\mathbf a\times\mathbf b+\mathbf b\times\mathbf c+\mathbf c\times\mathbf a)\leq D.
\end{gathered}}
$$

These four [half-spaces](../../../../../half-space.md) are the four inward sides of its faces. This is [tetrahedron membership via scalar triple products](../../../../../tetrahedron-membership-via-scalar-triple-products.md); making all inequalities strict describes the interior.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [11](../../11.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
