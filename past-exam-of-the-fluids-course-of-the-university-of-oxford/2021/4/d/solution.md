<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [Joukowski map](../../../../joukowski-map.md) with $|c|<a$, in particular its intended range $0\leq c<a/2$. On the original circle,

$$
X=\left(a+\frac{c^2}{a}\right)\cos\theta,\qquad
Y=\left(a-\frac{c^2}{a}\right)\sin\theta.
$$

Define the exterior inverse

$$
f(Z)=\frac{Z+\sqrt{Z^2-4c^2}}2,
$$

where the [holomorphic square root](../../../../holomorphic-square-root.md) is chosen so that $\sqrt{Z^2-4c^2}\sim Z$ at infinity. Then $f(Z)\sim Z$ is the branch mapping the exterior of the [ellipse](../../../../ellipse.md) to $|z|>a$. Composition of the zero-[circulation](../../../../circulation-physics.md) [complex potential](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) from part 4(c) with this inverse gives

$$
\boxed{W(Z)=\beta e^{i\alpha}f(Z)^2
+\frac{\beta a^4e^{-i\alpha}}{f(Z)^2}.}
$$

The [ellipse](../../../../ellipse.md) is a [streamline](../../../../streamline.md) because its inverse image is the circle, and $W(Z)\sim\beta e^{i\alpha}Z^2$ at infinity. An additive constant in the [complex potential](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) has no effect on the [velocity](../../../../velocity.md).

The transformed [complex velocity](../../../../complex-velocity.md) obeys the [chain rule](../../../../chain-rule.md):

$$
\frac{dW}{dZ}=\frac{dw/dz}{dZ/dz}
=\frac{2\beta e^{i\alpha}z-2\beta a^4e^{-i\alpha}z^{-3}}{1-c^2/z^2}.
$$

Since $|c|<a$, the denominator is nonzero on and outside $|z|=a$. The four [stagnation points](../../../../stagnation-point.md) therefore come from

$$
z^4=a^4e^{-2i\alpha},\qquad
z_n=ae^{i\theta_n},\qquad \theta_n=-\frac\alpha2+\frac{n\pi}2,\quad n=0,1,2,3.
$$

Their physical locations are

$$
\boxed{Z_n=\left(a+\frac{c^2}{a}\right)\cos\theta_n
+i\left(a-\frac{c^2}{a}\right)\sin\theta_n,\qquad n=0,1,2,3.}
$$

They all lie on the [ellipse](../../../../ellipse.md), and their positions are independent of $\beta>0$, which only sets the overall [speed](../../../../speed.md) scale.

The printed restriction that $c$ is real and $c<a/2$ is insufficient literally: $c=-2a$ satisfies it but makes $dZ/dz=0$ at $z=2a$ in the exterior, so there is no exterior [conformal map](../../../../conformal-map.md) of the claimed type; the stated minor semiaxis would also be negative. The intended positive-parameter range, or more generally $|c|<a$, is needed for the above solution. The reference to a sphere in the source is a wording slip: the geometry is two-dimensional flow around the mapped cylinder's elliptical cross-section.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
