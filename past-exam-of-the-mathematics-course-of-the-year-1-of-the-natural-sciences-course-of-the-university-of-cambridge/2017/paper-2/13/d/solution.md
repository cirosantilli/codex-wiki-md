<h1 id="13/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Evaluate the [line integral](../../../../../line-integral.md) along the three coordinate segments, treating coordinates not changing along a segment as constants. On the first segment, $y=z=0$, so $F_x=0$ and the contribution is zero. On the second segment,

$$
\int_0^yF_y(x,\eta,0)\,d\eta=\int_0^y(x^2-2\eta)\,d\eta=x^2y-y^2.
$$

On the final segment,

$$
\int_0^zF_z(x,y,\zeta)\,d\zeta
=\int_0^z(-3x\zeta^2-1)\,d\zeta=-xz^3-z.
$$

The [fundamental theorem for line integrals](../../../../../fundamental-theorem-for-line-integrals.md) therefore gives

$$
\boxed{\Phi(x,y,z)=x^2y-y^2-xz^3-z+C}.
$$

Taking its [gradient](../../../../../gradient.md) verifies each component of the field. The constant is $C=\Phi(0,0,0)$; the field specifies only potential differences because the [gradient](../../../../../gradient.md) of every constant is zero.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [13](../../13.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
