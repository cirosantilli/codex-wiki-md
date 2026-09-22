<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [Lagrange multiplier](../../../../../lagrange-multiplier.md) to maximize $V=\pi r^2h$ subject to $2\pi r(r+h)=A$, with $r,h>0$. The equations $\nabla V=\lambda\nabla A$ are

$$
2\pi rh=\lambda(4\pi r+2\pi h),\qquad\pi r^2=2\lambda\pi r.
$$

The second equation gives $\lambda=r/2$. Substituting into the first gives $2rh=r(2r+h)$, hence $h=2r$. The [constraint](../../../../../constraint-mechanics.md) then gives $A=6\pi r^2$, so

$$
\boxed{r=\sqrt{\frac A{6\pi}},\qquad h=2\sqrt{\frac A{6\pi}},\qquad V_{\max}=2\pi\left(\frac A{6\pi}\right)^{3/2}=\frac13\sqrt{\frac{A^3}{6\pi}}.}
$$

This is the same aspect ratio as the [minimum-area closed cylinder at fixed volume](../../../../../minimum-area-closed-cylinder-at-fixed-volume.md). To confirm maximality directly, eliminate $h$: $V(r)=Ar/2-\pi r^3$ on $0<r<\sqrt{A/(2\pi)}$. Its only stationary point is the value above, its second [derivative](../../../../../derivative.md) there is negative, and the [volume](../../../../../volume.md) tends to zero at either end of the interval.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
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
