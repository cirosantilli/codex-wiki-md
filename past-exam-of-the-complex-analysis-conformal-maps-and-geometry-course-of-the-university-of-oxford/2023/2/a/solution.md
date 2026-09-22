<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [conformal invariance of extremal length](../../../../conformal-invariance-of-extremal-length.md), work first on $1<|w|<R$. For a [conformal metric](../../../../conformal-metric.md) $\rho$, let $L_\rho$ be the infimum of lengths of curves joining the two circles, and $A_\rho$ its area. Each radial segment is admissible, so the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives, for every angle,

$$
L_\rho^2\leq\left(\int_1^R\rho(se^{i\theta})ds\right)^2\leq\log R\int_1^R\rho(se^{i\theta})^2s\,ds.
$$

Integrating in angle gives $2\pi L_\rho^2\leq A_\rho\log R$. Conversely, $\rho(w)=1/|w|$ has shortest joining length $\log R$ and area $2\pi\log R$, attaining the bound. Thus the [conformal modulus of an annulus](../../../../conformal-modulus-of-an-annulus.md) gives

$$
\boxed{d_\Omega(E,F)=\frac{\log R}{2\pi},\qquad\rho_\Omega(z)=c\left|\frac{\psi'(z)}{\psi(z)}\right|,\quad c>0}.
$$

The second formula is the pullback of $c/|w|$ by $\psi$. Pullback preserves curve lengths and metric area, so every displayed positive multiple is an extremal metric in $\Omega$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the complex analysis: conformal maps and geometry course of the University of Oxford](../../../split.md)
5. [Complex analysis: conformal maps and geometry course of the University of Oxford](../../../../complex-analysis-conformal-maps-and-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
