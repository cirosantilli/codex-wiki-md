<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A negative value of either radius makes the intersection empty. Assume henceforth $\alpha,\beta\geq0$ and put $D=|d|$. If $D=0$, the two [spheres](../../../../sphere.md) are concentric: their intersection is the entire sphere when $\alpha=\beta>0$, the origin when $\alpha=\beta=0$, and empty otherwise.

For $D>0$, subtract their squared equations to obtain the plane

$$
x\cdot d=\frac{D^2+\alpha^2-\beta^2}{2}.
$$

The [centre of the circle of intersection of two spheres](../../../../centre-of-the-circle-of-intersection-of-two-spheres.md) is $x_0=s\widehat d$, where

$$
\widehat d=\frac dD,\qquad s=\frac{D^2+\alpha^2-\beta^2}{2D}.
$$

Every point of that plane can be written $x=x_0+u$ with $u\cdot d=0$. Its remaining equation is

$$
|u|^2=\rho^2=\alpha^2-s^2
=\frac{[(\alpha+\beta)^2-D^2][D^2-(\alpha-\beta)^2]}{4D^2}.
$$

Thus **the intersection is a circle** of centre $x_0$ and radius $\rho$ if $|\alpha-\beta|<D<\alpha+\beta$; **a single point** $x_0$ at either equality; and **empty** otherwise. These include tangency to a zero-radius sphere. A negative $s$ places the circle centre beyond the first sphere's centre on the side opposite $d$.

In $\mathbb R^n$ for $n\geq2$, the same calculation gives an $(n-2)$-dimensional [sphere](../../../../sphere.md) in the perpendicular affine hyperplane when $\rho^2>0$, a point when $\rho^2=0$, and the empty set otherwise. In two dimensions the positive-radius case consists of two points. In one dimension the perpendicular hyperplane has only one point, so a nonconcentric intersection exists only when $\rho^2=0$. Concentric equal-radius sets coincide in every dimension.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
