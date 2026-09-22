<h1 id="12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The base costs $ab$, the glass front costs $2ac$, the wooden rear costs $ac$, and the other two walls cost $2bc$. Thus minimize $C=ab+3ac+2bc$ subject to $abc=V>0$. With the [Lagrange multiplier](../../../../../lagrange-multiplier.md) convention $\nabla C=\lambda\nabla(abc)$, the equations are

$$
b+3c=\lambda bc,\qquad a+2c=\lambda ac,\qquad 3a+2b=\lambda ab.
$$

Multiply these by $a,b,c$, respectively. Comparing their equal right sides gives $ab=3ac=2bc$. Since all dimensions are positive, $a=2c$ and $b=3c$. The volume condition then yields

$$
\boxed{(a,b,c)=(2,3,1)\left(\frac V6\right)^{1/3}.}
$$

This stationary shape is the unique [global minimum](../../../../../global-minimum.md), not merely a candidate: the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) applied to the three cost terms gives

$$
C\geq3[(ab)(3ac)(2bc)]^{1/3}=3(6V^2)^{1/3},
$$

with equality exactly at those ratios. Therefore the least cost, in pounds in the specified units, is

$$
\boxed{C_{\min}=3\,6^{1/3}V^{2/3}=18\left(\frac V6\right)^{2/3}.}
$$

This is a [weighted open-box minimization](../../../../../weighted-open-box-minimization.md), with each pair of opposite walls combined into its appropriate positive face weight.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [12](../../12.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
