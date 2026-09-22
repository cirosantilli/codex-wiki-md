<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed $t\in[0,1]$, [De Casteljau's algorithm](../../../../../de-casteljau-s-algorithm.md) first takes the same fractional position along both adjacent sides of the [control polygon](../../../../../control-polygon.md):

$$
L(t)=(1-t)A+tB=(-2+2t,t),\qquad
R(t)=(1-t)B+tC=(0,1-t).
$$

It then applies another [linear interpolation](../../../../../linear-interpolation.md) with that same $t$:

$$
F(t)=(1-t)L(t)+tR(t)
=(1-t)^2A+2t(1-t)B+t^2C.
$$

This is the degree-two [Bernstein basis](../../../../../bernstein-basis.md) representation of a quadratic [Bézier curve](../../../../../bezier-curve.md). Its [coordinate](../../../../../coordinate-linear-algebra.md) [polynomials](../../../../../polynomial-split.md) are

$$
\boxed{F_x(t)=-2(1-t)^2=-2+4t-2t^2,\qquad
F_y(t)=2t(1-t)=2t-2t^2.}
$$

The degree is exactly two, since its second [derivative](../../../../../derivative.md) $(-4,-4)$ is nonzero. As a check on the construction, at $t=1/2$ the two intermediate [points](../../../../../point-geometry.md) are $(-1,1/2)$ and $(0,1/2)$ and their [midpoint](../../../../../midpoint.md) is $F(1/2)=(-1/2,1/2)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
