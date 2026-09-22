<h1 id="14/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose any nonzero auxiliary [vector](../../../../../vector.md) $\mathbf q$ not collinear with $\mathbf p$. Then $\mathbf p,\mathbf q,\mathbf p\times\mathbf q$ form a [basis](../../../../../basis.md), so write

$$
\mathbf x=\alpha\mathbf p+\beta\mathbf q+\gamma(\mathbf p\times\mathbf q).
$$

Taking the [dot product](../../../../../dot-product.md) with $\mathbf p$ gives $\alpha|\mathbf p|^2+\beta\mathbf p\cdot\mathbf q=k$. This separates the two cases requested in the hint.

If $\mathbf p\cdot\mathbf q\ne0$, choose $\alpha,\gamma$ freely and solve for $\beta$:

$$
\boxed{\mathbf x=\alpha\mathbf p+
\frac{k-\alpha|\mathbf p|^2}{\mathbf p\cdot\mathbf q}\,\mathbf q
+\gamma(\mathbf p\times\mathbf q),\qquad \alpha,\gamma\in\mathbb R.}
$$

If $\mathbf p\cdot\mathbf q=0$, the coefficient of $\mathbf p$ is fixed and the other two are free:

$$
\boxed{\mathbf x=\frac{k}{|\mathbf p|^2}\mathbf p
+\beta\mathbf q+\gamma(\mathbf p\times\mathbf q),\qquad\beta,\gamma\in\mathbb R.}
$$

These formulas describe the whole [plane](../../../../../plane.md) with normal $\mathbf p$, including $k=0$. Completeness follows from the [basis](../../../../../basis.md) expansion, not only from checking that the displayed [vectors](../../../../../vector.md) satisfy the equation. The [parametrization of a plane with an auxiliary vector](../../../../../parametrization-of-a-plane-with-an-auxiliary-vector.md) also gives a single formula valid in both cases.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [14](../../14.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
