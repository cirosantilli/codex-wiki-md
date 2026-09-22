<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the positive causal sign convention $\mathcal L=\partial_y-x\partial_x^2$, so the forced equation is $\mathcal Lu=-xy^{-2}e^{-x/y}$. With source $(\xi,\tau)$, a forward [Green's function](../../../../../green-s-function-split.md) satisfies

$$
\boxed{(\partial_y-x\partial_x^2)G(x,y;\xi,\tau)=\delta(x-\xi)\delta(y-\tau),\qquad G=0\text{ for }y<\tau.}
$$

It vanishes at $x=0$, decays at spatial infinity in the chosen bounded evolution class, and has the temporal jump $G(x,\tau^+;\xi,\tau)=\delta(x-\xi)$. Away from the source it solves the homogeneous equation. Equivalently one may reverse both the Green-function operator and its source sign to use the original printed operator.

To select the physical zero-initial-data solution one also excludes extra corner-source terms of the kind found in (b). With this causal bounded convention the solution representation is

$$
u(x,y)=-\int_0^y\int_0^\infty G(x,y;\xi,\tau)\frac\xi{\tau^2}e^{-\xi/\tau}\,d\xi\,d\tau.
$$

A mere pointwise statement of the three boundary limits does not by itself provide that uniqueness convention.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
