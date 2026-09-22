<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Write $\boldsymbol\Delta=\boldsymbol d-\boldsymbol b$. At an intersection, $\boldsymbol\Delta=\lambda\boldsymbol a-\mu\boldsymbol c$, so its [scalar triple product](../../../../scalar-triple-product.md) with $\boldsymbol a,\boldsymbol c$ vanishes. The expression in the question is exactly

$$
\boldsymbol a\cdot(\boldsymbol c\times\boldsymbol d)+\boldsymbol c\cdot(\boldsymbol a\times\boldsymbol b)
=\boldsymbol\Delta\cdot(\boldsymbol a\times\boldsymbol c)=0.
$$

Under a shift of origin by $\boldsymbol h$, the direction vectors $\boldsymbol a,\boldsymbol c$ stay fixed, while $\boldsymbol b,\boldsymbol d$ both change by $-\boldsymbol h$. Thus $\boldsymbol\Delta$ and the condition are invariant. For nonparallel lines this is also sufficient for intersection; for parallel lines it only asserts coplanarity and need not imply intersection.

Put $\delta\lambda=\lambda_2-\lambda_1$ and $\delta\mu=\mu_2-\mu_1$. Then $\boldsymbol x_2-\boldsymbol x_1=\delta\lambda\boldsymbol a$ and $\boldsymbol x_4-\boldsymbol x_1=(\boldsymbol x_3-\boldsymbol x_1)+\delta\mu\boldsymbol c$. Bilinearity of the [cross product](../../../../cross-product.md) gives

$$
\begin{aligned}
[(\boldsymbol x_3-\boldsymbol x_1)\times(\boldsymbol x_4-\boldsymbol x_1)]\cdot(\boldsymbol x_2-\boldsymbol x_1)
&=\delta\mu\,\delta\lambda\,[(\boldsymbol\Delta+\mu_1\boldsymbol c-\lambda_1\boldsymbol a)\times\boldsymbol c]\cdot\boldsymbol a\\
&=-\delta\mu\,\delta\lambda\,\boldsymbol\Delta\cdot(\boldsymbol a\times\boldsymbol c)\\
&=\boldsymbol\Delta\cdot[(\boldsymbol x_4-\boldsymbol x_3)\times(\boldsymbol x_2-\boldsymbol x_1)].
\end{aligned}
$$

The [tetrahedron](../../../../tetrahedron.md) volume is one sixth of the [absolute value](../../../../absolute-value.md) of this triple product. Sliding either vertex pair along its line preserves $|\delta\lambda|$ or $|\delta\mu|$, because its separation is fixed and the direction vectors are fixed. Thus the volume is unchanged, including the zero-volume coplanar case. This is [tetrahedron volume under sliding opposite edges](../../../../tetrahedron-volume-under-sliding-opposite-edges.md).

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
