<h1 id="section-b/b8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [Euler strut](../../../../../../euler-strut.md) is a slender initially straight elastic column under axial compression. For a uniform [bending stiffness](../../../../../../bending-stiffness.md) $EI$ and a small transverse [displacement](../../../../../../displacement.md) $y(x)$, the second-order [potential energy](../../../../../../potential-energy.md) under a conservative compressive load $P$ is

$$
\Pi^{(2)}=\frac12\int_0^L\left[EI(y'')^2-P(y')^2\right]dx.
$$

The bending term is positive; shortening releases load potential. Stationarity yields $EIy^{(4)}+Py''=0$. Pinned ends impose $y(0)=y(L)=0$ and zero end [bending moments](../../../../../../bending-moment.md), $y''(0)=y''(L)=0$. Substitution of $y=A\sin(n\pi x/L)$ gives

$$
P_n=\frac{n^2\pi^2EI}{L^2},\qquad
\boxed{P_{\rm cr}=\frac{\pi^2EI}{L^2}.}
$$

The straight configuration loses stability first in the longest admissible bending mode. The [second moment of area](../../../../../../second-moment-of-area.md) $I=\int z^2dA$ is geometric, not a [mass](../../../../../../mass.md) [moment of inertia](../../../../../../moment-of-inertia.md). Boundary conditions matter: a fixed-free column has effective [length](../../../../../../length.md) $2L$, while fixed-fixed ends have effective [length](../../../../../../length.md) $L/2$, changing the threshold by factors $1/4$ and $4$. Slenderness, elastic material response, alignment and the weak bending direction must be checked. Imperfections produce bending before the ideal threshold, and a short column can yield or crush first. Linear buckling theory does not predict an unlimited deflection or a complete postbuckling curve.

<a id="section-b/b8/c/image-euler-strut-instability"></a>
![](../../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1-euler-strut.png)

**[Figure 2](#section-b/b8/c/image-euler-strut-instability). Euler strut instability**. Ideal pinned modes and energy curvature.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
