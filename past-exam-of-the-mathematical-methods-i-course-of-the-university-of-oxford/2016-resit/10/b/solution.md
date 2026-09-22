<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [matrix exponential](../../../../matrix-exponential.md) acts entrywise on a diagonal matrix, so

$$
\boxed{e^B=\operatorname{diag}(e^3,e^4,1).}
$$

For the two-dimensional matrix $C$, direct multiplication gives $C^2=-C$, hence $C^n=(-1)^{n-1}C$ for $n\ge1$. Summing its defining [power series](../../../../power-series.md) gives

$$
\boxed{e^C=I+(1-e^{-1})C
=\begin{pmatrix}1&0\\1-e^{-1}&e^{-1}\end{pmatrix}.}
$$

Finally, $e^A=V\operatorname{diag}(e,e^2,e^5)V^{\mathsf T}$, so each diagonal entry is a weighted sum of these exponential eigenvalues, with weights equal to squared eigenvector components:

$$
\boxed{(e^A)_{11}=\frac{e^2}{3}+\frac{2e^5}{3},\qquad
(e^A)_{22}=(e^A)_{33}=\frac e2+\frac{e^2}{3}+\frac{e^5}{6}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2016 resit](../../../2016-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
