<h1 id="15/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the needed [derivatives](../../../../../../derivative.md) exist continuously and $df/dg\ne0$ on a neighborhood, so the [inverse function theorem](../../../../../../inverse-function-theorem.md) provides a local inverse. Put $p=df/dg$, $q=d^2f/dg^2$, and $r=d^3f/dg^3$. The [chain rule](../../../../../../chain-rule.md) gives $d/df=p^{-1}d/dg$, so

$$
\frac{dg}{df}=\frac1p,\qquad
\frac{d^2g}{df^2}=\frac1p\frac d{dg}\frac1p=-\frac q{p^3}.
$$

Differentiate once more:

$$
\frac{d^3g}{df^3}=\frac1p\frac d{dg}(-qp^{-3})
=-\frac r{p^4}+\frac{3q^2}{p^5}.
$$

Thus the [first three derivatives of an inverse function](../../../../../../first-three-derivatives-of-an-inverse-function.md) are

$$
\boxed{\frac{dg}{df}=\frac1{df/dg},\qquad
\frac{d^2g}{df^2}=-\frac{d^2f/dg^2}{(df/dg)^3},\qquad
\frac{d^3g}{df^3}=
\frac{3(d^2f/dg^2)^2-(df/dg)(d^3f/dg^3)}{(df/dg)^5}.}
$$

All forward [derivatives](../../../../../../derivative.md) on the right are evaluated at the corresponding value $g(f)$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [15](../../../15.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
