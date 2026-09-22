<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Green-function representation](../../../../../green-function-representation.md) to integrate over the charged segment:

$$
\varphi(x,y)=-\frac1{4\pi\epsilon_0}\int_0^L\log((x-s)^2+y^2)\,ds+C_0.
$$

For $y\ne0$, a primitive with respect to $u$ is

$$
F(u,y)=u\log(u^2+y^2)-2u+2y\arctan(u/y),
$$

as direct [differentiation](../../../../../differentiation.md) verifies using the [derivative](../../../../../derivative.md) of [inverse tangent](../../../../../inverse-tangent.md). Therefore

$$
\boxed{\varphi(x,y)=-\frac{F(x,y)-F(x-L,y)}{4\pi\epsilon_0}+C_0.}
$$

This expression is even in $y$, since $y\arctan(u/y)$ is even. On $y=0$, take the continuous limit $F(u,0)=u\log u^2-2u$, with $u\log u^2=0$ at $u=0$. The finite segment has a logarithmically growing potential at large distance, but its [electric field](../../../../../electric-field-split.md) decays; the boundary condition constrains the field rather than the potential.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
