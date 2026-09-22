<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrate $f_x=ye^x$ with respect to $x$, obtaining $f=ye^x+g(y,z)$. Matching $f_y=e^x+2yz^3$ gives $g_y=2yz^3$, so $g=y^2z^3+h(z)$. Finally, $f_z=3y^2z^2+h'(z)$ must equal the third component, so $h'=0$. Thus a [scalar potential](../../../../../scalar-potential.md) is

$$
\boxed{f(x,y,z)=ye^x+y^2z^3+C,\qquad v=\nabla f.}
$$

The [fundamental theorem for line integrals](../../../../../fundamental-theorem-for-line-integrals.md) now gives $\int_Cv\cdot dr=f(1,1,1)-f(0,0,0)=e+1$ for either path, confirming both direct computations. Since the [curl of a gradient](../../../../../curl-of-a-gradient.md) is zero for this smooth [function](../../../../../function-split.md), it also confirms the result in part (b). The potential is defined throughout $\mathbb R^3$, so no domain obstruction to [path independence](../../../../../path-independence.md) occurs.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
