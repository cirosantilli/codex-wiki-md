<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [divergence](../../../../../divergence.md) is $y^2+z^2+x^2$. Over the cube $[-1/2,1/2]^3$, each squared-coordinate term has integral $\int_{-1/2}^{1/2}s^2ds=1/12$, while the other two coordinate integrals have length one. Thus

$$
\boxed{\int_V\nabla\cdot F\,dV=3\cdot\frac1{12}=\frac14.}
$$

Compute the surface [flux](../../../../../flux.md) separately. On $x=1/2$, the outward normal is $e_x$ and $F\cdot n=y^2/2$, giving flux $1/24$. On $x=-1/2$, the normal is $-e_x$, so $F\cdot n=-xy^2=y^2/2$, again giving $1/24$. The two $y$ faces similarly give $z^2/2$ each, and the two $z$ faces give $x^2/2$ each. All six face integrals therefore give

$$
\boxed{\int_{\partial V}F\cdot dS=6\cdot\frac1{24}=\frac14.}
$$

The independently evaluated values agree, verifying the [divergence theorem](../../../../../divergence-theorem.md) for this field and cube.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
