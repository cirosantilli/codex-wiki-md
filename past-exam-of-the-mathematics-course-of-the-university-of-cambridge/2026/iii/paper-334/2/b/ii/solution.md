<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [advection-diffusion equation](../../../../../../../advection-diffusion-equation.md) is

$$
c_t+u(y)c_x=D(c_{xx}+c_{yy}),
\qquad
u(y)=\frac Uh y.
$$

Write

$$
c=\bar c(x,t)+c'(x,y,t),
\qquad
\overline{c'}=0,
$$

where the bar is the cross-gap average. In the long, late-time Taylor regime, $c'$ adjusts rapidly across the gap while $\bar c$ varies slowly along the cell. The leading fluctuation balance is

$$
\boxed{
u(y)\bar c_x=Dc'_{yy}}.
$$

Its scaling is

$$
\frac{U\bar c}{L}\sim\frac{Dc'}{h^2},
\qquad
\boxed{
\frac{c'}{\bar c}
\sim\frac{Uh^2}{DL}
=\operatorname{Pe}_h\frac hL\ll1}.
$$

This final inequality is precisely the transverse-equilibration condition from part i.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 334](../../../../paper-334-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
