<h1 id="d/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The theorem gives

$$
F'(t)=-2\int_0^\infty xe^{-x^2}\sin(2xt)dx
=\int_0^\infty (e^{-x^2})'\sin(2xt)dx.
$$

[Integration by parts](../../../../../integration-by-parts.md) has zero boundary term: the sine vanishes at zero and the [Gaussian](../../../../../normal-distribution.md) tends to zero at infinity. Hence $F'(t)=-2t\int_0^\infty e^{-x^2}\cos(2xt)dx=-2tF(t)$.

The same [Gaussian](../../../../../normal-distribution.md) majorant and dominated convergence give [continuity](../../../../../continuous-function.md) at zero, where the allowed [Gaussian integral](../../../../../gaussian-integral.md) gives $F(0)=\sqrt\pi/2$. The differential equation implies $(e^{t^2}F(t))'=0$; [continuity](../../../../../continuous-function.md) at zero fixes that constant. Thus

$$
\boxed{F(t)=\frac{\sqrt\pi}{2}e^{-t^2}\qquad(0\leq t<b).}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [D](../../../d.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
