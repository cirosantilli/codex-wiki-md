<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

For a regular smooth constraint $g=0$, meaning $\nabla g\ne0$ at the point, constrained stationarity requires $\nabla f=\lambda\nabla g$. Solve these [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations together with the constraint, then compare candidate values and possible boundary or singular cases.

Let $r>0$ and $h>0$ be cylinder radius and height. Its [volume](../../../../../volume.md) is $V=\pi r^2h$ and the surface-area constraint is $2\pi r^2+2\pi rh=A$. The multiplier equations are

$$
2\pi rh=\lambda(4\pi r+2\pi h),\qquad
\pi r^2=\lambda(2\pi r).
$$

The second gives $\lambda=r/2$, and substituting into the first gives $h=2r$. Consequently $6\pi r^2=A$. To check global maximality, eliminate $h$ and obtain $V(r)=Ar/2-\pi r^3$ on $0<r<\sqrt{A/(2\pi)}$; it tends to zero at both ends and has exactly this one stationary point. **The largest volume is**

$$
\boxed{r=\sqrt{\frac A{6\pi}},\quad h=2r,\quad
V_{\max}=\frac{A^{3/2}}{3\sqrt{6\pi}}.}
$$

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
