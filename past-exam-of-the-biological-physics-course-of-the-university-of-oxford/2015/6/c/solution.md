<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The given [facilitated target search](../../../../facilitated-target-search.md) time contains a rising term $L\lambda/D_1$ and a falling term $V/(D_3\lambda)$. Longer sliding explores more neighbouring [DNA](../../../../deoxyribonucleic-acid.md) without another bulk encounter, reducing the cost of three-dimensional relocation; but it also spends longer revisiting local contour. Roughly $L/\lambda$ local scans, each taking time of order $\lambda^2/D_1$, give the first term. The second represents the bulk encounter cost for an effective capturable contour range of order $\lambda$, with a [Smoluchowski association rate](../../../../smoluchowski-association-rate.md) scaling as $D_3\lambda$. Numerical geometrical factors are already absorbed in the stipulated scaling formula.

Differentiating at fixed positive $L,V,D_1,D_3$ gives

$$
\frac{d\tau_{1+3}}{d\lambda}=\frac L{D_1}-\frac V{D_3\lambda^2},\qquad
\boxed{\lambda_* =\sqrt{\frac{VD_1}{LD_3}},\qquad
\tau_{\min}=2\sqrt{\frac{LV}{D_1D_3}}.}
$$

The second derivative $2V/(D_3\lambda^3)>0$ proves the minimum is unique. The two contributions are equal there. The formal curve diverges at both zero and infinite $\lambda$; real sliding lengths are bounded, for example by the available contour, so an inaccessible optimum must be replaced by the nearest physical boundary. In dimensionless form, $\tau/\tau_{\min}=(u+u^{-1})/2$ with $u=\lambda/\lambda_*$. The right panel of the original illustration shows its minimum and the two contributing terms. The supplied expression does not include a factor of 6000; it should not silently be identified with the preceding earliest-encounter estimate.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
