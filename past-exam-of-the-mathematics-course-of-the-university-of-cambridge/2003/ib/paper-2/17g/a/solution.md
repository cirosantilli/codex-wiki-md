<h1 id="17g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A Hermitian two-by-two [matrix](../../../../../../matrix.md) has the form

$$
A=\begin{pmatrix}\alpha&z\\\bar z&\delta\end{pmatrix},\qquad
\alpha,\delta\in\mathbb R,\quad z\in\mathbb C.
$$

Addition and real scalar multiplication preserve this condition, and the two diagonal entries plus the real and imaginary parts of $z$ give four independent real coordinates. Thus **$S$ is a real four-dimensional vector space**. The [trace](../../../../../../matrix-trace.md) product is real because $\overline{\operatorname{tr}(AB)}=\operatorname{tr}(BA)=\operatorname{tr}(AB)$; this also proves symmetry of $b$.

Directly, $\operatorname{tr}(A^2)=\alpha^2+\delta^2+2|z|^2$ and $(\operatorname{tr}A)^2=\alpha^2+2\alpha\delta+\delta^2$. Hence

$$
\boxed{b(A,A)=|z|^2-\alpha\delta=-\det A.}
$$

Since $\operatorname{tr}I=2$ and $\operatorname{tr}(AI)=\operatorname{tr}A$,

$$
\boxed{b(A,I)=-\frac12\operatorname{tr}A.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
