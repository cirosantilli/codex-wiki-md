<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $g>0$ be the gravitational acceleration, and let $y$ denote positive downward depth. For a frictionless particle released from rest, [conservation of energy](../../../../conservation-of-energy.md) gives $v^2=2gy$. The [arc length](../../../../arc-length.md) element of $(x,-y(x))$ is $ds=\sqrt{1+y'^2}\,dx$, so the [travel time](../../../../travel-time.md) and length are

$$
T[y]=\frac1{\sqrt{2g}}\int_0^1\frac{\sqrt{1+y'^2}}{\sqrt y}\,dx,\qquad S[y]=\int_0^1\sqrt{1+y'^2}\,dx.
$$

For a finite-time single arch, require $y>0$ in $0<x<1$, $y(0)=y(1)=0$, and interpret the endpoint integrals improperly. At a regular constrained minimizer with $S[y]=L$, the [Lagrange multiplier](../../../../lagrange-multiplier.md) rule for an [isoperimetric constraint](../../../../isoperimetric-constraint.md) makes $\sqrt{2g}\,T+\lambda(S-L)$ stationary. Dropping the constant $-\lambda L$ gives

$$
\boxed{I[y]=\int_0^1(y^{-1/2}+\lambda)\sqrt{1+y'^2}\,dx,\qquad y(0)=y(1)=0.}
$$

For $L>1$ the constraint is regular under interior [variations](../../../../variation.md): if its first variation vanished for every compactly supported variation, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) for $S$ would force $y'$ constant, hence $y\equiv0$ and $S=1$, a contradiction. Thus the multiplier is justified for a nondegenerate arch.

**The printed case $L=1$ is degenerate.** Since $\sqrt{1+y'^2}\ge1$, equality of the length with the horizontal separation forces $y'=0$ and $y=0$. A particle initially at rest then has no tangential gravitational acceleration and cannot complete the trip. Its [travel time](../../../../travel-time.md) is infinite. The finite-time calculation therefore concerns $L>1$, with endpoint regularity qualified below.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
