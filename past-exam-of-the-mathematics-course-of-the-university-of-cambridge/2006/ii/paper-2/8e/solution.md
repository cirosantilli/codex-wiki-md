<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

Take a [Hankel contour](../../../../../hankel-contour.md) $C_\eta$ around the positive real axis, going from infinity on its lower side toward a circle of radius $0<\eta<1$, clockwise around that circle, then out along the upper side. Use $0\le\arg z\le2\pi$ and define

$$
H(t)=\int_{C_\eta}\frac{z^te^{-z}}{1+z}\,dz.
$$

This is an [entire function](../../../../../entire-function.md) of $t$: the small circle stays away from zero and the pole at $-1$, while the exponentially decaying rays converge uniformly for $t$ in [compact subsets](../../../../../compact-space.md). [Contour deformation](../../../../../contour-deformation.md) shows independence of $\eta$. For $\Re t>-1$, let $\eta\to0$. The upper ray contributes $F(t)$, the lower ray contributes $-e^{2\pi it}F(t)$, and the small-circle contribution vanishes. Thus the [analytic continuation](../../../../../analytic-continuation.md) is

$$
\boxed{F(t)=\frac{H(t)}{1-e^{2\pi it}}.}
$$

The only apparent singularities are at integers. At the [nonnegative integers](../../../../../natural-number.md) they are removable because the original integral is [holomorphic](../../../../../complex-differentiability-at-a-point.md) throughout $\Re t>-1$. Hence singularities can occur only at $-1,-2,\ldots$.

In fact all of those points are [simple poles](../../../../../simple-pole.md). At $t=-n-1$ the two rays cancel and the clockwise circle gives $H(-n-1)=-2\pi i\,c_n$, where

$$
c_n=[z^n]\frac{e^{-z}}{1+z}=(-1)^n\sum_{j=0}^n\frac1{j!}\ne0.
$$

Since the denominator has derivative $-2\pi i$ at each integer, the residue at $-n-1$ is $c_n$. The parameter has been called $t$ consistently; the final use of $z$ for this parameter in the printed question is harmless notation.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
