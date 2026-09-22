<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

Write $z=x+iy$ and $w=u+iv$. Multiplying the numerator and denominator of the [Möbius transformation](../../../../../mobius-transformation.md) by $1+\bar z$ gives

$$
u=\frac{2y}{(1+x)^2+y^2},\qquad
v=\frac{1-x^2-y^2}{(1+x)^2+y^2}>0.
$$

Pull back the given upper-half-plane solution to obtain the [harmonic measure of a semicircle in a disk](../../../../../harmonic-measure-of-a-semicircle-in-a-disk.md):

$$
\boxed{F(x,y)=\frac12+\frac1\pi\arctan\left(\frac{2y}{1-x^2-y^2}\right),\qquad x^2+y^2<1.}
$$

The principal real arctangent is appropriate because $v>0$. By [conformal invariance of harmonicity](../../../../../conformal-invariance-of-harmonicity.md), composing a [harmonic function](../../../../../harmonic-function.md) with this analytic conformal map is harmonic. More explicitly, $\Delta_z(f\circ w)=|w'(z)|^2(\Delta_w f)\circ w=0$. At a boundary point on the open upper semicircle the ratio tends to $+\infty$, yielding one; on the lower semicircle it tends to $-\infty$, yielding zero.

At $z=\pm1$ the two boundary prescriptions jump, so no continuous boundary value can be imposed there and the interior limit depends on the approach. The bounded harmonic solution is interpreted with the specified values away from those endpoints. Boundedness also supplies the usual uniqueness for this [Dirichlet problem](../../../../../dirichlet-problem.md); without a boundedness or comparable regularity restriction, singular harmonic functions at the omitted endpoints would allow extra solutions.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
