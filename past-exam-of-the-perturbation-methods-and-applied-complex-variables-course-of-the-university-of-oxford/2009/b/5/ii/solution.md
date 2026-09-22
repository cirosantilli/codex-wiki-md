<h1 id="b/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an admissible [Laplace integral solution](../../../../../laplace-integral-solution.md), differentiation under the integral sign and [integration by parts](../../../../../integration-by-parts.md) give

$$
\begin{aligned}
2w''+2zw'+w
&=\int_\Gamma(2\zeta^2+1)g\,e^{z\zeta}\,d\zeta
+2\int_\Gamma\zeta g\,\frac{d}{d\zeta}e^{z\zeta}\,d\zeta\\
&=[2\zeta g e^{z\zeta}]_{\partial\Gamma}
+\int_\Gamma\{(2\zeta^2-1)g-2\zeta g'\}e^{z\zeta}\,d\zeta.
\end{aligned}
$$

Choose endpoints for which the boundary term vanishes. Setting the density in braces to zero gives

$$
\frac{g'}g=\zeta-\frac1{2\zeta},\qquad
\boxed{g=A\zeta^{-1/2}e^{\zeta^2/2}.}
$$

Two suitable contours are the rays $\Gamma_+:0\to+i\infty$ and $\Gamma_-:0\to-i\infty$, with a continuous square-root branch on each ray. The Gaussian decays at infinity, and $\zeta g=O(\zeta^{1/2})$ tends to zero at the finite endpoint. The integrals converge for every finite $z$.

To check independence rather than merely exhibit different paths, define

$$
J_0=\int_0^\infty s^{-1/2}e^{-s^2/2}\,ds>0,\qquad
J_1=\int_0^\infty s^{1/2}e^{-s^2/2}\,ds>0.
$$

With unit normalization, the two solutions satisfy $w_\pm(0)=e^{\pm i\pi/4}J_0$ and $w_\pm'(0)=\pm i e^{\pm i\pi/4}J_1$. Their [Wronskian](../../../../../wronskian.md) at zero is $-2iJ_0J_1\ne0$, so they form an independent pair.

Strictly, the printed necessity claim requires an injective contour-transform class as well as vanishing endpoint terms. An arbitrary contour representation may contain a [null weight in a contour Laplace representation](../../../../../null-weight-in-a-contour-laplace-representation.md), so a nonzero solution alone does not force every representing $g$ to have the displayed form. The calculation constructs the canonical density and two valid independent solutions; it does not assume uniqueness for unrestricted contour densities.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
